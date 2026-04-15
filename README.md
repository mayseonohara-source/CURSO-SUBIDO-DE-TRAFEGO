# CURSO SUBIDO DE TRAFEGO

Base de conhecimento estruturada do **Curso Subido de Trafego** (Comunidade Subido de Trafego - Pedro Sobral).

Este repositorio contem transcricoes, resumos e questoes-chave extraidas de cada aula, organizadas por modulo. O objetivo e servir como base para criacao de um **agente de IA especializado em trafego pago**.

---

## Estrutura do Curso

O curso possui **10 modulos** com 89 aulas teoricas + ABCs (tutoriais praticos):

| # | Modulo | Aulas | Descricao |
|---|--------|-------|-----------|
| 01 | Introducao ao Trafego Pago | 2 | Alinhamento de expectativas, estrutura do curso |
| 02 | O Metodo Subido de Trafego | 13 | 12 principios do metodo + conteudo base |
| 03 | Meta Ads | 11+ABC | Campanhas Facebook/Instagram |
| 04 | Google Ads | 13+ABC | Campanhas Google (Search, Display, YouTube, Pmax) |
| 05 | Otimizacao de Campanhas | 14 | Como otimizar lances, segmentacoes, criativos, etc |
| 06 | Estrategias de Trafego Pago | 13 | Planejamento para e-commerce, fisico, infoprodutos |
| 07 | TikTok Ads | 4+ABC | Campanhas no TikTok |
| 08 | LinkedIn Ads | 4+ABC | Campanhas no LinkedIn |
| 09 | Bloqueios e Contingencias | 13+ABC | Preveni/resolver bloqueios de conta |
| 10 | SOS Trafego Pago | 2+ABC | Conhecimento basico para subir campanhas rapido |

---

## Estrutura do Repositorio

```
CURSO-SUBIDO-DE-TRAFEGO/
├── README.md
├── indice-completo-curso.txt       # Indice completo com todas as aulas
├── modulo-01-introducao-ao-trafego-pago/
│   ├── aula-01-como-esse-curso-vai-funcionar.md
│   └── aula-02-como-ganhar-dinheiro-com-esse-curso.md
├── modulo-02-o-metodo-subido-de-trafego/
│   └── aula-XX-*.md (13 aulas)
├── modulo-03-meta-ads/
│   └── aula-XX-*.md (11 aulas)
├── ... (mesma estrutura para modulos 4-10)
├── pdfs/                           # PDFs originais do material de apoio
│   ├── m01/ m02/ ... m10/
└── pdf-texts/                      # Textos extraidos dos PDFs
    ├── m01/ m02/ ... m10/
```

---

## Formato dos Arquivos

Cada arquivo de aula (`.md`) contem:

- **Titulo e duracao** da aula
- **Conteudo do PDF de material de apoio** (quando disponivel)
- **Questoes-chave** extraidas ou sugeridas para estudo

Aulas sem PDF disponivel (nao publicado ainda ou apenas video) tem um template com questoes a investigar durante o estudo.

---

## 3 Tipos de Conteudo do Curso

1. **Aulas** - Explicacao de conceitos complexos de forma simples
2. **AI.LAS** - IAs criadas e treinadas de acordo com cada aula
3. **ABC** - Tutoriais praticos (apertando os botoes)

---

## Conceitos-Chave do Metodo Subido

### Teoria dos 8 Pontos de Contato
O conhecimento de trafego pago e construido em camadas atraves de 8 pontos de contato:
1. Aula  
2. AI.LA  
3. ABC  
4. Explorar gerenciador  
5. Subir campanha  
6. Pesquisar  
7. Perguntar na comunidade  
8. Contribuir na comunidade

### 5 Habilidades do Anunciante Profissional
1. Organizacao  
2. Curiosidade  
3. Processos e Padroes  
4. Cara de pau  
5. Comunicacao

### Rotina de Sucesso - 3 Fatores
1. **Quando** estudar  
2. **Onde** estudar  
3. **Quanto tempo** estudar

### 2 Caminhos para Ganhar Dinheiro
1. **Gestor de Trafego** - vende o servico para outros negocios
2. **Dono do Negocio** - anuncia para o proprio negocio

---

## Dados de Performance (Pesquisa com 5.000 alunos)

