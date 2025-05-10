
# 📊 Projeto de Análise Exploratória: Estudantes e Saúde Mental

Este projeto realiza uma **Análise Exploratória de Dados (EDA)** sobre um conjunto de dados de estudantes universitários, com o objetivo de entender como fatores como estudo, sono, uso de redes sociais, qualidade da dieta e escolaridade dos pais se relacionam com a **saúde mental e desempenho acadêmico**.

---

## 🔍 Objetivos

- Explorar padrões e correlações entre hábitos e saúde mental.
- Investigar como variáveis como sono, exercício e redes sociais impactam o bem-estar.
  
---

## 🛠️ Ferramentas utilizadas

- **Python 3**
- **Pandas** — manipulação de dados
- **Matplotlib / Seaborn** — visualização
- **Plotly Express** - visualização
---

## 🧠 Principais insights obtidos

- As duas variáveis que mais afetam a nota da prova é o tempo de estudo diário e a saúde mental.
- A diferença entre os gêneros em relação ao tempo médio de estudo é pequena, mas pessoas que não possuem gênero masculino ou feminino têm o maior tempo médio, seguidas por mulheres e, por último, homens.
- Trabalhar meio período reduz o tempo de estudo em todos os gêneros, com maior impacto entre pessoas de gênero "Outro".
1. Sem trabalhar, pessoas de gênero "Outro" estudam significativamente mais.
2. Com trabalho, a diferença entre F e M praticamente desaparece, e "Outro" passa a ter o menor tempo médio de estudo.
- Estudantes que conseguem fazer uma média de 2 a 3 treinos por semana tendem a serem mais saudáveis mentalmente do que estudantes que estão acima ou abaixo dessa média.
- A variável `escolaridade_dos_pais` tem valores nulos que foram tratados e convertidos para `category`, reduzindo significativamente o uso de memória.
- O uso de `pd.cut()` permitiu transformar variáveis numéricas contínuas (ex: notas da prova) em faixas categóricas para facilitar a visualização e interpretação.

---

## ⚙️ Como executar

1. Clone o repositório:
```bash
git clone https://github.com/seu_usuario/projeto_analise_estudantes.git
cd projeto_analise_estudantes
```

2. Instale as dependências:
```bash
pip install pandas matplotlib seaborn jupyter
```

3. Execute o notebook:
```bash
jupyter notebook projeto_analise_estudantes.ipynb
```

---

## 🧼 Pré-processamento feito

- Renomeação de colunas com `df.rename()`
- Conversão de tipos (`astype`, `category`, `float32`, etc.)
- Tratamento de valores nulos com `fillna()`
- Redução de memória com tipos otimizados
- Criação de variáveis categóricas com `pd.cut()`

---
