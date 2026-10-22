---
tipo: guia
tags:
  - guia
---
# 🛠️ Como Gerar Conteúdo

Os temas a partir de [[Funções]] estão em **esboço**: cada conceito já tem a sua pasta e uma nota curta dizendo o que estudar. Quando chegar a vez de um deles, peça ao Claude (de preferência no projeto **Reaprender matemática**) para gerar o conteúdo completo no mesmo padrão de [[Aritmética]] e [[Álgebra]].

## Prompt para um conceito

```
Gere o conteúdo completo do conceito [[NOME DO CONCEITO]] do tema TEMA no meu cofre
do Obsidian (C:\Users\jhonattan\Documents\estudo\matemática).
Siga o padrão de "00 - Comece Aqui/Como Gerar Conteúdo.md" e use uma nota pronta de
Aritmética ou Álgebra como referência. A nota-esboço já existe na pasta do conceito:
transforme-a na explicação completa e crie as notas de exercícios e de gabarito.
```

## Prompt para um tema inteiro

```
Gere o conteúdo completo de todos os conceitos do tema [[TEMA]] no meu cofre do
Obsidian (C:\Users\jhonattan\Documents\estudo\matemática), seguindo o padrão de
"00 - Comece Aqui/Como Gerar Conteúdo.md". Crie também o "TEMA - Diagnóstico" e
atualize a situação do tema no Mapa da Matemática.
```

---

## O padrão (referência para quem for gerar)

### Pastas e nomes
- Tema: `NN - Tema/` com a nota `Tema.md` (o índice do tema, com `tipo: tema`).
- Conceito: `NN - Tema/NN - Conceito/` com **3 notas**:
  - `Conceito.md`: explicação (`tipo: conceito`)
  - `Conceito - Exercícios.md` (`tipo: exercicios`)
  - `Conceito - Gabarito.md` (`tipo: gabarito`)
- Os nomes de nota são **únicos no cofre**, para os links `[[ ]]` funcionarem sem caminho.

### Propriedades da nota de explicação
```yaml
tipo: conceito
tema: Nome do Tema
concluido: false        # checkbox que o estudante marca
concluido_em:           # data
proxima_revisao:        # data, alimenta a lista "Revisar hoje"
conteudo_pronto: true   # false enquanto for esboço
aliases: [outros nomes do conceito]
tags: [tema-sem-acento]
```

### Preferências do estudante (importante)
- **Links por todo lado.** Cite outros conceitos **no próprio texto** com `[[ ]]` (inclusive os de temas futuros, que já existem como esboço) e termine cada explicação com a seção `## 🔗 Conexões` (Usa · É usado em · Mais adiante). O grafo do Obsidian é parte do aprendizado.
- **Misturar conjuntos numéricos.** Inclua sempre exercícios 🔀 com frações, decimais, dízimas, raízes e negativos juntos.
- **Do zero, com calma**, nos temas novos: intuição antes da fórmula, passo a passo, callouts `> [!question]- Tente agora` com a resposta recolhida e vários exemplos resolvidos.
- **Bastante treino de contas** (como o bloco 🧮 de [[Monômios e Polinômios - Exercícios]]): quando o conceito envolve operações, crie um bloco extra só de cálculo.
- **Conferir tudo**: todas as respostas do gabarito devem ser verificadas (de preferência por computador).
- Links para títulos de seção (`[[Nota#Título]]`) só para títulos **sem** `:` e sem LaTeX; dentro de tabelas, escreva o alias com `\|`.

### Estrutura da explicação
1. `> [!abstract] Em uma frase`: a ideia central.
2. Linha de navegação: **Tema · Pré-requisitos · Próximo** e **Praticar** (links para exercícios e gabarito).
3. `## ✅ Etapas`: o checklist padrão (igual ao [[Template - Conceito]]).
4. `## 🎯 Ao final, você deve conseguir`: de 3 a 5 objetivos concretos.
5. Seções numeradas com a teoria, **sempre com a intuição antes da fórmula**, usando exemplos do dia a dia, callouts (`[!tip]`, `[!example]`, `[!warning]`) e LaTeX.
6. `## 📝 Exemplos resolvidos`: de 3 a 5 exemplos, passo a passo.
7. `## ⚠️ Erros comuns`: os erros clássicos, com o certo e o errado lado a lado.
8. `## 💻 Conexão com programação e ML`: o estudante é desenvolvedor C#. Use analogias com código e diga onde o conceito aparece em machine learning.
9. `## 🔗 Conexões`: Usa · É usado em · Mais adiante, com links.
10. `## 🧠 Revisão ativa`: de 5 a 8 perguntas **sem resposta** (as respostas estão no texto).

### Estrutura dos exercícios
- `## 🟢 Fácil` (de 8 a 10 itens), `## 🟡 Médio` (de 6 a 10, com problemas contextualizados e itens 🔀 misturando conjuntos), `## 🔴 Difícil (estilo OBMEP)` (de 3 a 4, no estilo de olimpíada, escritos do zero; não atribuir a uma prova específica sem ter certeza), `## 💻 Extra em C# (opcional)` (1 ou 2) e `## 🏅 Teste-se com provas reais` (com link para [[Provas e Olimpíadas]] e o nível da OBMEP indicado).
- Cada item é um checkbox: `- [ ] **1.** enunciado`.

### Estrutura do gabarito
- As mesmas seções e numeração dos exercícios.
- Fáceis: só a resposta. Médios: a resposta e o raciocínio principal. Difíceis: a resolução completa, explicando a ideia-chave.
- **Todas as contas conferidas.**

### Diagnóstico do tema (`Tema - Diagnóstico.md`)
- Duas questões por conceito, agrupadas por conceito, com a resposta num callout recolhido `> [!success]- Resposta`.
- Uma tabela no fim dizendo: "errou as questões do conceito X? Estude-o com calma; acertou? Pode ir mais rápido".

### Esboço → conteúdo pronto
Ao gerar o conteúdo, reaproveite o "O que estudar aqui" da nota-esboço como roteiro, troque `conteudo_pronto` para `true` e remova o aviso `[!todo]`.