| Condicao | Faturamento SIM | Faturamento NAO |
|---|---|---|
| Rotina clara para estudar trafego pago | R$ 6.360,74 | R$ 4.060,57 |
| Rotina clara de prospeccao de clientes | R$ 9.246,62 | R$ 4.145,58 |
| Viu todas as aulas do curso | R$ 8.723,36 | R$ 3.753,72 |
| Certificacao Meta Ads | R$ 10.987,24 | R$ 3.515,14 |
| Certificacao Google Ads | R$ 15.149,87 | R$ 4.062,10 |

**Conclusao:** Assistir as aulas + EXECUTAR o conhecimento = resultado financeiro superior.

---

## Como Usar Este Repositorio

### Para Estudo
1. Siga os modulos em ordem (1 -> 10)
2. Para cada aula, leia o arquivo `.md` correspondente
3. Assista a aula em video no Universo Subido
4. Responda as "Questoes Mais Importantes" ao final
5. Coloque a mao na massa (ABC + gerenciador de anuncios)

### Para Criar um Agente de IA
Este repositorio serve como **base de conhecimento estruturada** para:
- Fine-tuning de modelos LLM especializados em trafego pago
- RAG (Retrieval-Augmented Generation) com contexto especifico
- Criacao de chatbots que respondem duvidas sobre campanhas
- Sistemas de automacao de otimizacao com base no metodo Subido

---

## Objetivo Final

Criar um **agente de IA especializado em trafego pago** baseado no Metodo Subido de Pedro Sobral, capaz de:
- Responder duvidas sobre Meta, Google, TikTok e LinkedIn Ads
- Sugerir estrategias de otimizacao de campanhas
- Orientar no planejamento de campanhas para diferentes nichos
- Auxiliar em situacoes de bloqueio e contingencia

---

## Agente Veltro (implementado)

A sintese proprietaria do conhecimento das 89 aulas foi destilada em uma skill do Claude Agent SDK pronta para plugar no **Veltro** (gestor de trafego).

Localizacao: [`agente-veltro/`](agente-veltro/)

**4 papeis que o agente assume:**
1. Consultor estrategico (planejamento, estrutura, canal, verba)
2. Otimizador de campanhas (diagnostico + 6 alavancas)
3. Criador de criativos (8 tipos de gancho, VSL, templates)
4. SOS bloqueios (blindagem + contingencia PCB)

**Estrutura:**
- `agente-veltro/SKILL.md` - identidade, principios, fluxo de atendimento, 8 comandos
- `agente-veltro/README.md` - como plugar no Veltro (3 opcoes: system prompt / SDK / RAG)
- `agente-veltro/references/` - 11 arquivos de conhecimento por dominio (metodo, Meta, Google, TikTok, LinkedIn, criativos, metricas, otimizacao, estrategia, bloqueios, diagnostico)

**Comandos do agente:**
`/plano`, `/anuncio`, `/otimizar`, `/icp`, `/sos`, `/nomenclatura`, `/metricas`, `/escala`

---

## Credito e Direitos

Todo o conteudo deste repositorio e baseado no curso oficial da **Comunidade Subido de Trafego** por **Pedro Sobral**. Uso pessoal e de estudo apenas.

Acesso ao curso: https://www.subido.com.br

---

## Status do Projeto

- [x] Modulo 01 - 2/2 aulas processadas
- [x] Modulo 02 - 13/13 aulas processadas (12 PDFs + 1 sem PDF)
- [x] Modulo 03 - 11/11 aulas processadas (10 PDFs + 1 sem PDF)
- [x] Modulo 04 - 13/13 aulas processadas (10 PDFs + 3 sem PDF)
- [x] Modulo 05 - 14/14 aulas processadas (12 PDFs + 2 sem PDF)
- [x] Modulo 06 - 13/13 aulas processadas (4 PDFs + 9 sem PDF)
- [x] Modulo 07 - 4/4 aulas processadas (sem PDFs)
- [x] Modulo 08 - 4/4 aulas processadas (3 PDFs + 1 sem PDF)
- [x] Modulo 09 - 13/13 aulas processadas (4 PDFs + 9 sem PDF)
- [x] Modulo 10 - 2/2 aulas processadas (2 PDFs)

**Total: 89/89 aulas teoricas processadas | 59 PDFs de apoio baixados**
