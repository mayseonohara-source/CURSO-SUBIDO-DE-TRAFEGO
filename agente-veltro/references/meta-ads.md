# Meta Ads - Playbook operacional

Facebook + Instagram + Messenger + WhatsApp via gerenciador de anuncios da Meta.

## Estrutura: sempre Campanha > Conjunto > Anuncio

| Nivel | Responde | Decisoes |
|---|---|---|
| Campanha | "Por que vou anunciar?" | Objetivo, orcamento (CBO), estrategia de lance |
| Conjunto | "Para quem / onde vou aparecer?" | Publico, posicionamentos, orcamento (ABO), janela de conversao |
| Anuncio | "O que vou mostrar?" | Criativo, copy, CTA, destino (site/WhatsApp/form) |

**Regra de volume:** conjunto com menos de 6 anuncios ativos = estrutura fraca. Padrao = 6.

---

## Nomenclatura Subido (obrigatoria)

- **Campanha:** `[OBJETIVO] [PUBLICO F/M/Q] [POSICIONAMENTO] [TAG] Descricao`
  - Ex.: `[CONVERSAO] [F] [STORIES] [BF2025] Video convite`
- **Conjunto:** `NN - [AUTO/MANUAL] - [Nome do publico]`
  - Ex.: `01 - [FEED] Envolvimento IG 14D`
- **Anuncio:** `ADNN - Descricao identificavel`
  - Ex.: `AD01 - Convite de cabeca para baixo`

Nomenclatura limpa = filtros rapidos = decisao mais rapida = ROI.

---

## Objetivos de campanha (e quando usar)

| Objetivo | Use quando |
|---|---|
| Vendas (conversao) | Tem pixel + pelo menos 50 conversoes/semana esperadas |
| Leads | Captura via formulario instantaneo ou site |
| Trafego | Quer enviar gente pro site, mas nao tem pixel maduro ainda |
| Engajamento / Mensagens | B2B local, servico por WhatsApp, recem-aberto |
| Reconhecimento | Branding, topo de funil, produto novo no mercado |
| Reproducao de video | Aquecer audiencia antes de vender (distribuicao de conteudo) |

**Regra de ouro:** escolha o objetivo que entrega o resultado final, nao o intermediario. Quer venda? Use Vendas. Nao use Trafego achando que "economiza".

---

## Os 4 tipos de orcamento

1. **CBO (Advantage Campaign Budget)** - orcamento na campanha, Meta distribui entre conjuntos. Default moderno.
2. **ABO (Ad Set Budget)** - orcamento no conjunto. Use para forcar gasto em publico especifico.
3. **Diario** - Meta gasta ate X por dia, media dentro de 7 dias.
4. **Vitalicio** - Meta gasta X no periodo total (bom para datas com fim).

**Recomendacao padrao:** comece com **CBO + diario**. Troque para ABO se precisar isolar teste de publico.

---

## Estrategias de lance

- **Menor custo (sem limite)** - default. Meta gasta tudo buscando menor CPA possivel. Use no aprendizado.
- **Limite de custo** - define CPA maximo. Use quando ja conhece o CPA historico e quer proteger margem.
- **ROAS minimo** - define retorno minimo por real. Use em e-commerce maduro.
- **Limite de lance** - avancado, define lance maximo no leilao. Raramente recomendado.

**Regra:** comece em **menor custo** por 7-14 dias. So mude para limite quando tiver 100+ conversoes de historico.

---

## Segmentacao: as 5 maneiras

1. **Publico salvo** (interesse + demo + comportamento) - bom para publico frio inicial.
2. **Publico personalizado** - baseado em lista (CRM, pixel, engajamento). Publico quente e superquente.
3. **Publico semelhante (lookalike)** - 1% a 10% de gente parecida com base. Use 1-3% para prospecting top.
4. **Publico aberto** (advantage+) - so pais + idade. Deixa Meta achar. Cresceu em 2024-2025.
5. **Publico broad + detalhado como sugestao** - abertura + indicacao leve de interesse.

