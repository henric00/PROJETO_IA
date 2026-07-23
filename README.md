# Análise e Modelagem Preditiva de Notas de Filmes (TMDB)

Projeto final desenvolvido para a disciplina de Inteligência Artificial, focado na aplicação de técnicas de Machine Learning para a predição de avaliações de filmes.

## Objetivo

Desenvolver e comparar modelos de regressão capazes de estimar a nota média (`vote_average`) de filmes da plataforma TMDB utilizando atributos relacionados ao engajamento do público e ao contexto temporal.

## Integrantes

* Carlos Henrico Fontes Cabral
* Gabriel Almeida Mota Bomfim
* Pedro Caldas de Souze Lucas Marques


## 👨‍💻 Divisão das Contribuições

O projeto foi desenvolvido de forma colaborativa, com a seguinte divisão de foco:

* **Gabriel Almeida Mota Bomfim:** Implementação do código-fonte em Python, preparação dos dados e treinamento dos modelos de Machine Learning (Regressão Linear, Árvore de Decisão e Random Forest).
* **Pedro Caldas de Souze Lucas Marques:** Extração e consolidação das métricas de avaliação (MAE, MSE, RMSE, R²) e geração dos gráficos de análise de resíduos dos modelos.
* **Carlos Henrico Fontes Cabral:** Revisão metodológica, adequação do código para execução em nuvem (Google Colab), redação das justificativas teóricas, interpretação analítica dos resultados e organização geral da documentação no GitHub.
---
## Fonte dos Dados

* **Dataset:** [TMDB Top 10000 Movies Updated 2026](https://www.kaggle.com/datasets/siddharthbhakta/tmdb-top-10000-movies-updated-2026)
* **Plataforma:** Kaggle

## Tipo da Tarefa

O problema foi tratado como uma tarefa de Aprendizado Supervisionado do tipo **Regressão**, tendo como variável-alvo a nota média (`vote_average`) dos filmes.

## Organização dos Arquivos

```text
PROJETO_IA/
│
├── Projeto_Final.ipynb
├── README.md
└── data/
    └── moviesTMBD.csv

## 🚀 Como Executar o Projeto

1. Acesse este repositório no GitHub.
2. Abra o arquivo `Projeto_Final.ipynb` no **Google Colab** (utilizando a opção **"Open in Colab"** ou importando o notebook diretamente na plataforma).
3. Execute as células sequencialmente, do início ao fim, para:
   - carregar o conjunto de dados;
   - realizar a análise exploratória;
   - executar o pré-processamento;
   - treinar os modelos de aprendizado de máquina;
   - avaliar os resultados obtidos.

---

## 🤖 Modelos Utilizados

| Modelo | Objetivo |
|---------|----------|
| **Regressão Linear** | Baseline (estabelecer um desempenho de referência). |
| **Árvore de Decisão** | Modelo intermediário para comparação de desempenho. |
| **Random Forest Regressor** | Modelo principal, capaz de capturar relações complexas e não lineares entre os atributos. |

---

## 📊 Principais Resultados

Foram comparados três modelos de regressão utilizando as métricas **MAE**, **MSE**, **RMSE** e **R²**.

O **Random Forest Regressor** apresentou o melhor desempenho geral, obtendo o menor erro médio e a maior capacidade de explicação da variabilidade das notas (`vote_average`) quando comparado aos demais modelos.

| Métrica | Regressão Linear | Árvore de Decisão | Random Forest |
|:--------:|:----------------:|:-----------------:|:-------------:|
| **MAE** | 0.4471 | 0.5347 | **0.4163** |
| **MSE** | 0.2951 | 0.5022 | **0.2754** |
| **RMSE** | 0.5433 | 0.7087 | **0.5247** |
| **R²** | 0.2927 | -0.2035 | **0.3400** |

Os resultados indicam que o **Random Forest** foi o modelo mais adequado para este problema, demonstrando maior capacidade de capturar os padrões presentes nos dados em comparação com os modelos linear e de árvore de decisão.

---

## 🎥 Vídeo de Apresentação

> **Link:** *(Inserir o link do vídeo no YouTube ou Google Drive.)*

---

## 🤝 Declaração de Uso de Inteligência Artificial

Durante o desenvolvimento deste projeto foram utilizadas ferramentas de Inteligência Artificial, **ChatGPT (OpenAI)** e **Gemini (Google)**, como instrumentos de apoio ao processo de aprendizagem e desenvolvimento.

O **ChatGPT** foi utilizado principalmente para esclarecer conceitos relacionados a Aprendizado de Máquina, discutir a estrutura metodológica do notebook, revisar textos e fornecer feedback sobre a coerência das análises e interpretações realizadas.

O **Gemini** foi utilizado como apoio na implementação de trechos de código, auxiliando na construção, adaptação e revisão de soluções durante o desenvolvimento do projeto.

As decisões referentes à definição do problema, escolha dos atributos, análise exploratória, implementação final do código, treinamento dos modelos, interpretação dos resultados e elaboração das conclusões foram conduzidas pelos autores.
As ferramentas de Inteligência Artificial foram empregadas exclusivamente como suporte ao aprendizado, revisão metodológica e auxílio ao desenvolvimento, mantendo-se a responsabilidade pelas decisões técnicas e pelo conteúdo final do trabalho.
