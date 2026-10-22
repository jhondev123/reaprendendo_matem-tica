---
tipo: gabarito
tema: Aritmética
conceito: "[[Operações Fundamentais]]"
tags:
  - aritmetica
  - gabarito
---
# Operações Fundamentais: Gabarito

**Voltar aos exercícios:** [[Operações Fundamentais - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $56 \div 7 = 8$: dividendo 56, divisor 7, quociente 8. Em $56 - 7 = 49$: minuendo 56, subtraendo 7, diferença 49.
**2.** $(25 + 75) + 68 = 168$
**3.** $(4 \cdot 25) \cdot 13 = 100 \cdot 13 = 1300$
**4.** Quociente 7, resto 5: $47 = 6 \cdot 7 + 5$.
**5.** (a) F  (b) V  (c) V  (d) F (não existe)
**6.** $6 \cdot (100 + 2) = 600 + 12 = 612$
**7.** $0$, $0$, $1$
**8.** $42 \cdot 24 = 1008$ ✔️, então a divisão está correta.

## 🟡 Médio
**1.** $48 \cdot (9 + 1) = 480$
**2.** $15 \cdot (100 - 1) = 1500 - 15 = 1485$
**3.** O maior resto possível é $12 - 1 = 11$. Então $D = 12 \cdot 25 + 11 = 311$.
**4.** $1000 = 64 \cdot 15 + 40$: são **15 lotes completos** e o último tem **40 imagens**, num total de **16 lotes**.
**5.** $1000 = 7 \cdot 142 + 6$. As semanas completas voltam ao sábado e os 6 dias que restam levam a **sexta-feira** (sáb → dom, seg, ter, qua, qui, **sex**).
**6.** $(24 \div 4) \div 2 = 6 \div 2 = 3$, mas $24 \div (4 \div 2) = 24 \div 2 = 12$. Os resultados são diferentes, o que prova que a divisão **não é associativa**.

## 🔴 Difícil
**1.** **Resto 2.**
Pela relação fundamental, o número é $n = 6q + 5$. Reescrevendo: $n = 6q + 3 + 2 = 3(2q + 1) + 2$. Então $n$ é "um múltiplo de 3 mais 2", e o resto da divisão por 3 é **2**. (Teste: 11, 17 e 23 deixam resto 5 na divisão por 6 e resto 2 na divisão por 3.)
💡 *Ideia-chave: escrever o número como $d \cdot q + r$ e reagrupar.*

**2.** **3.**
O algarismo das unidades de um produto depende **só dos algarismos das unidades** dos fatores: $6 \cdot 7 \cdot 8 = 336$, que termina em 6. Somando 7: $6 + 7 = 13$, que termina em **3**.

**3.** **5050.**
Pareie os termos: $(1 + 100) + (2 + 99) + (3 + 98) + \dots + (50 + 51)$. Cada par dá 101 e há 50 pares: $50 \cdot 101 = 5050$. (É o truque que se atribui a Gauss, quando criança. Você vai rever isso em PA.)

**4.** **9, 15, 25, 45, 75 e 225.**
$230 = d \cdot q + 5 \Rightarrow d \cdot q = 225$. Então $d$ é um divisor de 225 e, além disso, $d > 5$, porque o resto tem que ser menor que o divisor. Os divisores de 225 são 1, 3, 5, 9, 15, 25, 45, 75 e 225. Tirando os que não são maiores que 5, sobram **9, 15, 25, 45, 75 e 225**.

## 💻 Extra em C#
**1.**
```csharp
(int Quociente, int Resto) Dividir(int dividendo, int divisor)
{
    if (divisor == 0) throw new DivideByZeroException();
    int q = 0;
    while (dividendo >= divisor)
    {
        dividendo -= divisor; // "cabe mais uma vez"
        q++;
    }
    return (q, dividendo); // o que sobrou é o resto
}
```
**2.** `(total + tamanho - 1) / tamanho`: somar `tamanho - 1` faz qualquer resto diferente de zero "transbordar" para mais um lote. Se a divisão já for exata, o acréscimo não chega a completar outro lote.
Exemplo: `(1000 + 63) / 64 = 1063 / 64 = 16`, enquanto `(1024 + 63) / 64 = 1087 / 64 = 16`, porque 1024 já é múltiplo de 64.
