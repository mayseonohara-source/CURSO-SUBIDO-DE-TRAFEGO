# Agente Veltro - Especialista em Trafego Pago

Skill do Claude Agent SDK baseada no **Metodo Subido de Pedro Sobral** (89 aulas em 10 modulos). Pensada para ser o cerebro do **Veltro** (gestor de trafego).

## O que ela faz

O agente assume 4 papeis no Veltro, escolhidos pelo contexto da conversa:

1. **Consultor estrategico** - planejamento de midia, estrutura de campanhas, escolha de canal/objetivo/orcamento.
2. **Otimizador de campanhas** - diagnostico de metricas (CPA, CTR, ROAS, CPM, CPC, CPL) e decisao sobre as 6 alavancas de otimizacao.
3. **Criador de criativos** - gancho, corpo, CTA; 8 tipos de gancho do Metodo Subido; anuncios camuflados vs explicitos.
4. **SOS bloqueios** - blindagem de ativos, triagem de rejeicoes, plano de retomada em conta caida.

## Estrutura

```
~/.claude/skills/trafego-pago-veltro/
├── SKILL.md                    # Identidade do agente + fluxo + comandos
├── README.md                   # Este arquivo
└── references/
    ├── metodo-subido.md        # 12 conceitos + 5 habilidades + rotina
    ├── meta-ads.md             # Facebook + Instagram playbook
    ├── google-ads.md           # Search + YouTube + Display + Pmax
    ├── tiktok-ads.md           # TikTok Ads + Spark Ads + UGC
    ├── linkedin-ads.md         # B2B playbook
    ├── criativos.md            # 7 passos + 8 tipos de gancho + VSL
    ├── metricas.md             # Principais + secundarias + benchmarks BR
    ├── otimizacao.md           # 6 alavancas + rotina semanal
    ├── estrategia.md           # Por nicho (e-com, fisico, infoproduto, lancamento, B2B)
    ├── bloqueios-sos.md        # Blindagem + contingencia PCB + nichos sensiveis
    └── diagnostico.md          # Framework de diagnostico de campanha travada
```

## Como ativar

### 1. Dentro do Claude Code (local)

A skill ja esta registrada. O Claude ativa automaticamente quando o usuario mencionar:
- Campanhas, anuncios, trafego pago, gestao de midia
- Meta Ads, Google Ads, TikTok Ads, LinkedIn Ads
- CPA, CTR, ROAS, CPM, CPC, CPL, pixel, ICP, segmentacao
- Bloqueio de conta, BM, Business Manager
- Qualquer fluxo do Veltro

Invocacao manual tambem funciona:
```
/trafego-pago-veltro
```

### 2. Dentro do Veltro (como backend agent)

O arquivo `SKILL.md` e um system prompt completo. Para plugar no Veltro:

**Opcao A - System prompt direto (mais simples):**
- Copie o conteudo de `SKILL.md` + concatene as referencias relevantes ao contexto da conversa no system prompt.

**Opcao B - Claude Agent SDK (recomendado):**
```python
from anthropic import Anthropic

client = Anthropic()

# Le SKILL.md + monta sistema
with open("trafego-pago-veltro/SKILL.md") as f:
    system_prompt = f.read()

# Carrega referencia sob demanda conforme keyword
# (implementar RAG leve: quando usuario fala "bloqueio" -> carrega bloqueios-sos.md)

response = client.messages.create(
    model="claude-opus-4-6",
    system=system_prompt,
    messages=[{"role": "user", "content": user_input}]
)
```

**Opcao C - RAG completo:**
- Indexe os 11 arquivos `.md` em um vector store.
- Faca retrieval pelas top 2-3 referencias relevantes por turno.
- Injete no system prompt do modelo.

## Comandos do agente

O Veltro pode expor estes comandos como botoes ou slash-commands:

| Comando | O que faz |
|---|---|
| `/plano [nicho] [objetivo] [verba]` | Gera planejamento completo de campanhas |
| `/anuncio [nicho] [angulo] [formato]` | Gera 3 variacoes de anuncio (gancho + corpo + CTA) |
| `/otimizar [contexto + metricas]` | Diagnostica o que otimizar e em que ordem |
| `/icp [nicho]` | Gera pesquisa de ICP estruturada |
| `/sos [problema]` | Triagem de bloqueio com plano de retomada |
| `/nomenclatura [objetivo] [publico] [posicionamento]` | Gera nome padrao Subido |
| `/metricas [numeros]` | Interpretacao + recomendacao |
| `/escala [campanha performando]` | Plano de escala vertical/horizontal |

## Principios inegociaveis

1. Teoria > botao. Ancora em conceito antes de passo-a-passo.
2. Anuncio e o segredo. 80% do resultado vem daqui.
3. Ganha quem testa mais. Minimo 6 anuncios ativos por conjunto.
4. Otimizar = disciplina + checklist, nao improviso.
5. Nomenclatura traz ROI.
6. Basico bem feito no traqueamento (pixel + CAPI).
7. Sempre parta do ICP.
8. Portugues do Brasil, tom direto, exemplos com numeros.

## Fonte

Conhecimento sintetizado a partir do **Curso Subido de Trafego** de Pedro Sobral (Comunidade Subido de Trafego), mapeado no repositorio `mayseonohara-source/CURSO-SUBIDO-DE-TRAFEGO` (89 aulas / 10 modulos). Sintese proprietaria em linguagem do agente para uso interno no Veltro.

Acesso ao curso original: https://www.subido.com.br

## Proximos passos

- [ ] Integrar com gerenciadores (Meta Business API / Google Ads API) para leitura de metricas em tempo real.
- [ ] Adicionar modulo de auto-relatorio semanal por cliente.
- [ ] Treinar fine-tuning com historico de conversas reais dos gestores no Veltro.
- [ ] Criar modulo "Escala" com sinais de quando horizontal vs vertical.
