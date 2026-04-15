# Metricas - Algo simples que todo mundo complica

## Principio central

Gestor de trafego NAO precisa ser bom em matematica. Precisa entender **2 grupos de metricas** e a relacao entre eles.

---

## Grupo 1: Metricas PRINCIPAIS (quanto custa o resultado)

Respondem "a campanha esta dando certo?". Voce julga a campanha por elas.

### Metricas-base

| Metrica | O que mede | Formula |
|---|---|---|
| **Impressoes** | Quantas vezes o anuncio apareceu | Contagem |
| **CPM** | Custo por 1000 impressoes | (Gasto / Impressoes) × 1000 |
| **Cliques** | Quantos cliques teve | Contagem |
| **CTR** | Taxa de clique | Cliques / Impressoes |
| **CPC** | Custo por clique | Gasto / Cliques |
| **Sessoes** | Pessoas que chegaram no site | Google Analytics |
| **Connect rate** | Sessoes / Cliques | Mede se o site abre bem |
| **CPS** | Custo por sessao | Gasto / Sessoes |

### Metricas de resultado final

| Metrica | Use em |
|---|---|
| **Leads** + **CPL** (custo por lead) | Captura de contato |
| **Vendas** + **CPA** (custo por aquisicao) | E-commerce, infoproduto |
| **ROAS** (retorno sobre gasto) | E-commerce - receita / gasto |
| **Ticket medio** | E-commerce |
| **Taxa de conversao de site** | Conversoes / Sessoes |
| **Taxa de conversao de lista** | Vendas / Leads |
| **Mensagens** + **CPMsg** | WhatsApp, Instagram DM |

### Metricas de engajamento (distribuicao de conteudo)

| Metrica | O que mede |
|---|---|
| **Seguidores / CPSeguidor** | Aquisicao de audiencia |
| **Visualizacao / Custo por view** | Alcance de video |
| **Envolvimento / Custo por envolvimento** | Like + comentario + share |
| **Hook rate** | Views 3s / Impressoes (qualidade do gancho) |

---

## Grupo 2: Metricas SECUNDARIAS (efeito domino)

Voce NAO julga a campanha por elas. Mas elas explicam o PORQUE as principais estao boas ou ruins.

Exemplo: CPA alto (principal). A causa pode estar em:
- CPM alto → leilao competitivo, publico esgotado
- CTR baixo → anuncio fraco
- CPS alto → site lento ou link errado
- Taxa de conversao baixa → pagina de vendas ruim

**Regra mental:** sempre que uma principal piorar, desca nas secundarias ate achar a causa.

---

## Benchmarks Brasil 2025 (ordem de grandeza)

### Meta Ads

| Nicho | CPM esperado | CTR | CPA/CPL |
|---|---|---|---|
| E-commerce fashion | R$ 10-25 | 1.5-3% | CPA R$ 30-80 |
| E-commerce nicho (nutricao, pet) | R$ 15-35 | 1.2-2.5% | CPA R$ 40-120 |
| Infoproduto baixo ticket (R$ 200-500) | R$ 20-40 | 1-2% | CPA R$ 30-80 |
| Infoproduto alto ticket (R$ 2k-10k) | R$ 25-50 | 0.8-1.8% | CPL R$ 5-20, CPA R$ 150-600 |
| Servico local (clinica, estetica) | R$ 8-20 | 1.5-3% | CPL R$ 10-40 |
| SaaS B2B | R$ 30-60 | 0.6-1.5% | CPL R$ 25-100 |

### Google Search

| Nicho | CPC esperado | CTR | CPA |
|---|---|---|---|
| Advogado | R$ 15-50 | 4-8% | CPA R$ 80-300 |
| Servico local | R$ 3-12 | 4-10% | CPL R$ 15-60 |
| E-commerce produto especifico | R$ 1-5 | 3-6% | CPA R$ 20-80 |
| SaaS B2B | R$ 8-30 | 2-5% | CPL R$ 50-200 |

**AVISO:** sao ordens de grandeza. Varia muito por regiao, sazonalidade e concorrencia.

---

## Como interpretar (framework de diagnostico rapido)

Ao receber metricas do usuario, siga:

### 1. CPM muito alto
- Publico esgotado (frequencia alta)
- Leilao sazonal (Black Friday, eleicao)
- Conta nova sem historico
- Nicho sensivel com poucos anunciantes na fila
- → **Acao:** rotacionar criativo, ampliar publico, esperar 3-5 dias antes de agir

### 2. CTR baixo (< 1% Meta, < 3% Google Search)
- Anuncio ruim (gancho fraco, imagem pobre)
- Publico errado para o anuncio
- Canibalizacao de campanhas (seus proprios anuncios competindo)
- → **Acao:** subir 3 novos anuncios com ganchos diferentes. Pausar os que estao piores.

### 3. CTR alto mas CPA alto (o "enganador")
- Anuncio chama atencao mas leva publico errado (clickbait)
- Pagina de destino ruim
- Preco / oferta nao cola com prova social
- → **Acao:** testar LP alternativa OU endurecer copy do anuncio (remover promessa exagerada)

### 4. CPA bom mas pouco volume
- Orcamento insuficiente
- Publico pequeno esgotando
- → **Acao:** aumentar orcamento 20% OU duplicar conjunto com publico ampliado. Nao suba 100% de uma vez (reseta aprendizado).

### 5. CPA excelente e volume crescendo
- Escalar: +20% orcamento a cada 3-4 dias OU duplicacao horizontal (mais conjuntos com publicos novos)
- Monitorar se CPA mantem

---

## Como manipular (sem enganar)

"Manipular metricas" nao e mentir. E escolher qual mostrar para qual stakeholder:

| Stakeholder | Mostre |
|---|---|
| Dono de e-commerce | ROAS + Receita + Ticket medio |
| Dono de infoproduto | CPL + Taxa de conversao + Receita + ROI |
| Dono de servico local | Leads qualificados + CPL + agendamentos |
| Voce (gestor, interno) | Tudo, inclusive secundarias |

**Regra:** para o cliente, sempre traduza em dinheiro. "CPA R$ 45" nao significa nada. "Pra cada R$ 45 gastos, o senhor fatura R$ 200" significa.

---

## Como documentar (rotina semanal)

Planilha simples:

| Data | Conjunto | Gasto | Impressoes | Cliques | CTR | CPM | Conversoes | CPA | Observacao |
|---|---|---|---|---|---|---|---|---|---|
| 15/04 | 01 - LLA 3% | R$ 150 | 8.000 | 180 | 2.25% | R$ 18 | 5 | R$ 30 | Escalei +20% ontem |

Atualize diariamente. Decisao de otimizar sem documentacao = adivinhacao.

---

## Regras de ouro

1. **Nao julgue campanha em menos de 72h** (aprendizado).
2. **Nao julgue anuncio com menos de 1000-2000 impressoes**.
3. **Julgue por janela de 7 dias**, nao por dia ruim.
4. **ROAS e rei em e-commerce**, CPL + taxa de conversao em infoproduto.
5. **Se secundaria subiu a principal, nao olhe so a principal**.
