---
name: enp-instagram-content
description: >
  Skill de criação de conteúdo para Instagram do Ecommerce na Prática. Use sempre que a tarefa
  envolver produção, revisão ou estruturação de qualquer formato de Instagram da marca — Stories,
  Feed estático, Carrossel, Reels ou roteiro de Live. Aciona também quando o pedido mencionar
  "post no Insta", "story", "carrossel", "reel", "roteiro de live", "legenda", "criativo",
  "conteúdo de Instagram", "collab", "colaboração com parceiro" ou qualquer variação. Inclui
  briefing obrigatório de formato e parceria, calibração por ICP (Iniciantes/ICP5, Digital
  Natives/ICP2, Escala/ICP1), especificações de design e dimensão por formato, e tom 60% Mentor
  + 40% Sábio da marca. Em conteúdos de collab, lê em tempo real a planilha oficial de Parceiros
  no Google Drive para identificar benefícios ativos para a base e integrá-los ao copy. Não use
  para e-mail (use enp-email-marketing) nem para outras redes.
---

# Skill: Conteúdo para Instagram — Ecommerce na Prática

**Versão:** 1.2 | **Base:** Brand Book + Tom de Voz EnP v3.0 + skill de e-mail marketing v1.1

> **Autocontida.** Esta skill traz todos os arquivos de referência que precisa dentro de `references/`. Não depende de knowledge base externa nem de preferências de usuário. Funciona igual em qualquer Claude que tenha a skill instalada.
>
> **Exceção em tempo real:** quando o conteúdo for collab com parceiro, a skill instrui o Claude a ler a planilha oficial de Parceiros via Google Drive (ver seção 7.0). Isso garante que benefícios e cupons estejam sempre atualizados. Requer conexão Google Drive ativa no Claude de quem está usando.

---

## 0. Briefing obrigatório — perguntar SEMPRE antes de criar

Nunca começar a produzir conteúdo de Instagram sem passar pelo briefing abaixo. As respostas determinam formato, dimensão, tom, estrutura e CTA. Se a pessoa não souber alguma resposta, sugira a mais provável com base no contexto e peça validação.

**Use a ferramenta `ask_user_input_v0` para fazer o briefing sempre que possível** — é mais rápido para a Ana Clara responder no celular do que digitar.

---

### 0.1 Perguntas de briefing (fazer todas, nesta ordem)

**1. Qual é o formato (ou formatos) desejado?**
- [ ] Stories (sequência de telas verticais)
- [ ] Feed estático (post único)
- [ ] Carrossel (2 a 10 cards)
- [ ] Reels (vídeo curto)
- [ ] Roteiro de Live

> Se for mais de um formato, produzir um por vez seguindo o padrão de cada um. Não misturar copy de carrossel com legenda de feed estático — são lógicas diferentes.

**2. É colaboração com parceiro?**
- [ ] Não, é conteúdo orgânico próprio
- [ ] Sim, é collab

> **Se sim, antes de qualquer outra pergunta:**
>
> 1. **Leia a planilha oficial de Parceiros do Ecommerce na Prática** via Google Drive:
>    - URL: https://docs.google.com/spreadsheets/d/1ZUQpEBAaNLo4_sbiqBGxUOm4orJJubWUeN7n_V5-24U/edit
>    - File ID: `1ZUQpEBAaNLo4_sbiqBGxUOm4orJJubWUeN7n_V5-24U`
>    - Use a tool `Google Drive:read_file_content` com o File ID acima.
> 2. **Pergunte ao solicitante: "Qual é o parceiro?"**
> 3. **Cruze a resposta com a planilha:**
>    - Se o parceiro **estiver na planilha**: trazer para o briefing o conteúdo das colunas "O que faz?", "Benefício da parceria EnP" e "Link/Cupom" referentes àquele parceiro. Esses dados vão modular o copy (especialmente o CTA, que pode incluir o benefício específico — desconto, cupom, freemium, etc.).
>    - Se o parceiro **não estiver na planilha**: avisar o solicitante que o parceiro não está cadastrado e perguntar se há benefício ativo a ser comunicado, ou se é uma collab pontual sem benefício para a base.
>    - Se a planilha **não puder ser lida** (sem acesso, erro de quota, etc.): avisar o solicitante e seguir o fluxo normal de collab sem cruzamento, perguntando manualmente se há benefício ativo.
> 4. **Continuar com o briefing de collab** (perguntas em sequência abaixo):
>    - Nome do parceiro e @ no Instagram
>    - O que o parceiro faz (área, autoridade, contexto) — pode vir pré-preenchido pela planilha; pedir validação
>    - É colab paga, troca, parceiro estratégico ou parceiro de conteúdo?
>    - Quem é o público "dono" do conteúdo? (nosso público, do parceiro, ou ambos)
>    - Tem CTA cruzado para o perfil do parceiro? Onde?

