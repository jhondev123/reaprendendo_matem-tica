---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Frações com letras
  - Simplificação algébrica
  - Condição de existência
tags:
  - algebra
---
# Frações Algébricas

> [!abstract] Em uma frase
> Frações com letras seguem **exatamente as mesmas regras** das [[Operações com Frações|frações numéricas]]. A diferença é que, para simplificar e achar o denominador comum, você precisa **fatorar** primeiro, e o denominador nunca pode valer zero.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Fatoração]], [[Operações com Frações]], [[MMC e MDC]] · **Próximo:** [[Equações do 1º Grau]]
**Praticar:** [[Frações Algébricas - Exercícios]] · [[Frações Algébricas - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Dizer para quais valores uma fração algébrica **existe**.
- **Simplificar** fatorando e cortando **fatores** (nunca parcelas).
- Multiplicar, dividir, somar e subtrair frações algébricas.

---

## 1. Condição de existência

$\frac{3}{x - 2}$ só existe se $x - 2 \neq 0$, ou seja, $x \neq 2$. Em $x = 2$, o denominador valeria zero, e [[Operações Fundamentais#7. Por que não se divide por zero|não se divide por zero]].

| Fração | Condição |
|---|---|
| $\frac{3}{x - 2}$ | $x \neq 2$ |
| $\frac{x + 1}{x^2 - 9}$ | $x^2 - 9 \neq 0 \Rightarrow x \neq 3$ e $x \neq -3$ |
| $\frac{5}{x(x + 4)}$ | $x \neq 0$ e $x \neq -4$ |

> [!tip] Fatorar ajuda aqui também
> Com o denominador fatorado, cada fator vira uma condição: $x(x + 4) = 0$ quando $x = 0$ **ou** $x = -4$.

## 2. Simplificar: fatore, depois corte

O mesmo princípio de $\frac{6}{8} = \frac{2 \cdot 3}{2 \cdot 4} = \frac{3}{4}$: só se cortam **fatores** que multiplicam o numerador **inteiro** e o denominador **inteiro**.

> [!example] Passo a passo
> $$\frac{x^2 - 9}{x^2 + 3x}$$
> 1. Fatore em cima: $x^2 - 9 = (x + 3)(x - 3)$
> 2. Fatore embaixo: $x^2 + 3x = x(x + 3)$
> 3. Corte o fator comum $(x + 3)$:
> $$\frac{(x + 3)(x - 3)}{x(x + 3)} = \frac{x - 3}{x} \qquad (x \neq 0,\; x \neq -3)$$

> [!danger] O erro nº 1 da álgebra
> $$\frac{x + 3}{x} \neq 3 \qquad \frac{x + 2}{x + 5} \neq \frac{2}{5}$$
> O $x$ em $x + 3$ é uma **parcela**, não um fator. Teste com $x = 1$: $\frac{1 + 3}{1} = 4$, e não 3. **Na dúvida, teste com um número.**
> (Você viu esse alerta pela primeira vez em [[Frações e Equivalência]].)

**Truque de sinal:** $b - a = -(a - b)$. Então $\frac{a - b}{b - a} = -1$ e
$$\frac{x^2 - 3x}{9 - x^2} = \frac{x(x - 3)}{(3 - x)(3 + x)} = \frac{x(x - 3)}{-(x - 3)(x + 3)} = -\frac{x}{x + 3}$$

## 3. Multiplicar e dividir

Fatore tudo, corte o que for possível e multiplique.

$$\frac{x^2 - 1}{x + 3} \cdot \frac{2x + 6}{x - 1} = \frac{(x + 1)(x - 1)}{x + 3} \cdot \frac{2(x + 3)}{x - 1} = 2(x + 1)$$

Dividir é multiplicar pelo **inverso** da segunda:
$$\frac{4}{x} \div \frac{2}{x^2} = \frac{4}{x} \cdot \frac{x^2}{2} = 2x$$

## 4. Somar e subtrair

Igual a $\frac{1}{2} + \frac{1}{3}$: encontre um **denominador comum** (o MMC dos denominadores **fatorados**) e ajuste cada numerador.

> [!example] $\dfrac{1}{x} + \dfrac{1}{x + 1}$
> Os denominadores $x$ e $x + 1$ não têm fator comum, então o MMC é o produto $x(x + 1)$.
> $$\frac{1 \cdot (x + 1)}{x(x + 1)} + \frac{1 \cdot x}{x(x + 1)} = \frac{x + 1 + x}{x(x + 1)} = \frac{2x + 1}{x(x + 1)}$$

> [!example] $\dfrac{2}{x - 1} - \dfrac{1}{x + 1}$
> $$\frac{2(x + 1) - 1 \cdot (x - 1)}{(x - 1)(x + 1)} = \frac{2x + 2 - x + 1}{x^2 - 1} = \frac{x + 3}{x^2 - 1}$$
> ⚠️ O sinal de menos vale para o numerador **inteiro** da segunda fração: $-(x - 1) = -x + 1$.

> [!example] Com fatores repetidos
> $\frac{1}{x^2 - 4} + \frac{1}{x + 2}$: como $x^2 - 4 = (x + 2)(x - 2)$, o MMC é $(x + 2)(x - 2)$ (e não o produto de tudo).
> $$\frac{1 + (x - 2)}{(x + 2)(x - 2)} = \frac{x - 1}{x^2 - 4}$$

> [!question]- Tente agora (clique para ver as respostas)
> (a) Simplifique $\frac{x^2 + 5x + 6}{x + 2}$. (b) Calcule $\frac{3}{x} - \frac{2}{x^2}$.
> **Respostas:** (a) $\frac{(x + 2)(x + 3)}{x + 2} = x + 3$ (b) $\frac{3x - 2}{x^2}$

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: com decimais
> $\frac{0{,}5x + 1}{x + 2} = \frac{0{,}5(x + 2)}{x + 2} = 0{,}5 = \frac{1}{2}$ (para $x \neq -2$)

> [!example] Exemplo 2: fração de frações
> $$\frac{1 - \frac{1}{x}}{1 - \frac{1}{x^2}} = \frac{\frac{x - 1}{x}}{\frac{x^2 - 1}{x^2}} = \frac{x - 1}{x} \cdot \frac{x^2}{(x - 1)(x + 1)} = \frac{x}{x + 1}$$

> [!example] Exemplo 3: com frações nos termos
> $$\left(\frac{x}{2} - \frac{1}{3}\right) \div \frac{x}{6} = \frac{3x - 2}{6} \cdot \frac{6}{x} = \frac{3x - 2}{x}$$

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $\frac{x + 3}{x} = 3$ | $1 + \frac{3}{x}$ | não se cortam parcelas |
| $\frac{x^2 - 9}{x - 3} = x - 3$ | $x + 3$ | fatore: $(x + 3)(x - 3)$ |
| $\frac{1}{a} + \frac{1}{b} = \frac{1}{a + b}$ | $\frac{a + b}{ab}$ | precisa de denominador comum |
| $\frac{2}{x - 1} - \frac{x - 3}{x - 1} = \frac{2 - x - 3}{x - 1}$ | $\frac{2 - x + 3}{x - 1}$ | o menos pega o numerador inteiro |
| Esquecer a condição de existência | anote $x \neq \dots$ | ela some na simplificação, mas continua valendo |

---

## 💻 Conexão com programação e ML

- **"Simplificar" pode esconder um buraco.** $\frac{x^2 - 9}{x + 3}$ e $x - 3$ são iguais para **todo** $x \neq -3$. Em $x = -3$, a primeira dá `0.0 / 0.0 = NaN` no C#, enquanto a segunda dá $-6$. Bugs de "divisão por zero que sumiu na simplificação" são reais.
- **Em ML:** a **sigmoide**, $\sigma(x) = \frac{1}{1 + e^{-x}}$, é uma fração algébrica. Manipulações como as desta nota mostram que a derivada dela é $\sigma(x)\,(1 - \sigma(x))$, um resultado que torna o treino de redes neurais barato. Agendas de taxa de aprendizado como $\alpha_t = \frac{\alpha_0}{1 + kt}$ também são frações algébricas.

---

## 🔗 Conexões
- **Usa:** [[Fatoração]] (sempre o primeiro passo), [[Operações com Frações]] (as mesmas regras), [[MMC e MDC]] (o denominador comum), [[Frações e Equivalência]] (só se cortam fatores).
- **É usado em:** [[Equações do 1º Grau]] e [[Equações Redutíveis ao 2º Grau]] (equações com $x$ no denominador).
- **Mais adiante:** [[Propriedades e Cálculo de Limites]] (os limites $\frac{0}{0}$ são frações algébricas), [[Regras de Derivação]] (a regra do quociente) e [[Integral Indefinida]] (frações parciais, como no 🔴 2).

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Qual é a condição de existência de $\frac{x}{x^2 - 16}$?
2. Por que $\frac{x + 5}{5} \neq x$? Como mostrar isso com um número?
3. Simplifique $\frac{x^2 - 4}{x^2 - 4x + 4}$.
4. Como achar o denominador comum de $\frac{1}{x^2 - 1}$ e $\frac{1}{x - 1}$?
5. Calcule $\frac{1}{x} - \frac{1}{x + 2}$.
6. Por que a condição de existência continua valendo depois de simplificar?
