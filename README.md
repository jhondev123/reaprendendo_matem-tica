# 📐 Reaprender Matemática

Meu cofre do [Obsidian](https://obsidian.md) para **reaprender matemática do zero até o cálculo**, com uma base sólida para estudar **machine learning** depois.

A ideia: recuperar tudo o que a escola deveria ter deixado firme (frações, potências, álgebra, funções, trigonometria) e seguir até o cálculo diferencial e integral, a álgebra linear e a probabilidade que aparecem nas fórmulas de ML. As notas são estudadas junto com um **caderno físico**, onde ficam os resumos e os exercícios resolvidos à mão.

---

## 🗺️ A trilha

| Fase                                  | #   | Tema                                                                                                | Situação    |
| ------------------------------------- | --- | --------------------------------------------------------------------------------------------------- | ----------- |
| Fundamentos                           | 01  | [Aritmética](<01 - Aritmética/Aritmética.md>)                                                       | 📘 completo |
|                                       | 02  | [Álgebra](<02 - Álgebra/Álgebra.md>)                                                                | 📘 completo |
| Pré-cálculo                           | 03  | [Funções](<03 - Funções/Funções.md>)                                                                | 📝 esboço   |
|                                       | 04  | [Exponenciais e Logaritmos](<04 - Exponenciais e Logaritmos/Exponenciais e Logaritmos.md>)          | 📝 esboço   |
|                                       | 05  | [Geometria Plana](<05 - Geometria Plana/Geometria Plana.md>)                                        | 📝 esboço   |
|                                       | 06  | [Trigonometria](<06 - Trigonometria/Trigonometria.md>)                                              | 📝 esboço   |
|                                       | 07  | [Geometria Analítica](<07 - Geometria Analítica/Geometria Analítica.md>)                            | 📝 esboço   |
|                                       | 08  | [Sequências e Séries](<08 - Sequências e Séries/Sequências e Séries.md>)                            | 📝 esboço   |
| Cálculo                               | 09  | [Cálculo Diferencial](<09 - Cálculo Diferencial/Cálculo Diferencial.md>)                            | 📝 esboço   |
|                                       | 10  | [Cálculo Integral](<10 - Cálculo Integral/Cálculo Integral.md>)                                     | 📝 esboço   |
| Matrizes, probabilidade e estatística | 11  | [Matrizes e Sistemas Lineares](<11 - Matrizes e Sistemas Lineares/Matrizes e Sistemas Lineares.md>) | 📝 esboço   |
|                                       | 12  | [Combinatória e Probabilidade](<12 - Combinatória e Probabilidade/Combinatória e Probabilidade.md>) | 📝 esboço   |
|                                       | 13  | [Estatística Básica](<13 - Estatística Básica/Estatística Básica.md>)                               | 📝 esboço   |
| Ponte para ML                         | 14  | [Ponte para Machine Learning](<14 - Ponte para Machine Learning/Ponte para Machine Learning.md>)    | 📝 esboço   |

- **📘 completo:** cada conceito tem explicação, exercícios e gabarito.
- **📝 esboço:** a pasta de cada conceito já existe, com uma nota curta dizendo o que estudar. O conteúdo completo é gerado quando eu chegar lá (veja [Como Gerar Conteúdo](<00 - Comece Aqui/Como Gerar Conteúdo.md>)).

O mapa completo, com as dependências entre os temas, está em [Mapa da Matemática](<00 - Comece Aqui/Mapa da Matemática.md>).

---

## 📂 Como o cofre está organizado

```
00 - Comece Aqui/          método de estudo, mapa, painel de progresso, caderno de erros,
                           símbolos e LaTeX, provas e olimpíadas, templates
01 - Aritmética/
├── Aritmética.md          índice do tema (trilha, progresso, checklist final)
├── Aritmética - Diagnóstico.md
├── 01 - Sistema de Numeração Decimal/
│   ├── Sistema de Numeração Decimal.md              ← explicação
│   ├── Sistema de Numeração Decimal - Exercícios.md
│   └── Sistema de Numeração Decimal - Gabarito.md
├── ...
└── 15 - Treino Misto/     5 listas misturando frações, dízimas, raízes e potências
02 - Álgebra/
...
14 - Ponte para Machine Learning/
```

Cada conceito tem **três notas**:

| Nota | O que tem |
|---|---|
| **Explicação** | checklist de etapas, objetivos, intuição, regras, exemplos resolvidos, erros comuns, conexão com programação (C#) e ML, links para os conceitos relacionados e perguntas de revisão |
| **Exercícios** | 🟢 fácil → 🟡 médio → 🔀 misto → 🔴 difícil (estilo OBMEP) → 💻 extra em C# → 🏅 provas reais |
| **Gabarito** | respostas e resoluções, separadas para eu não espiar |

---

## 🔁 Método de estudo

1. **Diagnóstico** do tema, para saber onde focar.
2. **Ler com o caderno aberto**, resumindo com as minhas palavras e refazendo os exemplos sem olhar.
3. **Praticar** os exercícios no caderno e corrigir ao fim de cada bloco.
4. **Registrar os erros** no [Caderno de Erros](<00 - Comece Aqui/Caderno de Erros.md>) e refazer no dia seguinte.
5. **Revisão ativa**: responder às perguntas sem consultar (técnica Feynman).
6. **Concluir**: marcar `concluido` e agendar a próxima revisão.
7. **Revisão espaçada**: rever depois de 7 dias, depois de 30 e depois de 90.

Detalhes em [Comece Aqui](<00 - Comece Aqui/Comece Aqui.md>).

---

## 📊 Progresso

Cada nota de explicação tem as propriedades:

```yaml
concluido: false        # marco quando termino o conceito
concluido_em:           # data em que concluí
proxima_revisao:        # data da próxima revisão espaçada
conteudo_pronto: true   # false enquanto o conceito for só um esboço
```

O painel [`Progresso.base`](<00 - Comece Aqui/Progresso.base>) usa o recurso **Bases** do Obsidian para mostrar os próximos conceitos, as revisões do dia, o progresso por tema e o desempenho nos treinos.

---

## 🛠️ Para abrir

1. Clone o repositório.
2. No Obsidian: **Abrir pasta como cofre** e selecione a pasta clonada.
3. Não precisa de plugins da comunidade: tudo usa recursos nativos (Bases, Templates, Mermaid e LaTeX).

> As notas usam a sintaxe do Obsidian (links `[[ ]]`, callouts, Bases). No GitHub, as fórmulas em LaTeX e os diagramas Mermaid aparecem, mas os links internos e os painéis só funcionam dentro do Obsidian.

---

## 🏅 Fontes de exercícios reais

- [Provas e soluções da OBMEP](https://www.obmep.org.br/provas.htm)
- [Banco de Questões da OBMEP](https://www.obmep.org.br/banco.htm)
- [Portal do Saber (OBMEP)](https://portaldosaber.obmep.org.br/)

---

*Anotações pessoais de estudo, montadas com a ajuda do Claude. Os exercícios "estilo OBMEP" foram escritos para este cofre; as questões oficiais estão nos links acima.*