Ver seção 7 para regras de collab e como integrar o benefício do parceiro no copy.

**3. Qual é o objetivo deste conteúdo?**
Um conteúdo = uma ação. Se houver mais de um objetivo, são posts separados.
- Opções comuns: gerar autoridade / educar sobre dor específica / divulgar produto / divulgar evento (live, webinar, lançamento) / converter para checkout / engajar (comentário, compartilhamento, save) / reativar seguidor inativo / mostrar bastidor

**4. Qual produto está em jogo (se houver)?**
- [ ] Assinatura (R$497/ano)
- [ ] Implementação de Loja Virtual (R$897)
- [ ] Consultoria 12 semanas (R$6.870)
- [ ] Nenhum — conteúdo de autoridade, educação, bastidor ou evento

A abordagem muda completamente por produto. Ver seção 0.3.

**5. Para qual ICP?**
- [ ] ICP 5 — Iniciantes (não vendem ainda, ~59% da base)
- [ ] ICP 2 — Digital Natives (vendem até R$5k, dependência de Instagram, ~27%)
- [ ] ICP 1 — Migração/Escala (faturam R$20k+, ~10%)
- [ ] ICP 4 — Baixa Maturidade (marketplace, ~4%)
- [ ] Misto — segmentar copy ou priorizar ICP majoritário

Se não houver definição, sugerir o ICP mais representativo para o objetivo e pedir validação.

**6. Tem CTA explícito ou é conteúdo de autoridade puro?**
- [ ] CTA para checkout (link na bio / sticker / arrasta pra cima)
- [ ] CTA para conteúdo (save, comentário, compartilhamento)
- [ ] CTA para perfil do parceiro (em collab)
- [ ] Sem CTA — conteúdo de marca / autoridade

---

### 0.2 Decisão de formato quando não há direcionamento

Se a pessoa pedir "um post" sem especificar formato, usar esta lógica para sugerir:

| Objetivo | Formato sugerido | Por quê |
|---|---|---|
| Educar sobre dor / conceito | Carrossel | Profundidade + save + leitura sequencial |
| Mostrar resultado de aluno (case) | Reels ou Carrossel | Vídeo gera prova social mais forte; carrossel se houver muitos dados |
| Engajamento rápido / opinião | Feed estático ou Story | Frase forte + design impactante |
| Bastidor, rotina, "dia a dia" | Story ou Reels | Formato que naturalmente humaniza |
| Lançamento de produto / evento | Reels (anúncio) + Stories (lembrete) + Carrossel (detalhes) | Combinação cobre alcance, lembrete e profundidade |
| Quebrar objeção comum (preço, tempo, dúvida) | Carrossel | Permite construir argumento completo |
| Notícia de mercado / dado novo | Reels curto ou Feed estático | Velocidade > profundidade |
| Live anunciada | Story (countdown) + Reels (chamada) + Feed (cobertura completa) | Cobertura full-funnel |

---

### 0.3 Referências por produto (resumo operacional)

**Assinatura — R$497/ano**
- Parcelado: 12x R$49,37 | 2x R$248,50 | âncora: menos de R$1,65/dia
- Para quem: ICP 2, 4, 5
- Argumento central: método para cada fase, sem adivinhar o próximo passo
- Link de checkout: `https://seguro.ecommercenapratica.com/pay/perpetuo-497`

