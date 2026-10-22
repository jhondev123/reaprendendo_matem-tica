---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Equações biquadradas
  - Equações irracionais
  - Equações fracionárias
  - Mudança de variável
tags:
  - algebra
---
# Equações Redutíveis ao 2º Grau

> [!abstract] Em uma frase
> Muitas equações "assustadoras" viram uma [[Equações do 2º Grau|equação do 2º grau]] com o truque certo: **trocar de variável** ($y = x^2$), **fatorar**, **tirar o denominador** ou **elevar ao quadrado**. Nesse último caso, é **obrigatório verificar** as respostas.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Equações do 2º Grau]], [[Frações Algébricas]], [[Expoentes e Radicais com Variáveis]] · **Próximo:** [[Somatório e Produtório]]
**Praticar:** [[Equações Redutíveis ao 2º Grau - Exercícios]] · [[Equações Redutíveis ao 2º Grau - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Resolver equações **biquadradas** com a troca $y = x^2$.
- Usar **mudança de variável** em geral.
- Resolver **equações-produto** e **equações fracionárias** (com condição de existência).
- Resolver **equações irracionais** e **eliminar raízes estranhas**.

---

## 1. Biquadradas: $ax^4 + bx^2 + c = 0$

Repare que $x^4 = (x^2)^2$. Chamando $y = x^2$, a equação vira $ay^2 + by + c = 0$.

> [!example] $x^4 - 5x^2 + 4 = 0$
> 1. Troque: $y = x^2 \Rightarrow y^2 - 5y + 4 = 0$
> 2. Resolva: $(y - 1)(y - 4) = 0 \Rightarrow y = 1$ ou $y = 4$
> 3. **Volte para $x$**: $x^2 = 1 \Rightarrow x = \pm 1$; $\;x^2 = 4 \Rightarrow x = \pm 2$
>
> Solução: $\{-2, -1, 1, 2\}$. Uma biquadrada pode ter **até 4** raízes.

> [!warning] $y$ negativo não gera $x$ real
> Em $x^4 + 3x^2 - 4 = 0$: $y^2 + 3y - 4 = 0 \Rightarrow y = 1$ ou $y = -4$. Como $x^2 = -4$ não tem solução real, sobram só $x = \pm 1$.

## 2. Mudança de variável em geral

Sempre que uma **mesma expressão** aparece repetida, dê um nome a ela.

> [!example] $(x - 1)^2 - 5(x - 1) + 6 = 0$
> Com $y = x - 1$: $y^2 - 5y + 6 = 0 \Rightarrow y = 2$ ou $y = 3$. Voltando: $x - 1 = 2 \Rightarrow x = 3$ e $x - 1 = 3 \Rightarrow x = 4$.

> [!example] $x^{2/3} - 5x^{1/3} + 6 = 0$
> Como $x^{2/3} = (x^{1/3})^2$, use $y = x^{1/3}$: $y^2 - 5y + 6 = 0 \Rightarrow y = 2$ ou $y = 3$. Então $x = 2^3 = 8$ ou $x = 3^3 = 27$.

Essa é uma das ideias mais poderosas da matemática. Ela volta em [[Equações Exponenciais e Logarítmicas]] ($y = 2^x$), em [[Equações Trigonométricas]] ($y = \operatorname{sen} x$) e em [[Integração por Substituição]].

## 3. Equações-produto

Fatore e use o **produto nulo**:
$$x^3 - 4x = 0 \Rightarrow x(x^2 - 4) = 0 \Rightarrow x(x - 2)(x + 2) = 0 \Rightarrow x \in \{0, 2, -2\}$$

## 4. Equações fracionárias ($x$ no denominador)

1. Escreva a **condição de existência** (denominadores $\neq 0$).
2. Multiplique tudo pelo **MMC** dos denominadores.
3. Resolva e **descarte** as soluções que violam a condição.

> [!example] $x + \dfrac{6}{x} = 5$, com $x \neq 0$
> Multiplicando por $x$: $x^2 + 6 = 5x \Rightarrow x^2 - 5x + 6 = 0 \Rightarrow x = 2$ ou $x = 3$. Ambas são diferentes de 0, então valem.

> [!example] $\dfrac{1}{x - 1} + \dfrac{1}{x + 1} = \dfrac{4}{3}$, com $x \neq \pm 1$
> Somando à esquerda ([[Frações Algébricas]]): $\frac{2x}{x^2 - 1} = \frac{4}{3}$. Pela propriedade das proporções: $6x = 4x^2 - 4 \Rightarrow 2x^2 - 3x - 2 = 0 \Rightarrow x = 2$ ou $x = -\frac{1}{2}$. Nenhuma é $\pm 1$, então as duas valem.

## 5. Equações irracionais ($x$ dentro da raiz)

1. **Isole a raiz** num dos lados.
2. **Eleve os dois lados ao quadrado.**
3. Resolva a equação que resultar.
4. **Verifique cada candidato na equação ORIGINAL.**

> [!example] $\sqrt{x + 5} = x - 1$
> 1. A raiz já está isolada.
> 2. Elevando ao quadrado: $x + 5 = (x - 1)^2 = x^2 - 2x + 1$ (cuidado com o [[Produtos Notáveis|produto notável]]!)
> 3. $x^2 - 3x - 4 = 0 \Rightarrow x = 4$ ou $x = -1$
> 4. Verificando:
>    - $x = 4$: $\sqrt{9} = 3$ e $4 - 1 = 3$ ✔️
>    - $x = -1$: $\sqrt{4} = 2$, mas $-1 - 1 = -2$ ❌
>
> Solução: **só $x = 4$**. O $-1$ é uma **raiz estranha**.

> [!danger] Por que aparecem raízes estranhas?
> Elevar ao quadrado **não é reversível**: se $a = b$, então $a^2 = b^2$, mas $a^2 = b^2$ não garante $a = b$ (pode ser $a = -b$). Quando elevamos, "misturamos" a equação $\sqrt{x + 5} = x - 1$ com a equação $-\sqrt{x + 5} = x - 1$, e a solução desta última se infiltra. Por isso, **a verificação faz parte da resolução**: não é opcional.

> [!tip] Duas raízes? Isole uma e eleve duas vezes
> $\sqrt{x + 7} + \sqrt{x} = 7 \Rightarrow \sqrt{x + 7} = 7 - \sqrt{x}$. Elevando: $x + 7 = 49 - 14\sqrt{x} + x \Rightarrow 14\sqrt{x} = 42 \Rightarrow \sqrt{x} = 3 \Rightarrow x = 9$. Verificação: $\sqrt{16} + \sqrt{9} = 7$ ✔️

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: com fração
> $x^4 - 0{,}25x^2 = 0 \Rightarrow x^2\left(x^2 - \frac{1}{4}\right) = 0 \Rightarrow x = 0$ ou $x = \pm\frac{1}{2}$

> [!example] Exemplo 2: com dízima
> $(x^2 - 2)^2 = 0{,}\overline{1} \cdot 9$. Como $0{,}\overline{1} \cdot 9 = \frac{1}{9} \cdot 9 = 1$: $\;x^2 - 2 = \pm 1 \Rightarrow x^2 = 3$ ou $x^2 = 1 \Rightarrow x \in \{\pm\sqrt{3}, \pm 1\}$

> [!example] Exemplo 3: irracional com raiz estranha
> $\sqrt{2x + 1} = x - 1 \Rightarrow 2x + 1 = x^2 - 2x + 1 \Rightarrow x^2 - 4x = 0 \Rightarrow x = 0$ ou $x = 4$.
> Verificando: $x = 0$ dá $\sqrt{1} = 1 \neq -1$ ❌; $x = 4$ dá $\sqrt{9} = 3 = 3$ ✔️. Solução: **$x = 4$**.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| Parar em $y = 1$ e $y = 4$ | voltar para $x$: $x = \pm 1, \pm 2$ | a incógnita era $x$ |
| $x^2 = -4 \Rightarrow x = \pm 2$ | sem solução real | |
| $(\sqrt{x + 5})^2 = (x - 1)^2 \to x + 5 = x^2 + 1$ | $x^2 - 2x + 1$ | $(a - b)^2$ tem o termo do meio |
| Não verificar a equação irracional | **sempre** verifique | raízes estranhas |
| Multiplicar por $x$ e aceitar $x = 0$ | confira a condição de existência | |

---

## 💻 Conexão com programação e ML

- **Verificar candidatos** é fácil em código: resolva, depois filtre com `Math.Abs(ladoEsquerdo(x) - ladoDireito(x)) < 1e-9`. É o que você deveria fazer à mão, automatizado.
- **Em ML, mudar de variável é uma técnica central:**
  - **Engenharia de atributos:** se $y$ depende de $x^2$, crie o atributo $z = x^2$, e um modelo **linear** em $z$ resolve um problema **quadrático** em $x$. É a mesma ideia do $y = x^2$ das biquadradas.
  - Transformar com **logaritmo** ($z = \log x$) deixa dados exponenciais com cara de reta ([[Escalas Logarítmicas]]).
  - O "*reparametrization trick*" dos autoencoders variacionais é, literalmente, uma troca de variável que facilita o treino.

---

## 🔗 Conexões
- **Usa:** [[Equações do 2º Grau]] (o destino de todas), [[Fatoração]] (produto nulo), [[Frações Algébricas]] (MMC e condição), [[Expoentes e Radicais com Variáveis]] e [[Produtos Notáveis]] (elevar ao quadrado corretamente).
- **Mais adiante:** [[Equações Exponenciais e Logarítmicas]], [[Equações Trigonométricas]] e [[Integração por Substituição]], todas com mudança de variável.

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Que troca de variável resolve uma biquadrada? Quantas raízes ela pode ter, no máximo?
2. Resolva $x^4 - 9x^2 = 0$.
3. Por que, numa equação fracionária, é preciso anotar a condição de existência?
4. Quais são os 4 passos para resolver uma equação irracional?
5. Explique, com suas palavras, por que elevar ao quadrado pode criar raízes estranhas.
6. Em $(x^2 + 1)^2 - 3(x^2 + 1) + 2 = 0$, que troca você faria?
