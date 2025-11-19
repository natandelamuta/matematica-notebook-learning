# Projeto: Predição de Desempenho Estudantil 🎓

Este repositório contém uma **esteira de Machine Learning (Pipeline)** desenvolvida para prever a aprovação de estudantes em Matemática com base em dados socioeconômicos e notas de outras disciplinas.

## 📂 Sobre o Dataset
O conjunto de dados `StudentsPerformance.csv` contém informações sobre:
- Notas (Matemática, Leitura, Escrita).
- Gênero e Etnia.
- Nível de escolaridade dos pais.
- Tipo de alimentação (Lunch) e curso preparatório.

## 🚀 Pipeline de Desenvolvimento

O projeto segue um fluxo estruturado de ciência de dados:

1.  **Análise Exploratória:**
    - Importação de bibliotecas e carga de dados.
    - Estatísticas descritivas para entender a distribuição das notas.
    
2.  **Tratamento de Dados:**
    - Verificação de integridade (remoção de duplicatas).
    - Criação do **Target Binário**: Define aprovação se `Math Score >= 60`.
    - **Label Encoding**: Transformação de variáveis de texto em números para leitura do algoritmo.

3.  **Modelagem:**
    - Divisão dos dados: **70% Treino, 15% Validação, 15% Teste**.
    - Algoritmo utilizado: **Random Forest Classifier**.

## 📊 Resultados

O modelo apresentou métricas sólidas na base de teste. 

- **Matriz de Confusão**: Utilizada para analisar falsos positivos e negativos.
- **Limitações**: Como observado nos testes de predição individual, o modelo é suscetível a erros pontuais, o que é esperado dado o tamanho do dataset (1.000 instâncias). O aumento da base de dados poderia refinar ainda mais a precisão.

## 🛠️ Como Reproduzir
1. Clone este repositório.
2. Instale as dependências: `pandas`, `numpy`, `sklearn`, `matplotlib`, `seaborn`.
3. Execute o notebook `pipeline_students.ipynb`.