**Implementação de Loja Virtual — R$897**
- Parcelado: 12x R$89,10 | 3x R$299
- Para quem: ICP 2, 4 com produto definido; ICP 1 migrando de plataforma
- **Não indicar para ICP 5 puro** (precisa ter produto)
- Entregável: loja Nuvemshop pronta em 10 dias úteis
- Lojas-prova: Mari Morena, Zenfit, Cookie Dreams, Bishopet, Stril Brand, Julie Semijoias

**Consultoria 12 semanas — R$6.870** (de R$10.000+)
- Parcelado: 12x R$572,50
- Para quem: ICP 1 — fatura R$20k+/mês
- **Não indicar para iniciantes**
- CTA padrão: "Agendar conversa com a equipe" (qualificação, não compra direta)
- Cases: Belarosa Plus Size (+75% conversão, R$78k/mês), DHPro (R$232k/mês), Inspira Decore (R$211k/mês), Efflore (+38% faturamento)

---

## 1. Identidade da marca (resumo operacional)

**O Ecommerce na Prática é o guia que o empreendedor precisava ter do lado desde o começo: alguém que já percorreu o caminho, não tem paciência para desculpa e sabe exatamente o próximo passo.**

- Tom: **60% Mentor (empático, mão na massa) + 40% Sábio (exigente, baseado em dados)**
- Posicionamento: **anti-guru** — sem promessas de dinheiro fácil, sem urgência falsa, sem achismo
- Nome: sempre **Ecommerce na Prática** — nunca "EnP", nunca "E-commerce na Prática" (com hífen)
- Plataforma: sempre **Nuvemshop** — nunca "nuvem shop" ou "NS"

No Instagram, a marca compete com gurus que usam estética de luxo, promessas de dinheiro fácil e urgência manipulativa. Nossa diferenciação visual e textual deve ser óbvia: design limpo, dados reais, linguagem de quem opera no dia a dia.

📄 **Para regras completas de tom de voz, ler `references/tom-de-voz.md`** (incluído nesta skill).
📄 **Para perfis de ICP e detalhes de produto, ler `references/icp-produtos.md`** (incluído nesta skill).

---

## 2. Proporção Mentor/Sábio por tipo de conteúdo

| Tipo de conteúdo | Proporção | Implicação prática |
|---|---|---|
| Conteúdo educacional (carrossel, Reels) | 60% Mentor / 40% Sábio | Ensina com dado, sem condescendência |
| Case de aluno / prova social | 65% Mentor / 35% Sábio | Acolhe a história, fecha com lição |
| Quebra de objeção | 50% Mentor / 50% Sábio | Reframe respeitoso + argumento racional |
| Lançamento / oferta | 50% Mentor / 50% Sábio | Convite firme + benefício claro |
| Bastidor / dia a dia | 75% Mentor / 25% Sábio | Humaniza, aproxima, sem perder credibilidade |
| Opinião / posicionamento de marca | 40% Mentor / 60% Sábio | Postura firme, dado na mão |
| Reativação | 65% Mentor / 35% Sábio | Reconecta sem cobrar |
| Live (anúncio) | 60% Mentor / 40% Sábio | Antecipa o que vai entregar de valor |

---

## 3. Estrutura geral de um post de alta performance no Instagram

Independente do formato, todo post da marca tem três camadas:

**Camada 1 — Hook (gancho)**
A primeira coisa que o usuário vê. Tem dois objetivos: parar o scroll e prometer valor.
- Parte de tensão, dor, paradoxo, dado ou pergunta — nunca de saudação genérica
- No carrossel é o card 1; no Reels é os primeiros 2 segundos; no Story é a primeira tela; no feed é a primeira linha da legenda + arte
- Ver seção 8 para checklist de hooks aprovados/reprovados

**Camada 2 — Desenvolvimento**
Entrega o que o hook prometeu. Aqui mora o argumento, a história, o dado, o ensinamento.
- Uma ideia central por post
- Pelo menos um dado concreto, prazo ou exemplo real
- Estrutura preferida: dor → consequência → método → prova
- Sem listas de bullet points longos — prefira texto corrido com ritmo

