---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Equação do primeiro grau
  - Equações lineares
  - Isolar a variável
tags:
  - algebra
---
# Equações do 1º Grau

> [!abstract] Em uma frase
> Uma equação é uma **balança em equilíbrio**: o que você fizer de um lado, faça do outro. O objetivo é deixar o $x$ **sozinho**, desfazendo as operações de trás para a frente.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Linguagem Algébrica]], [[Frações Algébricas]], [[Treino Misto - Lista 4]] · **Próximo:** [[Inequações do 1º Grau]]
**Praticar:** [[Equações do 1º Grau - Exercícios]] · [[Equações do 1º Grau - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Fazer o bloco 🔀 de equações com frações, decimais, dízimas e raízes
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Resolver equações do 1º grau com parênteses, frações, decimais, dízimas e raízes.
- Entender o que "passar para o outro lado" **realmente** significa.
- **Isolar uma variável** numa fórmula.
- Reconhecer equações **sem solução** e com **infinitas soluções**.
- Transformar um problema em equação, resolver e **verificar**.

---

## 1. O que é uma equação

$$2x + 3 = 11$$

É uma **igualdade** com uma incógnita. **Resolver** é achar o valor de $x$ que torna a igualdade verdadeira (a **solução**, ou **raiz**). Aqui, $x = 4$, porque $2 \cdot 4 + 3 = 11$ ✔️.

É de **1º grau** porque o maior expoente do $x$ é 1. Toda equação desse tipo pode ser arrumada na forma $ax + b = 0$, com $a \neq 0$, cuja solução é $x = -\frac{b}{a}$.

## 2. A balança

Imagine $2x + 3 = 11$ como uma balança equilibrada: de um lado, duas caixas misteriosas e 3 pesinhos; do outro, 11 pesinhos.

| Passo | Na balança | Na equação |
|---|---|---|
| Tire 3 pesinhos **dos dois lados** | continua equilibrada | $2x + 3 - 3 = 11 - 3 \Rightarrow 2x = 8$ |
| Divida **os dois lados** ao meio | continua equilibrada | $\frac{2x}{2} = \frac{8}{2} \Rightarrow x = 4$ |

> [!important] A única regra
> Você pode **somar, subtrair, multiplicar ou dividir os dois lados** pelo mesmo número (menos dividir por zero), e a igualdade continua verdadeira.

> [!tip] "Passar para o outro lado" é um atalho
> - "O $+3$ **passa subtraindo**" é o mesmo que subtrair 3 dos dois lados.
> - "O 2 que multiplica **passa dividindo**" é o mesmo que dividir os dois lados por 2.
>
> O atalho é ótimo, **desde que você saiba de onde ele vem**. Quando bater a dúvida, volte à balança.

## 3. O método, passo a passo

1. **Tire os parênteses** (distributiva, cuidado com os sinais).
2. **Tire os denominadores**: multiplique **todos os termos** dos dois lados pelo MMC dos denominadores.
3. **Junte**: termos com $x$ de um lado, números do outro.
4. **Divida** pelo coeficiente do $x$.
5. **Verifique**, substituindo na equação **original**.

> [!example] Exemplo completo
> $$4(x - 2) = 3x + 1$$
> 1. $4x - 8 = 3x + 1$
> 2. (não há denominadores)
> 3. $4x - 3x = 1 + 8 \Rightarrow x = 9$
> 4. (o coeficiente já é 1)
> 5. Verificação: $4(9 - 2) = 28$ e $3 \cdot 9 + 1 = 28$ ✔️

## 4. Equações com frações

Multiplique **cada termo** pelo MMC dos denominadores. As frações somem.

> [!example] $\dfrac{x}{2} + \dfrac{x}{3} = 10$
> MMC(2, 3) = 6. Multiplicando **tudo** por 6: $3x + 2x = 60 \Rightarrow 5x = 60 \Rightarrow x = 12$.
> Verificação: $6 + 4 = 10$ ✔️

> [!example] $\dfrac{x - 1}{3} - \dfrac{x + 2}{4} = \dfrac{1}{6}$
> MMC(3, 4, 6) = 12. Multiplicando:
> $$4(x - 1) - 3(x + 2) = 2$$
> ⚠️ O traço de fração é um parêntese: o $-3$ multiplica o $(x + 2)$ **inteiro**.
> $$4x - 4 - 3x - 6 = 2 \Rightarrow x - 10 = 2 \Rightarrow x = 12$$

## 5. Equações com decimais, dízimas e raízes

Aqui entra a aritmética mista que você treinou no [[Treino Misto de Aritmética]].

> [!example] Decimais: multiplique por 10, 100…
> $0{,}3x + 1{,}2 = 0{,}5x - 0{,}4$. Multiplicando tudo por 10:
> $$3x + 12 = 5x - 4 \Rightarrow 16 = 2x \Rightarrow x = 8$$

> [!example] Dízimas: transforme em fração antes
> $0{,}\overline{3}x + \frac{1}{2} = 1$. Como $0{,}\overline{3} = \frac{1}{3}$:
> $$\frac{x}{3} + \frac{1}{2} = 1 \;\xrightarrow{\times 6}\; 2x + 3 = 6 \Rightarrow x = \frac{3}{2}$$

> [!example] Raízes no coeficiente: trate a raiz como um número
> $\sqrt{2}\,x + 3 = 5 \Rightarrow \sqrt{2}\,x = 2 \Rightarrow x = \frac{2}{\sqrt{2}} = \frac{2\sqrt{2}}{2} = \sqrt{2}$ (com a [[Radiciação#6. Racionalização (raiz fora do denominador)|racionalização]]).
> $x\sqrt{3} - \sqrt{12} = 0 \Rightarrow x\sqrt{3} = 2\sqrt{3} \Rightarrow x = 2$

> [!example] $x$ no denominador: anote a condição
> $\frac{3}{x} + \frac{1}{2} = 2$, com $x \neq 0$. Então $\frac{3}{x} = \frac{3}{2}$, ou seja, $x = 2$ ✔️ (e $2 \neq 0$, então vale).

## 6. Isolando uma variável numa fórmula

É a **mesma técnica**, mas com letras no lugar dos números. É uma das habilidades mais usadas em física, finanças e ML.

| Fórmula | Isolar | Resultado |
|---|---|---|
| $F = 1{,}8C + 32$ | $C$ | $C = \dfrac{F - 32}{1{,}8}$ |
| $v = \dfrac{d}{t}$ | $t$ | $t = \dfrac{d}{v}$ |
| $y = wx + b$ | $x$ | $x = \dfrac{y - b}{w}$ |
| $A = \dfrac{b \cdot h}{2}$ | $h$ | $h = \dfrac{2A}{b}$ |

## 7. Casos especiais

Às vezes, o $x$ desaparece:
- **Sem solução:** $2(x + 3) - 3(x - 1) = 5 - x \Rightarrow -x + 9 = 5 - x \Rightarrow 9 = 5$, que é falso. Nenhum $x$ funciona.
- **Infinitas soluções:** $3(x - 2) + 6 = 3x \Rightarrow 3x = 3x$, que é sempre verdade. **Todo** $x$ funciona.

## 8. Resolvendo problemas

1. **Leia** e sublinhe o que é pedido.
2. **Dê nome** à incógnita ("seja $x$ a idade do filho").
3. **Traduza** o texto em equação ([[Linguagem Algébrica#4. Traduzindo português ↔ álgebra|tradução]]).
4. **Resolva** e **verifique no texto**, não só na equação.
5. **Responda** com uma frase, com a unidade.

> [!example] Idades
> O pai tem o triplo da idade do filho. Daqui a 12 anos, terá o dobro. Quais são as idades?
> Filho: $x$; pai: $3x$. Daqui a 12 anos: $3x + 12 = 2(x + 12)$, ou seja, $3x + 12 = 2x + 24$, e $x = 12$.
> **O filho tem 12 anos e o pai, 36.** Verificando: daqui a 12 anos, 48 é o dobro de 24 ✔️.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $\frac{x}{2} + 3 = 5 \to x + 3 = 10$ | $x + 6 = 10$ | o MMC multiplica **todos** os termos |
| $2x = 6 \to x = 6 - 2$ | $x = \frac{6}{2} = 3$ | o 2 multiplica, então "passa dividindo" |
| $-\frac{x - 3}{2}$ vira $\frac{-x - 3}{2}$ | $\frac{-x + 3}{2}$ | o menos pega o numerador inteiro |
| $-3x = 12 \to x = 4$ | $x = -4$ | divide-se pelo coeficiente **com o sinal** |
| Achar $x$ e não verificar | verifique sempre | é a forma mais barata de pegar um erro |

---

## 💻 Conexão com programação e ML

- Resolver $ax + b = c$ em código é **uma linha**: `x = (c - b) / a`. A matemática está em chegar a essa fórmula, e em tratar o caso $a = 0$ (sem solução ou infinitas soluções).
- **Em ML:**
  - Isolar uma variável é "inverter" um modelo. Se $\hat{y} = 0{,}8x + 1{,}5$, que entrada $x$ produz $\hat{y} = 9{,}5$? $x = \frac{9{,}5 - 1{,}5}{0{,}8} = 10$.
  - Na regressão linear "de verdade", os melhores pesos saem de **resolver equações** (as *equações normais*). Com uma variável só, é uma equação do 1º grau; com várias, um sistema ([[Sistemas de Equações]]).

---

## 🔗 Conexões
- **Usa:** [[Linguagem Algébrica]] (traduzir), [[Monômios e Polinômios]] (reduzir termos), [[Operações com Frações]] e [[Frações Algébricas]] (o MMC), [[Números Decimais]] e [[Radiciação]] (coeficientes "feios"), [[Treino Misto - Lista 4]] (desfazer operações).
- **É usado em:** [[Inequações do 1º Grau]] (quase igual, com uma diferença importante), [[Sistemas de Equações]] (várias equações juntas), [[Equações do 2º Grau]].
- **Mais adiante:** [[Função Afim]] (a raiz de $ax + b = 0$ é onde a reta cruza o eixo $x$), [[Equações Exponenciais e Logarítmicas]] e [[Equações Trigonométricas]], que sempre terminam numa equação simples como esta.

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Explique, com a balança, por que podemos subtrair 5 dos dois lados de uma equação.
2. O que significa, de verdade, "o 3 passa dividindo"?
3. Quais são os 5 passos do método?
4. Resolva $\frac{x}{4} - \frac{1}{2} = \frac{x}{6}$. Qual é o MMC?
5. Como resolver uma equação que tem $0{,}\overline{6}$ como coeficiente?
6. Isole $r$ em $C = 2\pi r$.
7. Quando uma equação não tem solução? E quando tem infinitas?
