---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Razão
  - Proporção
  - Regra de três
  - Grandezas proporcionais
tags:
  - aritmetica
---
# Razão, Proporção e Regra de Três

> [!abstract] Em uma frase
> **Razão** é comparar por divisão; **proporção** é a igualdade entre duas razões. Quando duas grandezas variam na mesma razão (direta ou inversa), a **regra de três** acha o valor que falta.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Frações e Equivalência]], [[Operações com Frações]], [[Números Decimais]] · **Próximo:** [[Porcentagem]]
**Praticar:** [[Razão, Proporção e Regra de Três - Exercícios]] · [[Razão, Proporção e Regra de Três - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Usar razões em escalas, velocidades e proporções de tela.
- Aplicar a **propriedade fundamental** das proporções.
- Distinguir grandezas **diretamente** e **inversamente** proporcionais.
- Resolver regras de três **simples** e **compostas** e dividir um valor em partes proporcionais.

---

## 1. Razão

A **razão** entre $a$ e $b$ é $\frac{a}{b}$ (ou $a : b$, que se lê "a está para b"). Ela diz **quantas vezes** uma quantidade cabe na outra.

| Razão | Exemplo |
|---|---|
| **Escala** | 1 : 50.000 → 1 cm no mapa = 50.000 cm (0,5 km) na realidade |
| **Velocidade** | 180 km em 2 h → $\frac{180}{2} = 90$ km/h |
| **Proporção de tela** | 1920 : 1080 = 16 : 9 (veja [[MMC e MDC]]) |
| **Densidade demográfica** | habitantes por km² |

> [!warning] Unidades
> Numa razão entre grandezas **da mesma espécie**, use a **mesma unidade**: a razão entre 30 cm e 2 m é $\frac{30}{200} = \frac{3}{20}$, e não $\frac{30}{2}$.

## 2. Proporção e a propriedade fundamental

Uma **proporção** é uma igualdade de razões: $\frac{a}{b} = \frac{c}{d}$ (lê-se "a está para b assim como c está para d").

> [!important] Propriedade fundamental
> $$\frac{a}{b} = \frac{c}{d} \iff a \cdot d = b \cdot c$$
> (O produto dos **extremos** é igual ao produto dos **meios**; na prática, é a "multiplicação cruzada".)

Ela vem de multiplicar os dois lados por $b \cdot d$. Exemplo: $\frac{x}{12} = \frac{5}{4} \Rightarrow 4x = 60 \Rightarrow x = 15$.

## 3. Grandezas direta e inversamente proporcionais

> [!tip] O teste do "dobro"
> **Dobre** uma grandeza e veja o que acontece com a outra (mantendo todo o resto igual):
> - **dobra** também → **diretamente proporcionais**: a razão $\frac{y}{x}$ é constante;
> - **cai pela metade** → **inversamente proporcionais**: o produto $x \cdot y$ é constante;
> - nenhum dos dois → **não são proporcionais**, e a regra de três **não** se aplica.

| Grandezas | Tipo |
|---|---|
| Quilos de arroz × preço pago | direta |
| Velocidade × tempo (para a mesma distância) | inversa |
| Número de pedreiros × dias para terminar a obra | inversa |
| Idade × altura de uma pessoa | **nenhuma** |

## 4. Regra de três simples

1. Monte uma tabela com as grandezas em colunas.
2. Coloque uma seta na coluna do $x$.
3. Decida se a outra grandeza é direta (seta no **mesmo** sentido) ou inversa (seta **contrária**).
4. Se for inversa, **inverta** essa coluna e resolva a proporção.

> [!example] Direta
> 5 kg custam R\$ 32,50. Quanto custam 8 kg?
> $$\frac{5}{8} = \frac{32{,}50}{x} \Rightarrow 5x = 260 \Rightarrow x = 52$$

> [!example] Inversa
> 6 pedreiros fazem uma obra em 10 dias. Em quantos dias 4 pedreiros fazem a mesma obra?
> Menos pedreiros significa **mais** dias: é inversa. Invertendo a coluna dos pedreiros:
> $$\frac{10}{x} = \frac{4}{6} \Rightarrow 4x = 60 \Rightarrow x = 15 \text{ dias}$$
> Pense também no "trabalho total": $6 \cdot 10 = 60$ pedreiro-dias, e $60 \div 4 = 15$.

## 5. Regra de três composta

Com três ou mais grandezas, compare **cada uma com a do $x$, separadamente** (supondo as outras fixas).

> [!example] 8 máquinas produzem 600 peças em 5 dias. Quantas peças 10 máquinas produzem em 6 dias?
> | Máquinas | Dias | Peças |
> |---|---|---|
> | 8 | 5 | 600 |
> | 10 | 6 | $x$ |
>
> Mais máquinas → mais peças (direta); mais dias → mais peças (direta).
> $$x = 600 \cdot \frac{10}{8} \cdot \frac{6}{5} = 600 \cdot 1{,}25 \cdot 1{,}2 = 900$$

**Atalho:** parta do valor conhecido de $x$ e multiplique por cada razão, "para cima" se a grandeza aumenta o $x$ e "para baixo" se diminui.

## 6. Divisão em partes proporcionais

Dividir R\$ 1.200 em partes proporcionais a 2, 3 e 5: o total de "partes" é $2 + 3 + 5 = 10$, e cada parte vale $1200 \div 10 = 120$. Então as partes são $240$, $360$ e $600$.

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: escala
> Num mapa de escala 1 : 50.000, duas cidades estão a 4 cm. A distância real é $4 \cdot 50.000 = 200.000$ cm $= 2$ km.

> [!example] Exemplo 2: imagem
> Uma imagem de $1920 \times 1080$ vai ter 1280 de largura, mantendo a proporção. Altura: $\frac{1920}{1080} = \frac{1280}{h} \Rightarrow h = \frac{1080 \cdot 1280}{1920} = 720$.

> [!example] Exemplo 3: com frações
> Uma torneira enche $\frac{2}{3}$ de um tanque em 1,5 h. Quanto tempo leva para encher o tanque todo?
> $\frac{2}{3}$ do tanque → 1,5 h; 1 tanque → $x$. É direta: $x = 1{,}5 \div \frac{2}{3} = 1{,}5 \cdot \frac{3}{2} = 2{,}25$ h $=$ **2 h 15 min**.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| Resolver toda regra de três "em cruz" | primeiro decida se é direta ou inversa | mais pedreiros → **menos** dias |
| Misturar unidades (min com h, cm com m) | converta tudo antes | |
| Usar regra de três em grandezas não proporcionais | teste do "dobro" | se uma criança cresce 10 cm aos 5 anos, não terá 2 m aos 100 |
| 2,25 h = 2 h 25 min | 2 h 15 min | $0{,}25$ h $= 0{,}25 \cdot 60 = 15$ min |

---

## 💻 Conexão com programação e ML

- **Mapear um intervalo em outro** é uma proporção: um valor $x$ entre $[a, b]$ vai para $c + (x - a) \cdot \frac{d - c}{b - a}$ no intervalo $[c, d]$. Serve para converter coordenadas, barras de progresso e animações (o famoso *lerp*).
- **Em ML:**
  - A **normalização min-max** leva cada atributo para $[0, 1]$: $x' = \frac{x - \min}{\max - \min}$. É exatamente a fórmula acima.
  - **Divisão treino/teste** 80 : 20 é uma divisão em partes proporcionais.
  - Num dataset **desbalanceado** (razão 1 : 9 entre classes), um modelo que sempre "chuta" a classe maior acerta 90% sem aprender nada. A razão entre as classes é a primeira coisa a olhar.

---

## 🔗 Conexões
- **Usa:** [[Frações e Equivalência]] (a razão é uma fração), [[Operações com Frações]], [[Números Decimais]].
- **É usado em:** [[Porcentagem]] (razão com denominador 100).
- **Na álgebra:** uma proporção é uma [[Equações do 1º Grau|equação do 1º grau]].
- **Mais adiante:**
  - A proporcionalidade direta $y = kx$ é uma [[Função Afim]] que passa pela origem.
  - [[Congruência e Semelhança]]: triângulos semelhantes têm lados proporcionais.
  - [[Trigonometria no Triângulo Retângulo]]: seno, cosseno e tangente **são razões**.
  - A normalização de dados volta em [[Medidas de Dispersão]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. O que é uma razão? Por que as unidades precisam ser iguais?
2. Enuncie a propriedade fundamental das proporções. De onde ela vem?
3. Como saber se duas grandezas são direta ou inversamente proporcionais? Dê um exemplo de cada.
4. Por que velocidade e tempo são inversamente proporcionais (para a mesma distância)?
5. Explique como montar uma regra de três composta.
6. Divida 90 em partes proporcionais a 1, 2 e 6.
