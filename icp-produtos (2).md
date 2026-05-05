# Especificações por formato — Instagram

Documento de referência para a skill `enp-instagram-content`. Sempre consultar antes de entregar qualquer formato.

**Sumário**
1. Stories
2. Feed estático
3. Carrossel
4. Reels
5. Roteiro de Live

---

## 1. Stories

### 1.1 Especificações técnicas
- **Dimensão:** 1080 x 1920 px (vertical 9:16)
- **Duração por tela:** 5 a 15 segundos (15s é o limite nativo de vídeo)
- **Áreas seguras (não cobrir com texto):**
  - Topo: 250 px (nome de usuário, barra de progresso)
  - Base: 250 px (campo de mensagem, stickers, botões)
  - Texto e CTA principal devem ficar no terço central da tela
- **Formato:** PNG ou JPG para imagens; MP4 para vídeo (máximo 4 GB)
- **Tipografia:** Mínimo 32 px para garantir leitura no celular

### 1.2 Estrutura de uma sequência de Stories
Stories funcionam em sequência, não isolados. Pensar em "carrossel vertical com tempo".

**Sequência padrão de 4 a 7 telas:**

| Tela | Função | Conteúdo |
|---|---|---|
| 1 | Hook | Pergunta, dado ou paradoxo que para o scroll. Texto grande, fundo limpo. |
| 2 | Contexto | Por que isso importa. Conecta com a dor do ICP. |
| 3-5 | Desenvolvimento | Argumento, passo a passo, dados. Pode usar enquete, quiz ou pergunta. |
| Penúltima | Prova / dado / case | Número concreto + prazo + nome quando possível |
| Última | CTA | Sticker de link, "arrasta pra cima", botão de mensagem direta |

### 1.3 Stickers — quando usar
- **Enquete:** Engajamento + dado de comportamento (ex.: "Você já tem loja? Sim / Não")
- **Quiz:** Educacional. Dá ao seguidor a sensação de testar conhecimento.
- **Caixa de pergunta:** Topo de funil, conversa direta. "O que mais te trava hoje?"
- **Sticker de link:** Sempre na última tela quando há CTA de checkout
- **Countdown:** Lançamento, live, fim de campanha — só quando o prazo é real
- **Menção (@):** Em colab, na primeira tela e na última

### 1.4 Boas práticas de copy
- Uma frase por tela. Stories não é blog.
- Caixa alta com moderação — só para destaque pontual
- Emojis: 1 ou 2 por tela, no máximo. Sem fileiras.
- Voz em primeira pessoa funciona bem ("Eu vejo isso todo dia")

### 1.5 Exemplo de sequência aprovada (ICP 2, objetivo: vender Assinatura)

```
Tela 1 (Hook):
"Você vende pelo Instagram. E quando o algoritmo mudar?"

Tela 2 (Contexto):
"Algoritmo já mudou em 2018, 2020, 2022, 2024.
Cada mudança matou negócios."

Tela 3 (Enquete):
"Você tem loja própria?
[ ] Sim   [ ] Ainda não"

Tela 4 (Dado):
"R$497/ano = menos de R$1,65/dia.
Custa menos que um café."

Tela 5 (Prova):
"Em 60 dias, Jones tinha vendido R$10 mil.
Sem depender do feed."

Tela 6 (CTA):
[Sticker de link]
"Acesso completo. 1 ano. 12x R$49,37."
```

---

## 2. Feed estático (post único)

### 2.1 Especificações técnicas
- **Dimensão recomendada:** 1080 x 1350 px (4:5 vertical) — ocupa mais espaço no feed do que o quadrado
- **Quadrado tradicional:** 1080 x 1080 px (1:1) — para casos específicos
- **Tipografia mínima:** 36 px no celular
- **Áreas seguras:** Manter elementos importantes a no mínimo 60 px da borda

### 2.2 Quando usar feed estático
Feed estático é o formato menos usado da marca hoje, mas funciona em três casos:

1. **Frase de impacto / posicionamento de marca** — uma única ideia forte
2. **Cobertura visual de evento** — foto de bastidor, palco, aluno
3. **Anúncio rápido** — lançamento, mudança importante, comunicado

