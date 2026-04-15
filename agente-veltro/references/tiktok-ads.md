# TikTok Ads - Playbook operacional

## Logica da plataforma

TikTok NAO e Meta. Erros comuns:
- Subir o mesmo video do Reels achando que funciona igual.
- Priorizar "look ad-style" quando o usuario consome UGC nativo.
- Segmentar demais em vez de deixar o algoritmo achar.

**Regra TikTok:** criativo vence 80% do jogo. 20% restantes = objetivo + ICP. Segmentacao tem peso muito menor que no Meta.

---

## Criativos: o 80/20

Se o usuario so tiver energia para uma coisa: **volume de criativos UGC verticais (9:16) de 15-30 segundos**.

### Estrutura do video TikTok Ads

1. **Hook nos primeiros 1-3 segundos** - algo quebra padrao, movimento, pergunta direta, numero.
2. **Corpo 4-20s** - entrega o valor/prova/demo em linguagem nativa (sem cara de comercial).
3. **CTA 20-30s** - "clica no botao amarelo / link na bio / comprar agora".

### Padrao que funciona

- Filmado em celular.
- Legenda embutida (quase todo mundo assiste sem som).
- Texto sobreposto chamando atencao nos primeiros segundos.
- Musica em tendencia (TikTok Creative Center → sons em alta).
- UGC com criador de conteudo proximo do ICP.

### Formatos ruins

- Video horizontal cortado.
- Logo grande + texto corporativo.
- Abertura com "ola, meu nome e..." (mata o hook).
- Video com mais de 40s sem gancho forte.

---

## Objetivos de campanha

| Objetivo | Use quando |
|---|---|
| Vendas (conversao site) | Tem pixel + conversoes regulares |
| Geracao de cadastros (lead) | Formulario instantaneo / site |
| Trafego | Aquecer / baixo funil |
| Alcance | Topo de funil, lancamento |
| Visualizacoes de video | Distribuicao de conteudo / aquecimento |
| Reconhecimento | Branding novo mercado |

**Regra:** Smart+ Campaigns (similar ao Advantage+ da Meta) funciona bem. Se a conta e nova, use-a.

---

## Segmentacao

### 3 abordagens, em ordem de prioridade

1. **Totalmente aberta (broad)** - so pais + idade + genero. Deixa TikTok achar.
2. **Interesses amplos** - adicione 3-5 categorias relacionadas. Evite cortar demais.
3. **Publicos personalizados** - pixel 30d, lista de clientes, LLA 1-5%.

**Nunca empilhe:** interesse + comportamento + demo detalhado. O algoritmo trava.

---

## Pixel TikTok

Equivalente ao pixel Meta.

Eventos essenciais: `ViewContent`, `AddToCart`, `InitiateCheckout`, `Purchase`, `SubmitForm`.

Instale via:
1. Shopify / Nuvemshop / parceiros (nativo)
2. Google Tag Manager
3. Manual

**Ative Events API (server-side)** sempre que possivel.

---

## Orcamento e lance

- Minimo recomendado por conjunto: R$ 20-30/dia (se for menor, sem aprendizado).
- Estrategia: **Menor custo** no comeco. Troque para lance maximo so depois de 100+ conversoes.
- CBO (Campaign Budget Optimization) ativa = similar ao Meta CBO.

---

## Spark Ads (use sempre que possivel)

Spark Ad = impulsionar post organico existente como anuncio.

Vantagens:
- Likes/comentarios/views do video organico aparecem no anuncio → prova social.
- Usuario pode clicar no perfil → cresce seguidor.
- CPM geralmente menor.

**Regra:** se o cliente tem perfil organico, SEMPRE ofereca Spark Ad como prioridade 1 antes de criar anuncio do zero.

---

## Checklist para subir TikTok Ads do zero

1. Pixel instalado + Events API.
2. 6+ criativos UGC 9:16 de 15-30s.
3. Objetivo alinhado com estagio do funil.
4. 1 campanha, 1-2 conjuntos, segmentacao aberta.
5. Orcamento minimo R$ 30/dia por conjunto.
6. Horario full-day (nao corte horario no inicio).
7. Deixar rodar 72h antes de julgar.

---

## Metricas TikTok (benchmarks BR)

| Metrica | Bom | Alerta |
|---|---|---|
| CPM | R$ 5-15 | > R$ 25 |
| CTR | > 1% | < 0.5% |
| CPC | R$ 0,50-2 | > R$ 4 |
| Hook rate (3s) | > 30% | < 15% |
| Completion rate | > 10% | < 3% |
| ROAS e-com | > 2 | < 1 |

**Hook rate baixo** = criativo ruim nos primeiros 3s. Troque.