**Hierarquia de publicos (exclusao obrigatoria):**
- Superquente (compradores 30d) → excluir de
- Quente (visitantes 30d, engajou 30d) → excluir de
- Frio (LLA + aberto + interesse)

Sem exclusao = concorrencia entre seus proprios conjuntos = CPA inflado.

---

## Recursos Advantage

Meta empurra automacao. O agente recomenda por default:

| Recurso | Ativar? |
|---|---|
| Advantage+ publico | SIM em prospecting frio + campanha com boa base |
| Advantage+ posicionamentos | SIM (quase sempre) |
| Advantage+ criativos (expansoes) | DEPENDE. Ative no teste, desligue em escala estavel |
| Campanha Advantage+ Shopping (ASC) | SIM em e-commerce com catalogo |

---

## Posicionamentos principais (e o que funciona)

- **Feed Instagram/Facebook** - estatico e video. Ainda dominante em conversao.
- **Stories** - vertical 9:16. Bom para aquecimento + conversao com video curto.
- **Reels** - vertical, formato UGC vence. Barato e escala.
- **Messenger** - cai em desuso.
- **Audience Network** - fora dos apps Meta. Bom para alcance barato, ruim para conversao.
- **Marketplace** - misto, varia muito por nicho.

**Default inicial:** Advantage+ posicionamentos. Refine so depois de ter dado.

---

## Fase de aprendizado

- Conjunto entra em "Aprendizado" ao criar ou ao sofrer edicao significativa.
- Sai do aprendizado com **50 eventos de otimizacao em 7 dias** (ou 7 dias sem editar).
- **Durante o aprendizado:** NAO otimize. CPA 20-40% acima do alvo e normal.
- **Edicao significativa que reinicia aprendizado:** mudanca de publico, orcamento > 20%, objetivo, posicionamento, lance, anuncio novo em > 50% do total.

**Regra:** editou algo grande = paciencia. 72h minimo antes de julgar.

---

## Pixel + API de conversoes (obrigatorio)

- **Pixel** = tag JS no site, traqueia eventos (PageView, ViewContent, AddToCart, InitiateCheckout, Purchase, Lead).
- **API de conversoes (CAPI)** = envio server-to-server dos mesmos eventos. Dobra qualidade do sinal pos iOS14.
- **Instalar pelos metodos:**
  1. Google Tag Manager (recomendado - controle maximo)
  2. Parceiros (Shopify, WooCommerce, Nuvemshop, Hotmart - nativo)
  3. Manual (desenvolvedor)
  4. E-mail para desenvolvedor (ultimo recurso)

**Checklist do pixel saudavel:**
- [ ] Pixel base em todas as paginas
- [ ] Evento Purchase disparando com valor dinamico
- [ ] API de conversoes ligada (event_id igual em browser + server = deduplicacao)
- [ ] Qualidade do evento no Gerenciador > 7.0
- [ ] 7 eventos priorizados configurados no Conjunto de Dados

---

## Checklist para subir uma campanha Meta do zero

1. ICP definido (documento)
2. Pixel + CAPI validados (Purchase disparando)
3. 7 eventos priorizados configurados
4. Publicos criados: 1% LLA, 3% LLA, compradores (excluir), site 30d (retargeting)
5. Criativos: minimo 6 por conjunto (3 estaticos + 3 video)
6. Estrutura: 1 CBO Vendas, 3 conjuntos (frio Advantage+, LLA 1-3%, retargeting 30d)
7. Orcamento: R$ 50-150/dia inicial (depende do ticket)
8. Nomenclatura aplicada
9. Janela de conversao: 7 dias clique / 1 dia visualizacao (default)
10. Ligar e nao mexer por 72h

---

## Erros mais comuns (e como voce alerta)

- Trocar criativo/orcamento todo dia → reseta aprendizado.
- Publico < 1 milhao em frio → Meta nao otimiza bem.
- Rodar campanha de vendas sem 50 conversoes/semana → troca para Leads ou agrega conjuntos.
- Copiar campanha velha sem revisar nomenclatura → bagunca relatorio.
- Nao excluir compradores do prospecting → inflate CPA.