### 2.3 Estrutura
Feed estático é o formato mais "puro" do trio Hook-Desenvolvimento-CTA, porque tudo precisa caber em uma única arte + legenda.

**Arte:**
- Frase única, curta, com peso. 6 a 12 palavras idealmente.
- Tipografia hierárquica: palavra-chave em destaque (negrito, cor, tamanho)
- Logo no canto inferior — discreto, não invasivo
- Fundo limpo, contraste alto

**Legenda:**
- Primeira linha repete ou amplia o hook da arte
- Segunda linha quebra para contexto (Instagram só mostra ~125 caracteres antes do "ver mais")
- Desenvolvimento em 2 a 4 parágrafos curtos
- CTA na última linha
- Hashtags ao final ou no primeiro comentário (preferimos no primeiro comentário)

### 2.4 Exemplo aprovado (ICP 1, objetivo: posicionamento)

**Arte:**
> Faturamento cresce.
> Lucro não.

**Legenda:**
> Faturamento cresce. Lucro não.
>
> Quem opera e-commerce há mais de 2 anos conhece esse cenário. A receita sobe, mas a margem fica igual ou cai.
>
> Quase sempre é uma combinação de três coisas: CAC subindo sem ajuste de pricing, mix de produto desbalanceado e custo operacional escondido na operação do dia a dia.
>
> A boa notícia: dá pra resolver. A ruim: não com mais anúncio.
>
> Comenta MARGEM se você reconhece esse problema na sua operação.

---

## 3. Carrossel

### 3.1 Especificações técnicas
- **Dimensão recomendada:** 1080 x 1350 px (4:5 vertical) — todos os cards na mesma proporção
- **Número de cards:** mínimo 3, ideal 6 a 8, máximo 10 (limite do Instagram)
- **Áreas seguras:** Manter texto a no mínimo 60 px de qualquer borda
- **Indicador de "arraste":** Carrossel já mostra o ponto na parte inferior, mas é boa prática reforçar visualmente no card 1 (seta, "→", "arrasta")

### 3.2 Estrutura padrão de carrossel
Carrossel é o formato de maior profundidade. Tem lógica de "leitura", não de "imagem".

**Estrutura clássica (6 a 8 cards):**

| Card | Função | Conteúdo |
|---|---|---|
| 1 | Capa / Hook | Frase forte + arte de capa. Promete o que vem. |
| 2 | Contexto | Por que isso importa. Quem é o leitor. |
| 3-6 | Desenvolvimento | Argumento, passo a passo, dados, exemplos |
| Penúltimo | Síntese ou prova | Recap rápido OU case com nome/prazo/número |
| Último | CTA | Convite claro para ação |

### 3.3 O card 1 (capa) é 70% do trabalho
Igual ao headline de um anúncio Ogilvy. Se a capa não para o scroll, ninguém arrasta.

**Boas capas:**
- Pergunta direta ao ICP: *"Você fatura entre R$5k e R$15k? Leia."*
- Paradoxo: *"Mais anúncio não é a solução. Quase nunca é."*
- Promessa concreta: *"5 erros que travam quem está começando."*
- Dado provocativo: *"63% das lojas novas fecham no 1º ano. As outras 37% têm uma coisa em comum."*

**Capas reprovadas:**
- *"Dicas para vender mais!"* — vago, sem ICP
- *"Confira agora!"* — sem promessa de valor
- *"Tudo o que você precisa saber sobre e-commerce"* — abrangente demais

### 3.4 Ritmo de leitura
- Cada card precisa ter um motivo para ser arrastado para o próximo
- Final de cada card pode ter "gancho de continuidade": "Mas tem um detalhe…", "E é aqui que muda tudo:", "Veja o próximo →"
- Texto por card: 20 a 60 palavras. Mais que isso vira texto longo demais para mobile.
- Hierarquia visual em cada card: título (3-6 palavras grandes) + corpo (2-4 linhas curtas)

### 3.5 Card final — CTA
Tem dois trabalhos: dizer o que fazer e reforçar a marca.
- CTA específico: "Salva esse post pra revisar depois", "Comenta MÉTODO que te mando o link", "Link na bio pra começar"
- Reforço de marca: logo + frase de posicionamento (ex.: "Ecommerce na Prática — método para quem vende todos os dias")