**Camada 3 — CTA (chamada para ação)**
Diz o que fazer agora. Único, específico, sem urgência falsa.
- "Salva esse post pra não esquecer"
- "Comenta MÉTODO que te mando o link"
- "Link na bio pra começar hoje"
- Sem "clica no link", "saiba mais", "corre porque acaba"

---

## 4. Especificações por formato — leia antes de produzir

Para cada formato existem regras específicas de **dimensão, duração, copy, estrutura e design**. Antes de produzir qualquer formato, ler o arquivo de referência correspondente:

📄 **Ler `references/formatos.md`** — contém especificações completas de:
- Stories (dimensão, duração, número de telas, stickers, tipografia)
- Feed estático (dimensão, hierarquia visual, limite de texto, áreas seguras)
- Carrossel (número de cards, dimensão, ritmo de leitura, capa e fechamento)
- Reels (dimensão, duração, estrutura cena a cena, áudio, legenda)
- Roteiro de Live (estrutura, blocos, CTA por bloco, duração média)

Sempre consulte o arquivo antes de produzir o entregável final. Não suponha medidas ou durações de memória.

---

## 5. Calibração por ICP

### ICP 5 — Iniciantes Totais (~59% da base)
- **Faturamento:** R$0 (não vendem ainda)
- **Dores:** Medo de começar errado, excesso de informação, insegurança com investimento, não sabe escolher produto
- **Produto-alvo:** Assinatura
- **Tom:** 70% Mentor — reduz ansiedade, dá clareza, celebra o primeiro passo
- **Linguagem:** Acessível. Explica termos técnicos na primeira menção. Evita jargão.
- **Ganchos que funcionam:** "começar do jeito certo", "sem perder dinheiro testando", "antes de investir um real em anúncio", "passo a passo"
- **Formatos que mais convertem:** Carrossel educacional, Reels com tutorial simples, Stories com perguntas
- **Evitar:** Dados de faturamento alto, linguagem de "escala", referências a R$50k/mês, gestão de time

**Hooks aprovados para ICP 5:**
- *"Você ainda não vendeu. E isso pode ser a melhor coisa que aconteceu com seu negócio."*
- *"Antes de investir um real em anúncio, leia isso."*
- *"3 erros que travam quem está começando do zero."*

### ICP 2 — Digital Natives (~27% da base)
- **Faturamento:** Até R$5k (às vezes até R$12k, mas com operação imatura)
- **Dores:** Vendas instáveis, dependência do Instagram, falta de processo, não consegue escalar além do orgânico
- **Produto-alvo:** Assinatura (e Implementação se já tiver produto sem loja)
- **Tom:** 60% Mentor / 40% Sábio — valida o progresso, aponta o gargalo com dado
- **Linguagem:** Pode usar termos como CAC, funil, tráfego — mas explica
- **Ganchos que funcionam:** "vender todos os dias", "parar de depender do algoritmo", "loja própria", "sair do feed e ir pro checkout"
- **Formatos que mais convertem:** Reels de opinião, Carrossel de "como sair de X para Y", Stories com bastidor de loja
- **Evitar:** Tom de iniciante total (eles já vendem), promessa de "primeiras vendas"

**Hooks aprovados para ICP 2:**
- *"Você vende pelo Instagram. E quando o algoritmo mudar?"*
- *"Vender 5k/mês no Instagram é teto. Vender 5k/mês com loja própria é base."*
- *"Quem depende do feed perde sono. Quem tem método dorme."*

