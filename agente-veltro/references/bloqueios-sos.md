# Bloqueios e contingencia - SOS

## Principios

1. **Prevenir > remediar.** Uma conta blindada raramente bloqueia.
2. **Nao entre em panico.** Toda rejeicao tem caminho. 80% dos bloqueios sao reversiveis.
3. **Separe o joio do trigo.** Bloqueio por politica (ignoravel/apelavel) vs por seguranca (grave).
4. **Sempre tenha backup.** Gestor profissional tem BM/conta reserva pronta.

---

## 1. BLINDAGEM DE ATIVOS (prevencao)

Antes de qualquer problema, garanta:

### Conta pessoal Facebook
- 2FA ativado (autenticacao em 2 fatores)
- E-mail unico e exclusivo para marketing
- Nome completo real + foto real
- Celular confirmado
- Historico organico de uso (nao e perfil criado ontem)

### Business Manager (BM)
- Verificacao de negocio feita (documento da empresa + comprovante de endereco)
- 2 admins diferentes (se um cair, outro mantem)
- Papeis bem definidos (nao e todo mundo admin)
- Paginas + contas de anuncios + pixel dentro da BM, NUNCA em conta pessoal

### Conta de anuncios
- Criada dentro da BM verificada
- Limite de gasto configurado (previne fraude se cair em maos erradas)
- Cartao unico por conta
- Notificacoes ativas

### Gerenciamento de acesso
- Cliente concede acesso a BM via "Parceiros" (nao ao seu pessoal)
- Nunca pedir login/senha do cliente
- Sair do pc do cliente depois de acesso

---

## 2. VOCE ESTA SENDO RASTREADO

Meta e Google rastreiam:
- IP
- Device fingerprint (hardware + browser + plugins)
- Cookies
- Comportamento (horario de login, cliques, velocidade)
- Pagamento (cartao, CPF)
- Dominio do site anunciado
- Relacao entre contas (se voce ja foi banido com o mesmo CPF/email/cartao, cai tudo novo).

**Regra:** se voce foi banido em 1 conta, nao use nada comum (mesmo pc, mesmo cartao, mesma rede) na proxima sem multilogin.

---

## 3. TIPOS DE BLOQUEIO

### A. Anuncio reprovado
- **Grave?** Nao (quase sempre).
- **O que e:** Meta/Google viram que 1 anuncio fere politica.
- **Acao:** revisar politica citada. Editar anuncio. Se certeza que nao fere, pedir revisao.
- **Exemplos:** frase "voce esta gordo?" (atributo pessoal), "ganhe R$ 10k em 30 dias" (promessa financeira), produto restrito.

### B. Contas de anuncio desativada
- **Grave?** Medio.
- **O que e:** conta de anuncios especifica foi parada.
- **Acao:** recorrer via "Qualidade da conta" no gerenciador. Upload de documento. Aguardar 24-72h.
- **Causa comum:** metodo de pagamento falhou, anuncio reprovado muitas vezes, spike de gasto suspeito.

### C. Perfil pessoal desativado
- **Grave?** Grave.
- **O que e:** seu Facebook pessoal caiu.
- **Acao:** recurso via ajuda.facebook.com com documento. Se nao voltar, toda BM linkada cai.
- **Prevencao:** 2FA + historico de uso organico.

### D. BM desativada
- **Grave?** Muito grave.
- **O que e:** BM inteira parada. Todas contas dentro caem junto.
- **Acao:** recurso com documento da empresa. Pode levar dias ou nao voltar.
- **Prevencao:** verificacao de negocio feita, 2 admins.

### E. Dominio bloqueado
- **Grave?** Moderado.
- **O que e:** Meta marcou seu dominio (site) como suspeito. Nao deixa mais anunciar.
- **Acao:** recurso pelo gerenciador de dominios. Revisar landing page (politica).
- **Causa comum:** muito redirect, dominio muito novo, conteudo que viola politica.

### F. Pixel / pagina / ad account com aviso
- **Grave?** Baixo a medio.
- Ajustar o que esta flaggado, seguir.

---

## 4. IDENTIFICANDO REJEICOES

Ao receber notificacao, sempre:

1. Ler a politica citada (clicar no link da Meta).
2. Comparar com o anuncio.
3. Se violacao obvia: corrigir e subir de novo.
4. Se nao entender: pedir revisao via chat de suporte.
5. Registrar em planilha (data, campanha, politica, acao).

