# Classificação de Grãos de Trigo com Seeds Dataset 

Projeto desenvolvido como parte do desafio Hermes Reply (Fase 4), com foco em aplicar a metodologia **CRISP-DM** ao *Seeds Dataset* da UCI para classificação de três variedades de grãos de trigo.

## 🎯 Objetivo
Aplicar todas as fases do CRISP-DM ao Seeds Dataset:
1. Entendimento do Negócio  
2. Entendimento dos Dados  
3. Preparação dos Dados  
4. Modelagem  
5. Avaliação  
6. Deploy (exemplo de app Streamlit)

## 🧪 Lista de Atributos Utilizados e Justificativa
- **area, perimeter, compactness**  
  Medidas geométricas que ajudam a diferenciar variedades de grãos.  
- **kernel_length, kernel_width**  
  Dimensões dos grãos, essenciais para distinção de classe.  
- **asymmetry_coefficient, groove_length**  
  Características de forma que aprimoram a segmentação de classes.


## 💻 Código-Fonte Representativo
```python
import pandas as pd

# Carregar dados
col_names = [
    "area","perimeter","compactness","kernel_length","kernel_width",
    "asymmetry_coefficient","groove_length","class"
]
df = pd.read_csv(
    "seeds_dataset.txt",
    sep=r"\s+",
    names=col_names
)
# Exemplo: estatísticas descritivas
print(df.describe())
```

## 🔍 Processamento e Modelagem
- **Pré-processamento**: tratamento de valores ausentes e padronização com `StandardScaler`.  
- **Modelagem**: pipelines com KNN, SVM e RandomForest.  
- **Otimização**: `GridSearchCV` para seleção de hiperparâmetros.

## 📊 Análise Gráfica
- Histogramas e boxplots para distribuição de atributos.  
- Pairplot para dispersão e correlação entre variáveis.  
- Importância de atributos no RandomForest.

## 🔗 Links do Projeto
- **Notebook Colab (CRISP-DM Full Steps)**:  
  https://colab.research.google.com/drive/1BJvYSt8V64tG8Hnme5tiAllYLUWOoj9b  
- **Repositório GitHub**:  
  https://github.com/seu-usuario/seu-repo/tree/main/FASE_04/CTWP/Cap11

## ✅ Conclusão
Este projeto demonstrou com sucesso a aplicação prática do CRISP-DM ao Seeds Dataset, desde a ingestão dos dados até a entrega de modelos otimizados e um app Streamlit de demonstração.

## 👨‍💻 Integrantes
- Flavia Nunes Bocchino – RM564213  
- Pedro Henrique Zani – RM564956  
- Felipe Menezes – RM557891  

## 🎓 Curso
FIAP | Enterprise Challenge 2025.1  
Fase 4 – Cap 3 (Ir Além)