### ICP 1 — Migração / Escala (~10% da base)
- **Faturamento:** R$20k+/mês
- **Dores:** Escalar sem perder controle, tráfego não escala, gestão de time, previsibilidade, margem
- **Produto-alvo:** Consultoria
- **Tom:** 50% Mentor / 50% Sábio — respeita a maturidade, vai direto ao gargalo
- **Linguagem:** Técnica. CAC, LTV, ROAS, margem, churn, payback são bem-vindos sem explicação.
- **Ganchos que funcionam:** "escala com método", "gestão que funciona sem você", "previsibilidade", "margem real, não vaidade"
- **Formatos que mais convertem:** Carrossel com dados e gráficos, Reels com Bruno opinando sobre tendência, Live com case
- **Evitar:** Linguagem de iniciante, tom condescendente, promessas de "primeiras vendas", emojis em excesso

**Hooks aprovados para ICP 1:**
- *"Faturamento cresce. Lucro não. Você reconhece esse problema?"*
- *"CAC subiu 40% no último ano. Quem não fez a conta vai sentir."*
- *"Escalar sem método é só estresse com mais dígitos."*

---

## 6. Técnicas de copywriting aplicadas ao Instagram

Mesma base da skill de e-mail (Cialdini, Seth Godin, Ogilvy), com adaptações para a lógica de cada formato. A marca usa persuasão ética, nunca manipulação.

### 6.1 Princípios de Cialdini no Instagram

**Reciprocidade** — Entregar valor antes de pedir. Carrosséis e Reels educacionais são reciprocidade pura. Se o post não ensina algo concreto, não vale entregar oferta no mesmo post.
- ✅ Carrossel ensina os 5 erros de quem está começando + último card oferece a Assinatura
- ❌ Carrossel inteiro vendendo a Assinatura sem entregar valor antes

**Prova social** — Cases reais com número, prazo e contexto. No Instagram, prova social vira print de WhatsApp, depoimento em vídeo curto, before/after da loja.
- ✅ Reels com aluno falando em primeira pessoa: nome, prazo, resultado, contexto
- ✅ Carrossel "De 0 a R$10k em 60 dias: o que ele fez"
- ❌ "Nossos alunos faturam milhões!" sem nome, prazo ou número específico

**Autoridade** — 10 anos no mercado, 150 mil empreendedores, parte do grupo Nuvemshop, Bruno de Oliveira como autor. Reforçar com regularidade, sem repetir mecanicamente.
- ✅ Bruno de Oliveira na arte ou em vídeo — credencial visual silenciosa
- ✅ "Em 10 anos de Ecommerce na Prática, o erro que mais matou loja foi este."

**Escassez real** — Lançamento de turma com vagas limitadas, condição de preço com prazo real. Nunca falsa.
- ✅ "Inscrições da turma de outubro fecham domingo." — quando for verdade
- ❌ "Últimas vagas!" toda semana

**Compromisso e coerência** — Pequenos sins. CTA leve antes do CTA pesado. Comentar uma palavra → receber link → checkout.
- ✅ "Comenta MÉTODO e te mando o passo a passo no direct" — micro-conversão antes da venda

**Afinidade** — Mostrar que conhecemos a realidade do lojista. Linguagem, cenário, dor, rotina.
- ✅ Reels com cenário real de quem empacota pedido na sala de casa, não com lifestyle de Dubai

### 6.2 Seth Godin no Instagram

**Permission marketing** — O seguidor deu o follow em troca de valor. Cada post precisa honrar isso.
- Regra prática: se o post não entrega utilidade, opinião ou história real, não posta.

**Específico para o menor grupo possível** — Não tente falar com todo mundo. Cada post escolhe um ICP.
- ✅ Hook específico: "Se você fatura entre R$5k e R$15k e travou…" — fala diretamente com ICP 2
- ❌ "Para todos os empreendedores brasileiros" — genérico, ninguém se reconhece

**Histórias reais > argumentos genéricos** — A marca prefere uma história de aluno bem contada a três bullets de benefícios.

### 6.3 Ogilvy no Instagram

**O hook é 80% do trabalho** — No feed, é a arte + primeira linha. No Reels, são os primeiros 2 segundos. No carrossel, é o card 1. Dedique pelo menos o mesmo tempo ao hook que ao resto.

**Escreva para uma pessoa, não para uma audiência** — "Você está vendendo pelo Instagram." > "Vocês, empreendedores, estão…"