### 3.6 Legenda do carrossel
Diferente do feed estático: a legenda aqui é complementar, não principal.
- Primeira linha: extensão do hook do card 1
- Desenvolvimento curto (2-3 parágrafos)
- CTA repete o do último card
- Hashtags no primeiro comentário

### 3.7 Exemplo aprovado (ICP 5, objetivo: educar + converter para Assinatura)

**Estrutura de 7 cards:**

```
Card 1 (Capa):
[Arte com fundo escuro, texto grande]
"5 erros que travam
quem está começando
do zero no e-commerce"
[Seta → no rodapé]

Card 2 (Contexto):
"Se você nunca vendeu, este post é pra você.

A gente conversa com 150 mil empreendedores há 10 anos.
Os mesmos erros aparecem sempre."

Card 3 (Erro 1):
"ERRO 1
Escolher produto pelo que você gosta.

Você gosta. Mas o mercado quer?
Produto sem demanda é estoque parado."

Card 4 (Erro 2):
"ERRO 2
Investir em anúncio antes de ter loja.

Tráfego pago para Instagram = entregar o cliente
para o algoritmo decidir se converte."

Card 5 (Erro 3):
"ERRO 3
Achar que precisa do produto perfeito.

Lojas reais começam com 5 a 10 produtos.
Coleção completa = decisão paralisada."

Card 6 (Erros 4 e 5 condensados):
"ERRO 4
Não calcular markup. Vende e perde dinheiro.

ERRO 5
Não ter loja própria. Depende de quem manda no algoritmo."

Card 7 (CTA):
"O método para começar do jeito certo.

Acesso completo por 1 ano.
12x R$49,37 — menos de R$1,65/dia.

[Logo Ecommerce na Prática]
Link na bio pra começar."
```

---

## 4. Reels

### 4.1 Especificações técnicas
- **Dimensão:** 1080 x 1920 px (vertical 9:16)
- **Duração:** 15 a 90 segundos. Sweet spot para a marca: **30 a 60 segundos**.
- **Reels muito curto (até 15s):** opinião pontual, frase forte, dado isolado
- **Reels médio (30-60s):** o padrão da marca. Argumento completo.
- **Reels longo (60-90s):** roteiro com Bruno explicando conceito, case detalhado
- **Áreas seguras (não cobrir com texto):**
  - Topo: 250 px (nome, áudio)
  - Base: 350 px (legenda, botões, áudio)
- **Áudio:** original (próprio) ou trending. Trending aumenta alcance — verificar antes se o áudio já é tendência.
- **Legenda do post:** texto que aparece abaixo do vídeo no feed

### 4.2 Estrutura cena a cena (Reels de 30 a 60s)
Reels da marca tem 4 blocos. Cada bloco com função clara.

**Bloco 1 — HOOK (0 a 3 segundos)**
- Texto na tela: frase curta, 4-8 palavras, alto contraste
- Áudio: começa com afirmação forte, pergunta ou paradoxo
- Direção visual: rosto na câmera OU close em objeto que ilustra a dor OU texto dominando a tela
- **Se em 3 segundos não para o scroll, o Reels morre.**

**Bloco 2 — CONTEXTO (3 a 10 segundos)**
- Validação da dor: "Eu vejo isso todo dia", "Quem fatura X conhece esse problema"
- Texto na tela complementa o áudio (não repete)
- Direção visual: corte para outra perspectiva, mudança de ângulo

**Bloco 3 — DESENVOLVIMENTO (10 a 50 segundos)**
- Argumento, método, dado, história
- Idealmente 2 a 4 micro-cortes para manter ritmo
- Texto na tela aparece em momentos-chave (não toda hora)
- Se for case: nome + prazo + número
- Se for método: numerar passos visualmente ("1", "2", "3" entrando na tela)

**Bloco 4 — CTA (últimos 5 a 10 segundos)**
- Texto grande na tela
- Áudio: convite direto e específico
- CTA possível: "Salva esse Reels", "Comenta [palavra]", "Link na bio", "Segue pra mais"

### 4.3 Roteiro completo — formato de entrega

Reels precisam ser entregues em formato que a Ana consiga passar direto para quem vai gravar/editar. Modelo:

```
🎬 REELS — [TÍTULO INTERNO]
Duração estimada: [X]s
Áudio: [original ou nome do trending]

═══════════════════════════════
CENA 1 — HOOK (0:00 - 0:03)
─────────────────────────────
🎙️ Áudio: "[Fala exata do apresentador]"
🎥 Direção visual: [Onde a câmera está, quem aparece, ação]
📝 Texto na tela: "[Texto curto, alto contraste]"
✂️ Corte: [Hard cut / fade / zoom]

═══════════════════════════════
CENA 2 — CONTEXTO (0:03 - 0:10)
─────────────────────────────
🎙️ Áudio: "..."
🎥 Direção visual: ...
📝 Texto na tela: "..."
✂️ Corte: ...

═══════════════════════════════
CENA 3 — DESENVOLVIMENTO (0:10 - 0:45)
─────────────────────────────
[Subdividir em micro-cenas se necessário]
...

═══════════════════════════════
CENA 4 — CTA (0:45 - 0:55)
─────────────────────────────
🎙️ Áudio: "..."
🎥 Direção visual: ...
📝 Texto na tela: "..."

═══════════════════════════════

📝 LEGENDA DO POST:
[Texto da legenda, 2 a 4 linhas]

🏷️ HASHTAGS:
[Lista no primeiro comentário]
```

### 4.4 Boas práticas específicas de Reels da marca
- **Bruno na câmera funciona.** Aparição do fundador gera credibilidade. Quando possível, propor versões com Bruno.
- **Texto na tela é obrigatório.** 80% dos Reels são vistos sem som. Se precisar de áudio para entender, perdeu metade do alcance.
- **Cortes a cada 3-5 segundos.** Reels parado mata retenção.
- **Não começa com "Oi gente, hoje eu vou falar sobre…"**. Entra direto no hook.
- **Legenda funciona como segundo CTA.** Não repetir o roteiro — complementar.

### 4.5 Exemplo aprovado (ICP 2, objetivo: educar + converter)

```
🎬 REELS — "DEPENDÊNCIA DO INSTAGRAM"
Duração estimada: 45s
Áudio: original

═══════════════════════════════
CENA 1 — HOOK (0:00 - 0:03)
─────────────────────────────
🎙️ Áudio: "Vender pelo Instagram é teto. Não é base."
🎥 Direção visual: Bruno frontal na câmera, olhar direto
📝 Texto na tela: "Vender pelo Instagram É TETO"
✂️ Corte: Hard cut

═══════════════════════════════
CENA 2 — CONTEXTO (0:03 - 0:12)
─────────────────────────────
🎙️ Áudio: "Você vende cinco mil por mês pelo direct. Parabéns. Mas e quando o algoritmo mudar de novo?"
🎥 Direção visual: Bruno em movimento, sentando à mesa com notebook
📝 Texto na tela: "Já mudou em 2018, 2020, 2022, 2024"
✂️ Corte: Zoom in

═══════════════════════════════
CENA 3 — DESENVOLVIMENTO (0:12 - 0:38)
─────────────────────────────
Sub-cena 3a (12-22s):
🎙️ Áudio: "Loja própria não é luxo. É controle. Você decide o preço, o frete, o checkout, o público que volta."
🎥 Direção visual: Tela do notebook mostrando uma loja Nuvemshop
📝 Texto na tela: "LOJA PRÓPRIA = CONTROLE"

Sub-cena 3b (22-32s):
🎙️ Áudio: "Em 60 dias, o Jones tinha vendido mais de dez mil reais com loja própria. Não dependeu de algoritmo."
🎥 Direção visual: Print de loja real do aluno + número aparecendo na tela
📝 Texto na tela: "60 DIAS · R$10.000 · LOJA PRÓPRIA"

Sub-cena 3c (32-38s):
🎙️ Áudio: "E o investimento pra ter o método completo é menos de um real e sessenta e cinco por dia."
🎥 Direção visual: Volta para Bruno na câmera
📝 Texto na tela: "R$1,65/DIA"

═══════════════════════════════
CENA 4 — CTA (0:38 - 0:45)
─────────────────────────────
🎙️ Áudio: "Comenta MÉTODO que eu te mando o link no direct."
🎥 Direção visual: Bruno apontando para a câmera
📝 Texto na tela: "COMENTA MÉTODO ⬇️"

═══════════════════════════════

📝 LEGENDA DO POST:
Vender pelo Instagram é teto. Loja própria é base.

Quem fatura R$5k pelo direct sabe do que estou falando: o algoritmo manda, você obedece.

Comenta MÉTODO que te mando o link.

🏷️ HASHTAGS (no primeiro comentário):
#ecommerce #lojavirtual #empreendedorismo #vendasonline #nuvemshop
```

