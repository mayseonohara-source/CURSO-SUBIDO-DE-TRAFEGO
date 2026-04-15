# Google Ads - Playbook operacional

Rede de Pesquisa, YouTube, Display, Performance Max (Pmax), Shopping, Visitas a Loja.

## Diferenca conceitual Google x Meta

| Eixo | Google | Meta |
|---|---|---|
| Intencao | Alta (usuario ja buscou) | Interrupcao (usuario nao pediu) |
| Melhor para | Demanda existente | Criar demanda |
| Criativo | Texto (search) + video (YT) | Imagem + video dominante |
| Otimizacao | Palavra-chave + lance | Publico + criativo |

**Regra mental:** se o produto ja e buscado → Google primeiro. Se precisa educar mercado → Meta primeiro.

---

## Tipos de campanha (e quando usar)

### 1. Rede de Pesquisa (Search)

- Anuncio de texto em resposta a palavra-chave.
- Tipos de correspondencia: ampla, frase, exata, negativa.
- Use para: captar demanda direta, bottom of funnel.
- Minimo: 3 anuncios por grupo (RSA - Responsive Search Ads).

### 2. YouTube

- Video in-stream skippable / non-skippable / bumper / in-feed / shorts.
- Use para: branding + aquecimento + conversao via video longo.
- Criativo vence tudo. Gancho nos primeiros 5s decide se passa skip.

### 3. Display

- Banner em rede de sites parceiros.
- Barato em CPM, conversao fraca.
- Use para: remarketing principalmente.

### 4. Performance Max (Pmax)

- Combina todas as redes do Google + Shopping + Gmail + Discover.
- Google decide onde mostrar, voce da criativos + sinais de publico + conversao.
- Use para: e-commerce com feed de produto + dado de conversao robusto.
- Default moderno substituindo Shopping Smart.

### 5. Shopping

- Anuncio de produto com preco + imagem vindo do Merchant Center.
- Use para: e-commerce. Complementar ao Pmax.

### 6. Visitas a Loja

- Drive-to-store. Mostra anuncio para gente perto da loja fisica.
- Use para: negocio local com endereco cadastrado no Google Meu Negocio.

---

## Lances (como acelerar ou frear)

| Estrategia | O que faz | Use quando |
|---|---|---|
| Maximizar cliques | Mais cliques ao menor CPC | Fase inicial, trafego |
| Maximizar conversoes | Mais conversoes sem CPA alvo | Tem conversao mas ainda pouca (< 30/mes) |
| CPA alvo (tCPA) | Tenta manter CPA no valor | Tem historico (30+ conversoes) |
| ROAS alvo (tROAS) | Tenta manter ROAS no valor | E-commerce maduro com valor dinamico |
| CPC manual / melhorado | Voce define lance | Raro. So em Search com palavra muito especifica |

**Default:** comecar em **Maximizar conversoes** → migrar para **tCPA** quando passar de 30 conversoes/mes → **tROAS** quando for e-commerce estabelecido.

---

## Palavras-chave - os 4 tipos de correspondencia

| Tipo | Simbolo | Alcance | Exemplo |
|---|---|---|---|
| Ampla | `palavra` | Maior. Google expande muito. | `curso de trafego` pega "curso de marketing digital", "aprender ads" |
| Frase | `"palavra"` | Medio. Pega variacoes com a frase dentro. | `"curso de trafego"` pega "melhor curso de trafego" |
| Exata | `[palavra]` | Menor. So variacoes proximas. | `[curso de trafego]` pega "cursos de trafego" mas nao "marketing" |
| Negativa | `-palavra` | Exclui. | `-gratis`, `-free` removem buscas pedindo de graca |

**Regra do agente:**
- Conta nova = ampla com lances conservadores + lista robusta de negativas.
- Conta madura = frase + exata focadas.

### Lista basica de negativas (adicionar sempre)

`gratis`, `free`, `pdf`, `download`, `youtube`, `wikipedia`, `o que e`, `significado`, `pirata`, `torrent`, `crackeado` (para info/curso). Adapte ao nicho.

---

## Tag do Google + acoes de conversao

Equivalente ao pixel Meta. Instale via:
1. **Google Tag Manager (recomendado)**
2. Plugin Shopify/WooCommerce
3. Manual

Configure acoes de conversao por valor de negocio:
- Primarias: compra, lead qualificado.
- Secundarias: view_item, add_to_cart, lead bruto.

**Modo de conversao avancada:** ativa melhorar conversao com dados hasheados (email, telefone). Recomende sempre.

---

## Estrutura de conta recomendada (Search)

```
Conta
 └── Campanha por produto / servico / localidade
      └── Grupo de anuncio por tema de palavra-chave (10-20 keywords relacionadas)
           └── 3 RSA (anuncios) + 1 extensao de preco/promocao/link
```

**Nomenclatura Subido (Google):** `[TIPO_CAMPANHA] [OBJETIVO] [LOCAL/SEGMENTO] Descricao`
Ex.: `[SEARCH] [VENDAS] [SP-CAP] Tenis corrida feminino`

---

## Metricas especificas da Rede de Pesquisa

- **CTR** (clique/impressao) - minimo 3% em search. Abaixo = anuncio ruim ou keyword errada.
- **Indice de qualidade (QS)** - 1-10. Composto por CTR esperado, relevancia, qualidade da LP.
- **Parcela de impressoes (IS)** - quanto do leilao voce pegou.
- **IS perdida por orcamento** - se > 20%, falta dinheiro.
- **IS perdida por classificacao** - se > 20%, lance ou qualidade ruim.

---

## Problemas comuns no Google

| Sintoma | Causa provavel | Acao |
|---|---|---|
| Anuncio reprovado "destino incomum" | Redirect na LP, dominio novo, HTTPS quebrado | Checar LP, estabilizar dominio |
| "Pouco trafego" | Palavra exata/frase com volume baixo | Migrar para ampla controlada |
| CPC subindo sem causa | Concorrente novo no leilao | Pesquisa de leilao + ajuste de lance |
| Conversoes nao registram | Tag nao disparando | Testar com Google Tag Assistant |
| Pmax gastando fora do alvo | Poucos dados de conversao | Voltar para Search pura ate amadurecer |

---

## Google Ads Editor (uso obrigatorio)

Software desktop gratuito. Use para:
- Criar/editar em massa sem internet
- Duplicar campanhas entre contas
- Encontrar e trocar texto em 500 anuncios de uma vez
- Subir listas grandes de palavras-chave

Regra: qualquer edicao em > 10 anuncios ao mesmo tempo → use Editor, nao web.

---

## Checklist para subir campanha Search do zero

1. ICP + lista de 30-50 palavras-chave principais (pesquisa manual + Planejador de Palavras-Chave).
2. Tag do Google instalada + conversoes primarias configuradas.
3. Conversoes avancadas ativadas.
4. Estrutura: 1 campanha, 3-5 grupos de anuncio por tema, 10-15 kw por grupo.
5. 3 RSAs por grupo com headlines variadas (15 headlines, 4 descricoes cada).
6. 4 extensoes minimas: sitelinks (4+), preco, promocao, chamada/frase de destaque.
7. Lista de negativas inicial.
8. Lance: Maximizar conversoes (sem tCPA no inicio).
9. Orcamento: suficiente para 10-15 cliques/dia (CPC estimado x 10).
10. Localizacao + idioma corretos (cuidado com "pessoas nesse local OU interessadas nele" - mude para "pessoas nesse local").