**Fatos específicos > adjetivos** — "150 mil empreendedores em 10 anos" > "uma metodologia incrível"

---

## 7. Colaborações com parceiros — regras específicas

### 7.0 Consulta obrigatória à planilha de Parceiros

**Sempre que o conteúdo for collab, antes de produzir qualquer linha de copy, ler a planilha oficial de Parceiros do Ecommerce na Prática:**

- **URL:** https://docs.google.com/spreadsheets/d/1ZUQpEBAaNLo4_sbiqBGxUOm4orJJubWUeN7n_V5-24U/edit
- **File ID:** `1ZUQpEBAaNLo4_sbiqBGxUOm4orJJubWUeN7n_V5-24U`
- **Como ler:** usar `Google Drive:read_file_content` com o File ID acima.

**Estrutura esperada da planilha (4 colunas):**

| Coluna | Conteúdo | Como usar |
|---|---|---|
| Parceiro | Nome do parceiro | Para confirmar se está cadastrado |
| O que faz? | Descrição do que o parceiro entrega | Compor o argumento de autoridade no copy |
| Benefício da parceria EnP | Benefício específico para alunos do Ecommerce na Prática (desconto, cupom, mensalidade grátis, freemium, etc.) | **Vira eixo central do CTA quando houver** |
| Link/Cupom | Cupom de desconto ou link específico de afiliado | Vai no CTA / link na bio / sticker do Story |

**Se a planilha não puder ser lida** (erro de acesso, quota, sem conexão Google Drive): avisar o solicitante de forma transparente: *"Não consegui ler a planilha de parceiros agora. Pode confirmar manualmente: este parceiro tem algum benefício ativo para a base do Ecommerce na Prática?"* Seguir o briefing normal sem cruzamento.

### 7.1 Lógica de decisão após ler a planilha

**Cenário A — Parceiro está na planilha E tem benefício preenchido:**
- O benefício é o eixo central do CTA. Não comunicar collab sem mencionar o que a base ganha.
- Exemplo: se o parceiro é Bling e o benefício é "3 meses grátis", o CTA não pode ser apenas "siga @bling". Tem que ser: *"3 meses grátis de Bling para quem é da base do Ecommerce na Prática. Cupom: #viverdeecommerce03. Link na bio."*
- A coluna "O que faz?" vira o argumento de autoridade no corpo do post.

**Cenário B — Parceiro está na planilha SEM benefício preenchido:**
- Avisar o solicitante: *"O parceiro [X] está cadastrado mas não tem benefício ativo registrado. Quer comunicar collab institucional, ou validar com o time se há benefício a ser incluído?"*
- Se for institucional, seguir o fluxo padrão de collab (sem CTA de benefício específico).

**Cenário C — Parceiro NÃO está na planilha:**
- Avisar o solicitante: *"Este parceiro não está na planilha oficial de Parceiros. É um cadastro novo a fazer, ou uma collab pontual sem benefício para a base?"*
- Não inventar benefício. Não usar cupom de outro parceiro.
- Se for pontual: seguir o fluxo padrão de collab, sem cruzamento.
- Se for cadastro novo: sugerir ao solicitante que adicione o parceiro na planilha antes de produzir o conteúdo, para garantir consistência futura.

### 7.2 Dados obrigatórios do parceiro (após cruzamento com a planilha)

1. Nome e @ do Instagram (perguntar — a planilha não traz isso)
2. Área de atuação / autoridade do parceiro (vem da coluna "O que faz?" da planilha; validar com solicitante)
3. Tipo de parceria: paga, troca, parceiro estratégico, parceiro de conteúdo
4. Quem é o "dono" do conteúdo (nosso público, do parceiro, ou ambos)
5. Existe contrato, briefing prévio ou alinhamento de mensagens-chave?
6. Tem CTA cruzado (perfil do parceiro) e onde vai entrar?
7. **Benefício para a base** (vem da coluna "Benefício da parceria EnP")
8. **Link/Cupom** (vem da coluna "Link/Cupom") — usar exatamente como aparece, sem inventar variações