---

## 5. Roteiro de Live

### 5.1 Especificações técnicas
- **Plataforma:** Instagram Live (sozinho ou com convidado)
- **Duração ideal:** 30 a 60 minutos
- **Lives mais curtas (15-25 min):** anúncio, conteúdo único, Q&A pontual
- **Lives padrão (30-45 min):** estrutura completa com aquecimento, conteúdo, oferta
- **Lives longas (60+ min):** evento, lançamento, masterclass

### 5.2 Estrutura de uma live de venda (45 minutos)

| Bloco | Tempo | Função |
|---|---|---|
| Aquecimento | 0:00 - 5:00 | Receber audiência, esperar entrar gente, apresentação |
| Promessa da live | 5:00 - 8:00 | O que vai ser entregue hoje. Por que ficar até o fim. |
| Conteúdo principal | 8:00 - 30:00 | Ensinamento, método, argumento — a entrega de valor |
| Oferta | 30:00 - 38:00 | Apresentação do produto, preço, condição |
| Q&A | 38:00 - 43:00 | Responder dúvidas reais da audiência |
| Fechamento | 43:00 - 45:00 | Recap + CTA final + agradecimento |

### 5.3 CTAs por bloco
Cada bloco tem um CTA diferente. Não pedir compra desde o minuto 1.

| Bloco | CTA típico |
|---|---|
| Aquecimento | "Comenta de onde você está assistindo" |
| Promessa da live | "Marca um amigo que precisa ver isso" |
| Conteúdo principal | "Salva o stories pra revisar depois" / "Comenta [palavra]" |
| Oferta | "Link na bio. Vagas limitadas até [prazo real]" |
| Q&A | "Pergunta no comentário" |
| Fechamento | "Link na bio agora" |

### 5.4 Formato de entrega do roteiro

Roteiros de live são entregues em formato detalhado, com falas-chave, pontos de atenção e CTAs por bloco. A pessoa que apresenta a live (geralmente Bruno ou convidado) usa o roteiro como guia, não como script literal.

