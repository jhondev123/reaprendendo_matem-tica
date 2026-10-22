---
tipo: gabarito
tema: Aritmética
conceito: "[[Razão, Proporção e Regra de Três]]"
tags:
  - aritmetica
  - gabarito
---
# Razão, Proporção e Regra de Três: Gabarito

**Voltar aos exercícios:** [[Razão, Proporção e Regra de Três - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $\frac{15}{25} = \frac{3}{5}$
**2.** $4 \cdot 50.000 = 200.000$ cm $= 2.000$ m $=$ **2 km**
**3.** $4x = 60 \Rightarrow x = 15$
**4.** $9x = 72 \Rightarrow x = 8$
**5.** Direta: $x = \frac{32{,}50 \cdot 8}{5} = $ **R\$ 52,00**
**6.** Inversa: $6 \cdot 10 = 4 \cdot x \Rightarrow x = $ **15 dias**
**7.** (a) inversa (b) direta (c) nenhuma
**8.** São 10 partes de 120: **240, 360 e 600**.

## 🟡 Médio
**1.** $\frac{0{,}5}{0{,}75} = \frac{50}{75} = \frac{2}{3}$. Então $\frac{x+1}{3} = \frac{2}{3} \Rightarrow x + 1 = 2 \Rightarrow x = 1$.
**2.** Direta: $340 \div 12{,}5 = 27{,}2$ litros.
**3.** As duas grandezas são diretas: $600 \cdot \frac{10}{8} \cdot \frac{6}{5} = 900$ peças.
**4.** Mais operários → menos dias (inversa); mais horas por dia → menos dias (inversa).
$$x = 20 \cdot \frac{15}{12} \cdot \frac{8}{10} = 20 \cdot 1{,}25 \cdot 0{,}8 = 20 \text{ dias}$$
(Pelo "trabalho total": $15 \cdot 8 \cdot 20 = 2400$ horas-homem, e $2400 \div (12 \cdot 10) = 20$ dias.)
**5.** De cada $1 + 9 = 10$ exemplos, 1 é positivo: $\frac{25.000}{10} = $ **2.500**.
**6.** $h = \frac{1080 \cdot 1280}{1920} = $ **720**.
**7.** $1{,}5 \cdot \frac{3}{2} = 2{,}25$ h $=$ **2 h 15 min**.

## 🔴 Difícil
**1.** **2 horas.**
Em 1 hora, A enche $\frac{1}{3}$ do tanque e B enche $\frac{1}{6}$. Juntas, enchem $\frac{1}{3} + \frac{1}{6} = \frac{1}{2}$ do tanque por hora, então levam 2 horas.
💡 *Ideia-chave: some as **taxas** (tanque por hora), não os tempos. A resposta "4,5 h" (a média) ou "9 h" (a soma) não faz sentido: juntas, elas têm que ser mais rápidas que a mais rápida sozinha.*

**2.** **30 segundos.**
$72$ km/h $= \frac{72.000 \text{ m}}{3.600 \text{ s}} = 20$ m/s. A frente do trem precisa andar o comprimento da ponte **mais** o do próprio trem: $400 + 200 = 600$ m. Tempo: $600 \div 20 = 30$ s.

**3.** **16 alunos.**
Com a razão 3 : 5, havia $3k$ meninos e $5k$ meninas. Depois, $3k + 4 = 5k$, ou seja, $k = 2$. Eram 6 meninos e 10 meninas, 16 alunos. (Conferindo: 10 meninos e 10 meninas, razão 1 : 1. ✔️)

**4.** **3 gatos.**
Os 3 gatos caçam 3 ratos em 3 minutos, então cada gato caça 1 rato a cada 3 minutos. Em 100 minutos, cada gato caça $\frac{100}{3}$ ratos. Para 100 ratos: $100 \div \frac{100}{3} = 3$ gatos.
💡 *A pegadinha é achar que a resposta é 100. Calcule a **taxa de um gato** primeiro.*

## 💻 Extra em C#
**1.**
```csharp
double Mapear(double x, double a, double b, double c, double d)
    => c + (x - a) * (d - c) / (b - a);
```
**2.**
```csharp
(int Largura, int Altura) Redimensionar(int l, int a, int novaLargura)
    => (novaLargura, (int)Math.Round((double)a * novaLargura / l));
// Redimensionar(1920, 1080, 1280) == (1280, 720)
```