### 7.3 O que muda no copy em collab

**Crédito explícito ao parceiro**
- Mencionar o nome e @ logo no início (legenda) ou no card de capa (carrossel)
- Em Reels: nomear o parceiro nos primeiros 5 segundos OU em texto na tela na abertura
- Em Stories: marcar o @ na primeira tela

**Tom adaptado ao co-branding**
- Se o parceiro é técnico/especialista (ex.: Bling, BaseLinker): tom mais Sábio (50/50 ou até 40/60), porque a credencial dele autoriza ir mais fundo na operação
- Se o parceiro é case de sucesso (ex.: aluno que virou referência): tom mais Mentor (70/30) — a história da pessoa carrega a empatia
- Se o parceiro é institucional (ex.: Nuvemshop, evento de mercado): tom 50/50, com foco em autoridade conjunta
- Se o parceiro entrega serviço de apoio (ex.: contabilidade, escritório virtual): tom 60/40 padrão, foco em redução de risco e profissionalização

**CTA com benefício específico (quando houver)**
- Quando a planilha indicar benefício ativo, o CTA principal **integra** o benefício. Não é "siga @parceiro", é "use [benefício] que a base do Ecommerce na Prática tem".
- Estrutura: *"[Benefício específico]. Cupom: [cupom da planilha]. Link na bio."*
- O cupom/link da planilha vai exatamente como aparece, sem reinterpretar.

**CTA cruzado (sempre presente em collab)**
- O CTA principal continua sendo nosso. Quando houver benefício, o CTA principal já incorpora o benefício do parceiro (ver acima).
- Quando não houver benefício, o CTA do parceiro entra como CTA secundário no fim.
- Ordem padrão (sem benefício): "Salva esse post. Segue @parceiro pra conteúdo de [área]. Link na bio pra começar."
- Em Reels: CTA principal nos últimos 3 segundos; menção ao parceiro pode ser na legenda ou no card final.

**Linguagem de pertencimento, não de hierarquia**
- ✅ "A gente trouxe @parceiro pra falar sobre X porque ele opera isso todo dia."
- ❌ "Convidamos o renomado especialista @parceiro para honrar nosso perfil…"

### 7.4 Disclosure obrigatório (regulação)

Se a collab é paga ou patrocinada, marcar como **#publi** ou usar a tag de parceria paga do Instagram. Não esconder. Disclosure explícito reforça credibilidade e cumpre o CONAR.

Parcerias com benefício para a base (cupom, desconto, freemium) **não são** automaticamente publi — depende do acordo comercial. Validar com o solicitante quando a natureza da parceria não estiver clara.

### 7.5 Checklist específico de collab

