# Classificação de Sentimentos em Avaliações de Filmes (IMDb 50k)

**Disciplina:** Projetos em Inteligência Computacional – 2025/2
**Instituto:** IFAL Campus Arapiraca
**Curso:** Sistemas de Informação
**Aluno:** Sam
**Tipo:** Aprendizado Supervisionado – Classificação Binária

---

### Objetivo do Projeto

Desenvolver um classificador de sentimentos capaz de identificar automaticamente se uma crítica de filme é **positiva** ou **negativa** a partir do texto livre da avaliação.
Aplicação prática em sistemas de recomendação, moderação de reviews e análise de opinião.

### Dataset

* **IMDb Dataset of 50K Movie Reviews** (Kaggle)
* 50.000 avaliações rotuladas (25.000 positivas + 25.000 negativas)
* Dataset balanceado
* Link: [Kaggle IMDb Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

### Tecnologias e Modelos

| Modelo                  | Técnica                      | Acurácia no teste | Tempo de treino     |
| ----------------------- | ---------------------------- | ----------------- | ------------------- |
| Baseline (entregue)     | TF-IDF + Regressão Logística | **88.7 %**        | < 2 minutos (CPU)   |
| Versão avançada (bônus) | DistilBERT fine-tuning       | **90.2 %**        | ~12 min (GPU Colab) |

### Demo Interativa Online (ativa até 03/12/2025)

[Demo Gradio](https://SEU_LINK_GRADIO_AQUI.gradio.live)

### Estrutura do Repositório

```
imdb-sentimento-2025/
├── data/                     ← IMDB Dataset.csv (ignorado pelo .gitignore)
├── notebooks/
│   └── 1_Treinamento_IMDb.ipynb     ← código completo + interface Gradio
├── apresentacao/
│   └── Apresentacao_IMDb_Sentimento.pdf
├── requirements.txt
├── README.md
├── LICENSE                   ← MIT License
└── .gitignore
```

### Como Executar Localmente

```bash
# 1. Clone o repositório
git clone https://github.com/SEU_USUARIO/imdb-sentimento-2025.git
cd imdb-sentimento-2025

# 2. Crie e ative o ambiente virtual
python -m venv venv
venv\Scripts\activate          # Windows
# source venv/bin/activate     # Linux/Mac

# 3. Instale as dependências
pip install -r requirements.txt

# 4. Execute o notebook (recomendado)
jupyter notebook
→ Abra notebooks/1_Treinamento_IMDb.ipynb → Execute todas as células
```

### Resultados Alcançados

| Métrica  | Baseline (TF-IDF + RL) | DistilBERT (fine-tuning) |
| -------- | ---------------------- | ------------------------ |
| Acurácia | 88.7 %                 | 90.2 %                   |
| F1-Score | 0.887                  | 0.901                    |
| Precisão | 0.89                   | 0.90                     |
| Recall   | 0.88                   | 0.90                     |


### Licença

Este projeto está licenciado sob a MIT License – veja o arquivo LICENSE para detalhes.

### Referências

* IMDb Dataset of 50K Movie Reviews. Kaggle, 2017. Disponível em: [https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

* scikit-learn.org – Documentação oficial
* Gradio – Build Machine Learning Web Apps. Disponível em: [https://gradio.app](https://gradio.app)


