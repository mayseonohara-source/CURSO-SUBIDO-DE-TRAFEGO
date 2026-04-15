# Framework de diagnostico - Campanha travada

Use este fluxo quando o usuario disser "minha campanha nao esta funcionando".

## Passo 1 - Reunir contexto (faca em 3 perguntas)

1. **Qual o objetivo e qual a meta de CPA/ROAS?** (sem meta, nao existe "ruim")
2. **Quanto tempo ela esta rodando e quanto ja gastou?**
3. **Me manda os numeros**: impressoes, cliques, CTR, CPM, CPC, conversoes, CPA, gasto total.

Se o usuario nao tiver os numeros, ele precisa levantar antes de qualquer sugestao.

---

## Passo 2 - Validar os pre-requisitos

Antes de tudo, confirme:

- [ ] **Pixel / Tag funcionando?** Conversao aparecendo no gerenciador com valor?
- [ ] **API de conversoes ligada?**
- [ ] **Objetivo de campanha alinhado ao resultado desejado?**
- [ ] **Orcamento e suficiente para a meta?** (< R$ 20/dia em conjunto Meta = fome)
- [ ] **ICP definido?**
- [ ] **Minimo 6 anuncios ativos?**

Se algum falha: **resolver isso primeiro**, antes de otimizar nada.

---

## Passo 3 - Verificar se pode julgar

- [ ] Fora da fase de aprendizado (72h + 50 eventos)?
- [ ] Pelo menos 7 dias de dado?
- [ ] Pelo menos 1000-2000 impressoes por anuncio?
- [ ] Nao e fim de semana / feriado distorcendo?

Se nao: NAO julgar. Dizer ao usuario: "aguarde X dias antes de otimizar".

---

## Passo 4 - Diagnostico por sintoma

### Sintoma: CPM alto
**Causas provaveis:**
- Publico esgotado (frequencia > 3)
- Leilao sazonal (BF, eleicao)
- Nicho pequeno com pouca oferta
- Conta nova sem historico

**Acoes:**
- Ampliar publico (LLA maior, Advantage+)
- Rotacionar criativo
- Esperar 3-5 dias

---

### Sintoma: CTR baixo (< 1% Meta / < 3% Google Search)
**Causas:**
- Anuncio fraco (gancho ruim)
- Publico errado para o anuncio
- Canibalizacao (seu anuncio concorrendo consigo mesmo)

**Acoes:**
- Subir 3 anuncios novos com ganchos diferentes
- Verificar sobreposicao de publico
- Pausar anuncio com CTR < 1% e 2000+ imp

---

### Sintoma: CTR bom mas CPS alto (poucos chegam no site)
**Causas:**
- Site lento
- Link quebrado
- Redirect demais
- Mobile nao otimizado

**Acoes:**
- Testar o link voce mesmo em 3G no celular
- Rodar PageSpeed Insights
- Reduzir redirects

---

### Sintoma: Site recebe visitas mas nao converte
**Causas:**
- Pagina de destino fraca
- Preco fora do mercado
- Falta de confianca (sem depoimento, sem SSL)
- Formulario ou checkout chato
- Anuncio vendendo A, pagina entregando B

**Acoes:**
- Revisar LP com olhar frio
- Testar versao nova (outra headline, outro visual)
- Validar checkout: formas de pagamento, frete claro, politica de troca
- Garantir coerencia anuncio → LP

---

### Sintoma: Converte mas CPA acima da meta
**Causas:**
- Anuncio pega publico errado
- Ticket medio menor que esperado
- Competicao aumentou
- Meta irreal

**Acoes:**
- Rever meta (ela e realista?)
- Endurecer publico (lookalike menor)
- Testar novos angulos de anuncio
- Melhorar valor medio (upsell, kit)

---

### Sintoma: CPA bom mas volume baixo
**Causas:**
- Orcamento insuficiente
- Publico pequeno esgotando
- Horario limitado

**Acoes:**
- Aumentar orcamento +20% a cada 3 dias
- Duplicar conjunto com publico novo
- Ampliar posicionamento
- Abrir horario full-day

---

### Sintoma: Funcionava, parou de funcionar
**Causas:**
- Criativo saturou (frequencia > 3)
- Mudanca sazonal
- Concorrente novo entrou no leilao
- Mudanca de politica da plataforma
- Pixel quebrou silenciosamente

**Acoes:**
- Checar pixel (Debug Tool Meta)
- Pesquisa de Leilao (gerenciador Meta)
- Rotacionar criativos (todos)
- Investigar concorrencia (Ad Library)

---

## Passo 5 - Acao recomendada (formato padrao)

Entregue ao usuario no formato:

```
DIAGNOSTICO

Causa raiz provavel: [X]
Evidencia: [numero que sustenta]

ACAO (em ordem)

1. [acao mais barata/rapida primeiro]
2. [segunda]
3. [terceira]

O QUE NAO FAZER

- [mudanca que o usuario quer fazer mas vai piorar]

METRICA DE SUCESSO

Esperar: [X por Y dias]. Se nao mexer em [indicador], reavaliar.

PROXIMA CHECAGEM

[dia e hora]
```

---

## Checklist completo de campanha saudavel (usa para auditoria rapida)

### Setup
- [ ] Pixel + CAPI funcionando, Purchase com valor
- [ ] 7 eventos priorizados configurados
- [ ] Dominio verificado
- [ ] BM verificada + 2FA em todos admins
- [ ] Nomenclatura Subido aplicada

### Estrutura
- [ ] Objetivo correto para o resultado buscado
- [ ] Estrutura enxuta (1-3 conjuntos por campanha, raramente mais)
- [ ] Hierarquia de publicos com exclusao
- [ ] Retargeting ativo
- [ ] Minimo 6 anuncios por conjunto

### Criativo
- [ ] 50% estatico + 50% video (Meta)
- [ ] UGC presente
- [ ] Formato nativo por plataforma
- [ ] Legenda embutida
- [ ] CTA claro
- [ ] Rotacao: > 1 anuncio novo por semana

### Rotina
- [ ] Planilha de metricas atualizada diariamente
- [ ] Otimizacoes documentadas
- [ ] Reuniao semanal com o dono do negocio / cliente
- [ ] Meta definida por numero (nao "melhorar")

### Contingencia
- [ ] BM secundaria existe
- [ ] Conta reserva aquecida
- [ ] Dominio alternativo cadastrado
- [ ] Politica Meta + Google lida nos ultimos 30 dias

Se menos de 70% check = prioridade e consertar setup, nao otimizar campanha.