Antes de entregar conteúdo de collab, verificar:
- [ ] Planilha de Parceiros foi consultada
- [ ] Status do parceiro identificado (cadastrado com benefício / cadastrado sem benefício / não cadastrado)
- [ ] @ do parceiro está correto (com @, sem espaços, sem typo)
- [ ] Nome do parceiro e contexto da autoridade dele estão no conteúdo
- [ ] Benefício específico (se houver) está integrado ao CTA principal
- [ ] Cupom/link da planilha foi usado exatamente como cadastrado, sem inventar variação
- [ ] Disclosure (#publi ou tag oficial) presente quando aplicável
- [ ] Mensagens-chave alinhadas com briefing do parceiro
- [ ] Tom do co-branding ajustado conforme tipo de parceiro
- [ ] Nenhuma palavra proibida da marca (ver seção 8)

---

## 8. Vocabulário e padrões de IA — eliminar sempre

### 8.1 Usamos
E-commerce, loja virtual, loja própria, vendas online, método, metodologia, caminho, jornada, estrutura, estruturar, profissionalizar, escalar, crescer com consistência, destrave, CAC, LTV, ROAS, Markup, churn, conversão (explicar na primeira menção para ICP 5), resultado, execução, dados, métricas, prazo, especialista, profissional de mercado, quem opera no dia a dia.

### 8.2 Evitamos
- "Incrível", "revolucionário", "extraordinário", "fantástico"
- "Segredo", "fórmula mágica", "método secreto"
- "Renda extra", "dinheiro fácil", "fique rico"
- "Últimas vagas" ou "oferta imperdível" *(quando não for verdade)*
- "Simplesmente", "apenas" *(minimizam a dificuldade real)*
- "Parceiros", "colaboradores" *(para clientes — são alunos ou lojistas)*

### 8.3 Proibidas
- Promessa de resultado garantido ("você vai faturar X")
- Linguagem que associe empreendedorismo a riqueza fácil
- Marketplaces como canal principal ou único
- Mencionar plataformas concorrentes à Nuvemshop
- Abreviações: "EnP", "enp", "E-commerce na Prática" com hífen
- "nuvem shop", "NS"

### 8.4 Sinais de IA que precisam ser eliminados

**Pontuação:**
- Travessão (—) no meio de frases → substituir por vírgula, ponto ou dois-pontos
- Listas de três itens perfeitamente balanceados em todo o texto

**Vocabulário:**
- "Mergulhar", "navegar" (no sentido figurado), "paisagem" (cenário), "robusto", "abrangente", "holístico", "alavancar"
- "É fundamental/crucial/essencial" no início de frase
- "Em suma", "em resumo" abrindo parágrafo final
- "É importante ressaltar que…", "Vale destacar que…"

**Tom e ritmo:**
- Transições suaves demais ("Além disso", "Por outro lado", "Nesse sentido")
- Texto sem opinião ou atrito
- Abertura que resume o que vai ser dito antes de dizer

**Como soar humano:**
- Frases curtas para impacto. Frases longas para raciocínio.
- Começar frase com "E", "Mas", "Porque" quando fizer sentido
- Opinião direta: "Isso não funciona." em vez de "Pode ser que não seja a abordagem mais eficaz."

---

## 9. Checklist de qualidade — antes de entregar qualquer conteúdo

- [ ] Briefing completo (formato, parceria, objetivo, produto, ICP, CTA) confirmado pela Ana?
- [ ] Hook para no primeiro segundo / primeira linha / primeiro card?
- [ ] Uma única ideia central no conteúdo?
- [ ] Pelo menos um dado concreto, prazo ou exemplo real?
- [ ] CTA único, específico, sem urgência falsa?
- [ ] Tom calibrado para o ICP (proporção Mentor/Sábio correta)?
- [ ] Especificações de dimensão / duração / número de cards conforme `references/formatos.md`?
- [ ] Nome da marca correto? (Ecommerce na Prática, Nuvemshop)
- [ ] Nenhuma palavra proibida ou padrão de IA?
- [ ] Se collab: @ do parceiro, disclosure, CTA cruzado conferidos?
- [ ] Estaria confortável se o Bruno de Oliveira lesse / assistisse isso?

---

## 10. Estrutura de entrega — como devolver para a Ana

Sempre entregar o conteúdo organizado por blocos claros, separados visualmente. Modelo padrão:

```
📌 BRIEFING CONFIRMADO
- Formato: [X]
- ICP: [Y]
- Produto: [Z]
- Objetivo: [W]
- Collab: [Sim/Não — se sim, dados]

🎯 [FORMATO ESPECÍFICO]
[Conteúdo estruturado conforme references/formatos.md]

📐 ESPECIFICAÇÕES TÉCNICAS
- Dimensão: [valor]
- Duração / nº de cards: [valor]
- Áreas seguras: [se aplicável]

📝 LEGENDA (quando aplicável)
[Texto da legenda]

🏷️ HASHTAGS SUGERIDAS
[Lista]

✅ CHECKLIST FINAL
[Itens da seção 9]
```

Para múltiplos formatos no mesmo briefing (ex.: lançamento que pede Reels + Stories + Carrossel), entregar um por vez, perguntando antes se quer todos seguidos ou um por turno.

---

*Este skill é a fonte da verdade para conteúdo de Instagram da marca. Em conflito com outra instrução genérica, este prevalece. Atualizações devem ser aprovadas pelo time de marketing.*