**Rejeicoes comuns (Meta):**
- Atributos pessoais ("voce esta...")
- Promessa financeira irreal
- Saude, emagrecimento, suplemento sem registro
- Imagem antes/depois
- Linguagem agressiva ou de medo

**Rejeicoes comuns (Google):**
- Destino incomum (redirect duplo, URL muito nova)
- Concorrente mencionado
- Politica de promocao nao cumprida
- Site fora do ar na aprovacao

---

## 5. FUI BLOQUEADO E AGORA?

### Protocolo em 5 passos

1. **Respirar.** Nao tome decisao no 1o minuto.
2. **Screenshot de tudo** (email, aviso, politica citada).
3. **Tentar recorrer** pela ferramenta oficial (Qualidade da conta).
4. **Aguardar 24-72h** sem mexer em nada.
5. **Se nao voltar:** acionar ativo de backup (ver abaixo).

### NAO fazer (vai piorar)
- Tentar criar conta nova com mesmo cartao/CPF/device.
- Apelar muitas vezes em sequencia.
- Xingar no chat de suporte.
- Rodar conteudo ainda mais agressivo.

---

## 6. ESTRATEGIAS PCB (Plano Contingencia Bloqueio)

Sigla: Prevenir, Contingenciar, Blindar.

Para trabalhar em serio, tenha:

### Ativos principais (uso diario)
- 1 perfil Facebook pessoal bem conservado
- 1 BM verificada
- 1-2 contas de anuncio
- 1 pagina com historico organico
- 1 pixel maduro
- 1 dominio .com.br com HTTPS

### Ativos de backup (guardados)
- 1 perfil Facebook secundario (com historico real, nao fake)
- 1 BM secundaria em CNPJ diferente
- 1 conta de anuncios reserva pronta
- 1 dominio alternativo (subdominio ou .com adicional)
- Cartao de credito diferente
- Device alternativo (Multilogin, anti-detect browser)

### Regras dos backups
- NUNCA use com mesmo IP da principal.
- NUNCA use com mesmo cartao.
- NUNCA conecte via mesmo Facebook pessoal.
- Aqueca o ativo de backup antes (3-7 dias de uso organico).

---

## 7. FERRAMENTAS DE CONTINGENCIA

- **Multilogin / AdsPower / GoLogin** - navegadores anti-detect, cada conta em fingerprint separado.
- **Proxy 4G residencial** - IP brasileiro, nao datacenter.
- **VPN dedicada** - so se for IP unico de longo prazo. Nunca compartilhado.
- **Gestor de password** - 1Password/Bitwarden para nao misturar login.

---

## 8. NICHOS SENSIVEIS (precisam de cuidado extra)

Meta e Google sao rigorosos com:
- Emagrecimento / dieta / suplemento
- Apostas / criptomoeda
- Renda extra / ganhar dinheiro online
- Servicos financeiros (emprestimo, cartao)
- CBD / canabidiol
- Adulto (qualquer coisa sensual)
- Armas / produtos relacionados
- Politica
- Namoro / relacionamento

**Como operar em nicho sensivel:**
- Linguagem suave (nunca "emagreca 10kg em 30 dias")
- Destino sem promessa explicita
- Conta dedicada (nao misture com outros projetos)
- Multiplos ativos de backup
- Revisar politica cada atualizacao Meta

---

## 9. CONCLUSAO (mentalidade)

Bloqueio nao e "se", e "quando". Gestor profissional:
- Nao concentra tudo em 1 BM.
- Tem rotina de backup semanal.
- Documenta cada bloqueio que viveu (vira conhecimento).
- Respeita politica antes de tentar burlar.
- Educa o cliente: "bloqueio pode acontecer. Por isso temos redundancia."

---

## Template de resposta SOS

Quando o usuario disser "minha conta foi bloqueada", responda com:

```
SOS Bloqueio - Triagem rapida

1. O que bloqueou? (anuncio / conta de anuncio / perfil pessoal / BM / dominio / pagina)
2. Qual a politica citada no aviso?
3. Primeira vez ou recorrente?
4. Tem backup (BM, conta, dominio) pronto?

Enquanto voce responde, veja:
- Qualidade da conta (gerenciador Meta)
- Central de recursos Google Ads
- Screenshot do email de aviso

Nao mexa na conta principal por 24h. Nao apele mais de 1x. Aguarde minha orientacao com suas respostas.
```
