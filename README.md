# Seeds Dataset Classification (CRISP-DM Projeto)

Este projeto aplica a metodologia **CRISP-DM** ao *Seeds Dataset* da UCI, com foco em classificação de três variedades de grãos de trigo. Inclui notebooks em Jupyter que cobrem desde a aquisição dos dados até a entrega de modelos otimizados.

---

## 🎯 Objetivo
- Implementar todas as fases do CRISP-DM:  
  1. **Entendimento do Negócio**  
  2. **Entendimento dos Dados**  
  3. **Preparação dos Dados**  
  4. **Modelagem**  
  5. **Avaliação**  
  6. **Deploy**

- Comparar diversos algoritmos de classificação e otimizar hiperparâmetros via *GridSearchCV*.

---

## 📂 Estrutura do Projeto
```
FASE_04/
└── CTWP/
    └── Cap11/
        ├── seeds_dataset.txt
        ├── seeds_crispdm_local.ipynb
        ├── seeds_crispdm_fullsteps.ipynb
        └── seeds_crispdm_apostilas.ipynb
```

- **seeds_dataset.txt**: arquivo com 210 amostras e 8 atributos.
- **seeds_crispdm_local.ipynb**: CRISP-DM completo, leitura de TXT local, armazenamento em SQLite.
- **seeds_crispdm_fullsteps.ipynb**: Pipeline completo com estatísticas, visualizações, 5 classificadores e otimização de hiperparâmetros.
- **seeds_crispdm_apostilas.ipynb**: Versão enriquecida com práticas das apostilas (DDL, pipelines, Streamlit, segurança).

---

## ⚙️ Ambiente e Requisitos
- **Python** 3.6+  
- Bibliotecas:
  - `pandas`, `numpy`
  - `scikit-learn`
  - `matplotlib`, `seaborn`
  - `sqlite3`
  - `streamlit` (para app)

---

## 🚀 Como Executar
1. Clone o repositório e acesse a pasta:
   ```bash
   git clone https://github.com/seu-usuario/seu-repo.git
   cd seu-repo/FASE_04/CTWP/Cap11
   ```
2. Instale dependências (recomendado usar `venv` ou `conda`):
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn streamlit
   ```
3. Abra o notebook desejado:
   ```bash
   jupyter notebook seeds_crispdm_fullsteps.ipynb
   ```
4. (Opcional) Rode o app Streamlit:
   ```bash
   streamlit run seeds_crispdm_apostilas.ipynb
   ```

---

## 📓 Conteúdo dos Notebooks
- **Aquisição & DDL**: Leitura do TXT, criação de tabelas raw/processed/predictions em SQLite.  
- **Pré-processamento**: Limpeza, validação, escalonamento (StandardScaler).  
- **EDA**: Histogramas, boxplots, pairplots para análise visual.  
- **Modelagem**: Pipelines SCikit-learn com KNN, SVM, RandomForest, NaiveBayes e Regressão Logística.  
- **Otimização**: GridSearchCV em cada modelo para seleção de melhores hiperparâmetros.  
- **Deploy**: Exemplo de app Streamlit para previsão interativa.

---

## 📝 Licença
Material para fins **educacionais**. Sinta-se livre para adaptar e compartilhar.

---

## ✉️ Contato
- Felipe Menezes – [GitHub](https://github.com/seu-usuario)
- Slack do projeto: #fase4-ctwp
