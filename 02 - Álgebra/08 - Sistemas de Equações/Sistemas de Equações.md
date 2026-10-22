---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Sistemas lineares 2x2
  - Método da substituição
  - Método da adição
tags:
  - algebra
---
# Sistemas de Equações

> [!abstract] Em uma frase
> Com **duas incógnitas**, você precisa de **duas equações**. Resolver o sistema é achar o par $(x, y)$ que satisfaz **as duas ao mesmo tempo**, e geometricamente é o ponto onde **duas retas se cruzam**.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Equações do 1º Grau]] · **Próximo:** [[Expoentes e Radicais com Variáveis]]
**Praticar:** [[Sistemas de Equações - Exercícios]] · [[Sistemas de Equações - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Resolver sistemas 2×2 pelos métodos da **substituição** e da **adição**.
- Escolher o método mais rápido para cada sistema.
- Reconhecer sistemas **sem solução** e com **infinitas soluções**, e interpretá-los com retas.
- Montar sistemas a partir de problemas.

---

## 1. Por que duas equações?

"2 cafés e 1 pão custam R\$ 13." Isso tem muitas possibilidades: café a 5 e pão a 3? Café a 6 e pão a 1? Com **uma** equação e **duas** incógnitas, não dá para decidir.

Com uma segunda informação, "1 café e 3 pães custam R\$ 14", só **um** par funciona para as duas:
$$\begin{cases} 2c + p = 13 \\ c + 3p = 14 \end{cases} \qquad \Rightarrow \qquad c = 5, \; p = 3$$

Verificação: $2 \cdot 5 + 3 = 13$ ✔️ e $5 + 3 \cdot 3 = 14$ ✔️. **Verifique sempre nas duas.**

## 2. Método da substituição

1. **Isole** uma incógnita numa das equações (de preferência uma com coeficiente 1).
2. **Substitua** na outra equação, **entre parênteses**. Sobra uma equação com uma incógnita só.
3. Resolva e **volte** para achar a outra.

> [!example] $\begin{cases} x + y = 10 \\ x - y = 4 \end{cases}$
> 1. Da primeira: $x = 10 - y$.
> 2. Na segunda: $(10 - y) - y = 4 \Rightarrow 10 - 2y = 4 \Rightarrow y = 3$.
> 3. Voltando: $x = 10 - 3 = 7$.
>
> Solução: $(7, 3)$.

## 3. Método da adição (eliminação)

1. Multiplique as equações (se precisar) para que uma incógnita fique com **coeficientes opostos**.
2. **Some** as equações: essa incógnita some.
3. Resolva e volte para achar a outra.

> [!example] $\begin{cases} 2x + 3y = 13 \\ 3x - 2y = 0 \end{cases}$
> Para eliminar o $y$, multiplique a 1ª por 2 e a 2ª por 3:
> $$\begin{cases} 4x + 6y = 26 \\ 9x - 6y = 0 \end{cases} \;\xrightarrow{\text{somando}}\; 13x = 26 \Rightarrow x = 2$$
> Voltando à 1ª: $4 + 3y = 13 \Rightarrow y = 3$. Solução: $(2, 3)$.

> [!tip] Qual método usar?
> - Alguma incógnita tem **coeficiente 1** (ou já está isolada)? → **substituição**.
> - Os coeficientes já são **opostos** ou fáceis de igualar? → **adição**.
> - Na dúvida, a **adição** costuma gerar menos frações.

## 4. As três situações possíveis (com retas)

Cada equação do 1º grau com duas incógnitas é uma **reta** no plano. Resolver o sistema é achar onde as retas se encontram.

| Situação | Nas contas | Nas retas | Nome |
|---|---|---|---|
| **Uma** solução | chega-se a $x = \dots$, $y = \dots$ | se cruzam num ponto | possível e determinado (SPD) |
| **Nenhuma** solução | aparece algo falso, como $0 = 2$ | **paralelas** | impossível (SI) |
| **Infinitas** soluções | aparece $0 = 0$ | **a mesma reta** | possível e indeterminado (SPI) |

> [!example] Os casos especiais
> - $\begin{cases} x + y = 5 \\ x + y = 7 \end{cases}$: subtraindo, $0 = 2$. **Impossível**: dois números não podem somar 5 e 7 ao mesmo tempo.
> - $\begin{cases} x + 2y = 4 \\ 2x + 4y = 8 \end{cases}$: a 2ª é a 1ª multiplicada por 2. É a mesma informação duas vezes, então há **infinitas** soluções.

Você vai desenhar essas retas em [[Plano Cartesiano]] e [[Equação da Reta]].

## 5. Montando sistemas a partir de problemas

> [!example] Carros e motos
> Num estacionamento há 40 veículos (carros e motos) e 130 rodas. Quantos são de cada?
> $$\begin{cases} c + m = 40 \\ 4c + 2m = 130 \end{cases}$$
> Multiplicando a 1ª por $-2$ e somando: $2c = 50 \Rightarrow c = 25$, então $m = 15$.
> **São 25 carros e 15 motos.** (Verificação: $100 + 30 = 130$ rodas ✔️)

Lembra do problema da prova com acertos e erros em [[Números Inteiros - Exercícios|Números Inteiros]]? Ele é um sistema: $a + e = 17$ e $5a - 2e = 50$.

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: com frações
> $\begin{cases} \frac{x}{2} + \frac{y}{3} = 4 \\ x - y = 3 \end{cases}$
> Tire as frações da 1ª (multiplicando por 6): $3x + 2y = 24$. Da 2ª: $x = y + 3$.
> Substituindo: $3(y + 3) + 2y = 24 \Rightarrow 5y = 15 \Rightarrow y = 3$, e então $x = 6$.

> [!example] Exemplo 2: com decimais
> $\begin{cases} 0{,}2x + 0{,}5y = 1{,}9 \\ x + y = 5 \end{cases}$
> Multiplicando a 1ª por 10: $2x + 5y = 19$. Com $x = 5 - y$: $10 - 2y + 5y = 19 \Rightarrow y = 3$, e $x = 2$.

> [!example] Exemplo 3: com raízes
> $\begin{cases} \sqrt{2}\,x + y = 3 \\ \sqrt{2}\,x - y = 1 \end{cases}$
> Somando: $2\sqrt{2}\,x = 4 \Rightarrow x = \frac{4}{2\sqrt{2}} = \frac{2}{\sqrt{2}} = \sqrt{2}$. Então $y = 3 - \sqrt{2} \cdot \sqrt{2} = 3 - 2 = 1$.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| Substituir $x = 10 - y$ em $x - y$ como $10 - y - y$ **sem perceber** o que fez | escreva $(10 - y) - y$ | os parênteses evitam erros de sinal |
| Somar as equações sem igualar os coeficientes | primeiro deixe um par de coeficientes opostos | senão nada some |
| Subtrair as equações e errar o sinal de um termo | prefira multiplicar por $-1$ e **somar** | |
| Achar $x$ e esquecer o $y$ | a resposta é o **par** $(x, y)$ | |
| Verificar só numa equação | verifique nas **duas** | |

---

## 💻 Conexão com programação e ML

- **Regra de Cramer (2×2):** para $\begin{cases} a_1x + b_1y = c_1 \\ a_2x + b_2y = c_2 \end{cases}$, com $D = a_1b_2 - a_2b_1 \neq 0$:
$$x = \frac{c_1b_2 - c_2b_1}{D} \qquad y = \frac{a_1c_2 - a_2c_1}{D}$$
Se $D = 0$, as retas são paralelas ou coincidentes. Esse $D$ é um [[Determinantes|determinante]].
- **Em ML, sistemas lineares estão no coração de tudo.** Escrevendo de forma compacta, um sistema é $A\mathbf{x} = \mathbf{b}$, com uma **matriz** $A$ de coeficientes ([[Conceito de Matriz]], [[Sistemas Lineares]]).
  - A regressão linear com $n$ atributos se resolve com um sistema de $n$ equações (as *equações normais*).
  - Com mais equações do que incógnitas (muitos dados, poucos parâmetros), em geral não há solução exata, e procura-se a que **erra menos**: o método dos mínimos quadrados.
  - Bibliotecas como NumPy (`np.linalg.solve`) ou Math.NET (em C#) resolvem sistemas de milhares de equações pelo método da eliminação, a mesma ideia do método da adição.

---

## 🔗 Conexões
- **Usa:** [[Equações do 1º Grau]] (cada passo termina numa delas), [[Linguagem Algébrica]] (montar o sistema).
- **É parecido com:** [[Inequações do 1º Grau]] (sistemas de inequações: condições que valem juntas).
- **Mais adiante:**
  - [[Plano Cartesiano]], [[Equação da Reta]] e [[Posições Relativas entre Retas]]: a interpretação geométrica.
  - [[Conceito de Matriz]], [[Determinantes]] e [[Sistemas Lineares]]: sistemas grandes, com escalonamento.
  - [[Vetores e Operações Vetoriais]]: um sistema é uma pergunta sobre combinar vetores.

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Por que uma equação com duas incógnitas não basta para descobrir os dois valores?
2. Descreva o método da substituição em três passos.
3. Descreva o método da adição. Quando ele é melhor?
4. O que aparece nas contas quando o sistema é impossível? E quando é indeterminado? O que acontece com as retas?
5. Resolva $\begin{cases} x + y = 8 \\ 3x - y = 4 \end{cases}$ pelos dois métodos.
6. Monte o sistema: "Tenho 20 moedas de R\$ 0,50 e R\$ 1,00, que somam R\$ 14."