```
🎙️ LIVE — [TÍTULO]
Data: [data]
Duração estimada: [X] minutos
ICP: [Y]
Objetivo principal: [Z]
Convidado (se houver): [nome + @ + autoridade]

═══════════════════════════════════════════
BLOCO 1 — AQUECIMENTO (0:00 - 5:00)
═══════════════════════════════════════════

🎯 Objetivo do bloco: receber audiência, criar atmosfera

Pontos de fala:
- Apresentação rápida (nome, contexto)
- Cumprimento de quem está chegando
- "Vamos começar em 2 minutos, esperando vocês entrarem"
- Se tiver convidado: apresentação do convidado em 30 segundos

CTA do bloco:
"Comenta de onde você tá assistindo. E marca um amigo que precisa ver essa live."

⚠️ Pontos de atenção:
- Não começar conteúdo antes de ter pelo menos 30 pessoas online
- Repetir o tema da live nesta fase (audiência entra fora de ordem)

═══════════════════════════════════════════
BLOCO 2 — PROMESSA DA LIVE (5:00 - 8:00)
═══════════════════════════════════════════

🎯 Objetivo do bloco: deixar claro o que será entregue, ancorar a audiência

Falas-chave:
"Hoje vou mostrar [X], com [Y] e [Z]. Quem ficar até o final ainda tem [oferta exclusiva da live, se houver]."

[Se houver oferta exclusiva: descrever brevemente sem entregar o preço]

CTA do bloco:
"Comenta FICO se você vai ficar até o fim."

═══════════════════════════════════════════
BLOCO 3 — CONTEÚDO PRINCIPAL (8:00 - 30:00)
═══════════════════════════════════════════

🎯 Objetivo do bloco: entregar valor real, construir autoridade, criar pré-disposição para a oferta

Estrutura sugerida:
1. Dor / problema central (8:00-12:00)
2. Por que a maioria erra ao tentar resolver (12:00-17:00)
3. O método / abordagem certa (17:00-25:00)
4. Caso real / prova (25:00-30:00)

Pontos de fala-âncora (preencher conforme tema):
- [Dor específica do ICP]
- [Erro mais comum que o ICP comete]
- [Método ou framework — pode ser passo a passo]
- [Case com nome + prazo + número]

CTA do bloco:
"Comenta [palavra-chave do tema] que vou marcar quem comentou."

⚠️ Pontos de atenção:
- A cada 5 minutos: cumprimentar quem chegou recente
- Pegar 1 ou 2 perguntas do chat dentro do bloco — não esperar o Q&A formal
- Se for collab: dar protagonismo ao convidado nos blocos onde a autoridade dele é maior

═══════════════════════════════════════════
BLOCO 4 — OFERTA (30:00 - 38:00)
═══════════════════════════════════════════

🎯 Objetivo do bloco: apresentar produto, tratar 2 ou 3 objeções principais, conduzir ao link

Estrutura:
1. Transição: "Tudo que mostrei até aqui está sistematizado em [produto]" (30:00-31:00)
2. Apresentação do produto (31:00-34:00)
   - O que é, para quem é, o que entrega
   - Diferenciação clara em relação ao que existe gratuitamente
3. Preço e condição (34:00-36:00)
   - Apresentar parcelado primeiro
   - Âncora de custo diário (Assinatura: "menos de R$1,65/dia")
4. Tratamento de objeção (36:00-38:00)
   - Objeção 1 (preço): reframe pelo custo de não agir
   - Objeção 2 (tempo): "qualquer hora é hora certa quando o método está claro"

CTA do bloco:
"Link na bio agora. Esse preço é exclusivo da live e vai até [prazo real]."

⚠️ Pontos de atenção:
- Não usar urgência falsa. Se não há prazo real, não inventar.
- Mostrar o link na tela em texto grande (sticker no celular ou texto sobreposto)
- Não disfarçar que é venda. A audiência sabe.

═══════════════════════════════════════════
BLOCO 5 — Q&A (38:00 - 43:00)
═══════════════════════════════════════════

🎯 Objetivo do bloco: tratar dúvidas reais, transformar em prova social

Como conduzir:
- Pegar 5 a 8 perguntas reais do chat
- Priorizar perguntas sobre o produto e perguntas que tratam objeções comuns
- Para cada pergunta: nome de quem perguntou + resposta direta
- Se a pergunta for sobre tema fora do escopo da live, agradecer e dizer que tem post sobre isso

CTA do bloco:
"Pergunta no comentário que ainda dá tempo."

═══════════════════════════════════════════
BLOCO 6 — FECHAMENTO (43:00 - 45:00)
═══════════════════════════════════════════

🎯 Objetivo do bloco: recap, último CTA, agradecimento

Estrutura:
1. Recap do que foi entregue (43:00-44:00)
2. CTA final (44:00-44:30)
   "Link na bio. Preço da live até [prazo]."
3. Agradecimento + próximo conteúdo (44:30-45:00)
   "Próxima live é [dia]. Tema: [X]. Te espero."

CTA do bloco:
"Compartilha essa live nos seus stories. E link na bio."

═══════════════════════════════════════════

📝 LEGENDA DO POST DE COBERTURA (após a live):
[Texto resumindo principais aprendizados, com CTA para o IGTV/Reels da live editada]

🏷️ HASHTAGS:
[Lista]
```

### 5.5 Boas práticas de live da marca
- **Não fazer live sem objetivo claro.** Live sem CTA é entretenimento, não marketing.
- **Anunciar com antecedência:** Story de countdown 24h antes + Reels de chamada 48h antes + post no feed no dia
- **Se for collab:** alinhar com o parceiro a divisão de blocos (quem fala o quê) com 24h de antecedência
- **Salvar a live:** sempre salvar para depois cortar em Reels e fazer cobertura no feed
- **Não fazer live sozinho do zero:** Bruno ou Ana ou parceiro convidado funcionam melhor que rosto novo da marca

---

*Atualizações neste documento devem ser refletidas também no SKILL.md principal quando alterarem fluxo de briefing ou estrutura de entrega.*
