---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Equação quadrática
  - Bhaskara
  - Fórmula de Bhaskara
  - Discriminante
  - Delta
  - Completar quadrado
tags:
  - algebra
---
# Equações do 2º Grau

> [!abstract] Em uma frase
> Uma equação $ax^2 + bx + c = 0$ pode ter **duas, uma ou nenhuma** raiz real. Dá para resolvê-la por **fatoração**, **completando o quadrado** ou pela **fórmula de Bhaskara**, que é só o completar quadrado feito de uma vez para todos os casos.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Fatoração]], [[Produtos Notáveis]], [[Expoentes e Radicais com Variáveis]] · **Próximo:** [[Equações Redutíveis ao 2º Grau]]
**Praticar:** [[Equações do 2º Grau - Exercícios]] · [[Equações do 2º Grau - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Deduzir a fórmula de Bhaskara sozinho no caderno (seção 5)
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Resolver equações **incompletas** sem fórmula.
- Resolver por **fatoração** (soma e produto) e por **completar o quadrado**.
- Usar a **fórmula de Bhaskara** e o **discriminante** $\Delta$ para saber quantas raízes existem.
- Usar as relações de **soma e produto** das raízes.
- Montar e resolver problemas que levam a uma equação do 2º grau.

---

## 1. A forma geral

$$ax^2 + bx + c = 0, \qquad a \neq 0$$

| Equação | $a$ | $b$ | $c$ |
|---|---|---|---|
| $3x^2 - 5x + 2 = 0$ | 3 | −5 | 2 |
| $x^2 - 9 = 0$ | 1 | 0 | −9 |
| $-x^2 + 4x = 0$ | −1 | 4 | 0 |

> [!warning] Os coeficientes levam o sinal
> Em $3x^2 - 5x + 2$, $b = -5$ (e não 5). Errar esse sinal é o erro mais comum na fórmula de Bhaskara.

## 2. A ideia-chave: produto nulo

> [!important] Se um produto é zero, um dos fatores é zero
> $$A \cdot B = 0 \iff A = 0 \text{ ou } B = 0$$
> Por isso [[Fatoração|fatorar]] resolve equações: $(x - 2)(x - 3) = 0 \Rightarrow x = 2$ ou $x = 3$.

## 3. Equações incompletas (sem fórmula)

**Sem o termo em $x$ ($b = 0$):** isole o $x^2$ e tire a raiz, **lembrando do $\pm$**.
$$x^2 - 25 = 0 \Rightarrow x^2 = 25 \Rightarrow x = \pm 5$$
$$x^2 + 4 = 0 \Rightarrow x^2 = -4 \Rightarrow \text{sem raiz real}$$

**Sem o termo independente ($c = 0$):** coloque o $x$ em evidência.
$$x^2 - 7x = 0 \Rightarrow x(x - 7) = 0 \Rightarrow x = 0 \text{ ou } x = 7$$

> [!danger] Nunca "corte" o $x$ dividindo
> $x^2 = 7x \Rightarrow x = 7$ **perde** a raiz $x = 0$. Dividir por $x$ só é permitido quando se sabe que $x \neq 0$. Em vez de dividir, passe tudo para um lado e coloque em evidência.

## 4. Por fatoração (soma e produto)

Quando $a = 1$ e as raízes são inteiras, procure dois números com **soma $-b$** e **produto $c$** (ou fatore o trinômio, como no caso 5 da [[Fatoração]]):
$$x^2 - 5x + 6 = 0 \Rightarrow (x - 2)(x - 3) = 0 \Rightarrow x = 2 \text{ ou } x = 3$$

## 5. Completando o quadrado (e de onde vem Bhaskara)

**Ideia:** transformar o lado com $x$ num [[Produtos Notáveis|quadrado perfeito]] $(x + k)^2$ e depois tirar a raiz.

> [!example] $x^2 + 6x - 7 = 0$
> 1. Passe o número para o outro lado: $x^2 + 6x = 7$.
> 2. $x^2 + 6x$ é o começo de $(x + 3)^2 = x^2 + 6x + 9$ (a metade de 6 é 3). Some 9 dos dois lados: $x^2 + 6x + 9 = 16$.
> 3. Escreva como quadrado: $(x + 3)^2 = 16$.
> 4. Tire a raiz, com $\pm$: $x + 3 = \pm 4 \Rightarrow x = 1$ ou $x = -7$.

> [!question]- A dedução da fórmula de Bhaskara (faça no caderno!)
> Começando de $ax^2 + bx + c = 0$:
> 1. Divida tudo por $a$: $\;x^2 + \frac{b}{a}x = -\frac{c}{a}$
> 2. Some $\left(\frac{b}{2a}\right)^2$ dos dois lados (a metade do coeficiente do $x$, ao quadrado): $\;x^2 + \frac{b}{a}x + \frac{b^2}{4a^2} = \frac{b^2}{4a^2} - \frac{c}{a}$
> 3. O lado esquerdo é um quadrado; à direita, use o denominador comum $4a^2$: $\;\left(x + \frac{b}{2a}\right)^2 = \frac{b^2 - 4ac}{4a^2}$
> 4. Tire a raiz, com $\pm$: $\;x + \frac{b}{2a} = \pm\frac{\sqrt{b^2 - 4ac}}{2a}$
> 5. Isole o $x$: $\;x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a}$
>
> Não é uma fórmula mágica: é o completar quadrado feito com letras.

## 6. A fórmula de Bhaskara

$$x = \frac{-b \pm \sqrt{\Delta}}{2a}, \qquad \Delta = b^2 - 4ac$$

> [!example] $2x^2 - 3x - 2 = 0$
> 1. $a = 2$, $b = -3$, $c = -2$
> 2. $\Delta = (-3)^2 - 4 \cdot 2 \cdot (-2) = 9 + 16 = 25$
> 3. $x = \dfrac{-(-3) \pm \sqrt{25}}{2 \cdot 2} = \dfrac{3 \pm 5}{4}$
> 4. $x_1 = \frac{8}{4} = 2$ e $x_2 = \frac{-2}{4} = -\frac{1}{2}$
>
> Verificação: $2 \cdot 4 - 6 - 2 = 0$ ✔️

**O discriminante $\Delta$ diz quantas raízes reais existem:**

| $\Delta$ | Raízes reais | Por quê |
|---|---|---|
| $\Delta > 0$ | **duas** diferentes | $\pm\sqrt{\Delta}$ dá dois valores |
| $\Delta = 0$ | **uma** (raiz dupla) | $\pm 0$ é o mesmo valor |
| $\Delta < 0$ | **nenhuma** | não existe raiz real de número negativo ([[Radiciação]]) |

> [!tip] Ordem de prioridade
> 1. É incompleta? Resolva direto (seção 3).
> 2. Dá para fatorar de cabeça? Fatore (seção 4).
> 3. Senão, Bhaskara. Mas antes, se puder, **simplifique**: divida tudo por um fator comum e tire frações e decimais multiplicando pelo MMC.

## 7. Soma e produto das raízes (relações de Girard)

$$x_1 + x_2 = -\frac{b}{a} \qquad x_1 \cdot x_2 = \frac{c}{a}$$

Servem para conferir respostas, achar raízes de cabeça e responder perguntas **sem resolver** a equação. E a **forma fatorada** é:
$$ax^2 + bx + c = a(x - x_1)(x - x_2)$$

> [!question]- Tente agora (clique para ver as respostas)
> (a) Resolva $x^2 - 2x - 1 = 0$. (b) Sem resolver, qual é a soma das raízes de $2x^2 - 8x + 3 = 0$? E o produto?
> **Respostas:** (a) $\Delta = 8$, então $x = \frac{2 \pm 2\sqrt{2}}{2} = 1 \pm \sqrt{2}$ (b) soma $= 4$; produto $= \frac{3}{2}$

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: com frações
> $\frac{x^2}{2} - \frac{x}{3} - \frac{1}{6} = 0$. Multiplicando por 6: $3x^2 - 2x - 1 = 0$. $\Delta = 4 + 12 = 16$, então $x = \frac{2 \pm 4}{6}$: $x = 1$ ou $x = -\frac{1}{3}$.

> [!example] Exemplo 2: com raízes nos coeficientes
> $x^2 - 2\sqrt{3}\,x + 3 = 0$. Repare que é $(x - \sqrt{3})^2 = 0$ (o [[Produtos Notáveis|quadrado da diferença]]). Então $x = \sqrt{3}$ (raiz dupla; confira que $\Delta = 12 - 12 = 0$).

> [!example] Exemplo 3: problema
> Um retângulo tem área de 60 m², e um lado mede 4 m a mais que o outro. Quais são as medidas?
> $x(x + 4) = 60 \Rightarrow x^2 + 4x - 60 = 0 \Rightarrow (x + 10)(x - 6) = 0$. Como medida não é negativa, $x = 6$: **6 m por 10 m**.
> ⚠️ Nos problemas, descarte as raízes que não fazem sentido no contexto.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $x^2 = 9 \Rightarrow x = 3$ | $x = \pm 3$ | $(-3)^2$ também dá 9 |
| $x^2 = 5x \Rightarrow x = 5$ | $x = 0$ ou $x = 5$ | não divida por $x$ |
| Com $b = -5$: $-b = -5$ | $-b = 5$ | o menos de $-b$ troca o sinal |
| $\Delta = -5^2 - 4ac$ com $b = -5$ | $(-5)^2 = 25$ | o quadrado de $b$ é **sempre** positivo |
| $x = -b \pm \frac{\sqrt{\Delta}}{2a}$ | $\frac{-b \pm \sqrt{\Delta}}{2a}$ | o $2a$ divide o numerador **inteiro** |
| $\Delta < 0 \Rightarrow$ "a raiz é negativa" | **não há** raiz real | |

---

## 💻 Conexão com programação e ML

- **Bhaskara em código** é direto, mas precisa tratar os casos: $a = 0$ (não é do 2º grau), $\Delta < 0$ (sem raízes reais) e $\Delta = 0$ (uma raiz).
- **Curiosidade numérica:** quando $b^2$ é muito maior que $4ac$, a conta $-b + \sqrt{\Delta}$ subtrai dois números quase iguais e perde precisão no `double`. Bibliotecas sérias usam $x_1 = \frac{-b - \text{sinal}(b)\sqrt{\Delta}}{2a}$ e $x_2 = \frac{c}{a\,x_1}$ (a relação do produto!).
- **Em ML:** o erro quadrático de um modelo $\hat{y} = wx$ com um único dado é $(y - wx)^2 = x^2w^2 - 2xyw + y^2$, uma expressão **do 2º grau em $w$**. Treinar é achar o $w$ que deixa esse erro **mínimo**: o vértice de uma parábola ([[Função Quadrática]] e [[Otimização (Máximos e Mínimos)]]).

---

## 🔗 Conexões
- **Usa:** [[Fatoração]] (produto nulo), [[Produtos Notáveis]] (completar o quadrado), [[Radiciação]] e [[Expoentes e Radicais com Variáveis]] (simplificar $\sqrt{\Delta}$), [[Equações do 1º Grau]].
- **É usado em:** [[Equações Redutíveis ao 2º Grau]].
- **Mais adiante:**
  - [[Função Quadrática]]: as raízes são onde a parábola cruza o eixo $x$, e $\Delta$ diz quantas vezes ela cruza.
  - [[Otimização (Máximos e Mínimos)]]: achar o mínimo de um erro.
  - [[Autovalores e Autovetores]]: para matrizes 2×2, achar os autovalores é resolver uma equação do 2º grau.

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Por que fatorar resolve equações? Enuncie a propriedade do produto nulo.
2. Resolva $3x^2 - 12 = 0$ e $3x^2 - 12x = 0$ sem fórmula.
3. Complete o quadrado para resolver $x^2 - 4x - 5 = 0$.
4. Escreva a fórmula de Bhaskara e explique de onde ela vem.
5. O que o $\Delta$ informa? Dê um exemplo de equação com $\Delta < 0$.
6. Quais são a soma e o produto das raízes de $ax^2 + bx + c = 0$?
7. Por que não se pode dividir $x^2 = 3x$ por $x$?
