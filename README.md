# 📘 Telecom X – Advanced Churn Analytics

## 🚀 Visão Geral  
Este projeto implementa uma **pipeline completa de ciência de dados** para prever a evasão de clientes (churn) da Telecom X e propor estratégias de retenção data-driven. Construído em Jupyter Notebook com foco em **reprodutibilidade**, **clareza de código**, **impacto analítico** e **melhores práticas** de MLOps.

***

## 📋 Sumário  

1. [Motivação](#motivação)  
2. [Funcionalidades](#funcionalidades)  
3. [Estrutura do Repositório](#estrutura-do-repositório)  
4. [Instalação e Dependências](#instalação-e-dependências)  
5. [Uso](#uso)  
6. [Metodologia](#metodologia)  
7. [Resultados](#resultados)  
8. [Estratégias e Recomendações](#estratégias-e-recomendações)  
9. [KPIs & Monitoramento](#kpis--monitoramento)  
10. [Contato](#contato)

***

## 📝 Motivação  
- Reduzir perdas de receita decorrentes de churn  
- Antecipar clientes em risco e otimizar campanhas de retenção  
- Fornecer insights acionáveis para equipes de CS e Marketing  

***

## ⚙️ Funcionalidades  
- Carregamento e inspeção automática dos dados  
- Análise exploratória com estatísticas e visualizações detalhadas  
- Pré-processamento robusto (OneHotEncoder, StandardScaler, SMOTE)  
- Treinamento de múltiplos modelos (LogisticRegression, RandomForest, KNN, Ensemble)  
- Otimização de hiperparâmetros via `GridSearchCV`  
- Avaliação comparativa: acurácia, precisão, recall, F1-score, AUC-ROC  
- Matrizes de confusão, curvas ROC e radar charts  
- Interpretabilidade: feature importance e coeficientes de regressão  
- Segmentação de risco e recomendações estratégicas  
- KPIs, thresholds e cronograma de monitoramento  

***

## 📂 Estrutura do Repositório  
```
├── TelecomX_Parte2.ipynb  # Notebook principal  
├── README.md                               # Este documento  
├── requirements.txt                        # Dependências Python  
└── data/                                   # (Opcional) Dados locais  
```

***

## ⚙️ Instalação e Dependências  

1. Clone o repositório:  
   ```bash
   git clone https://github.com/everton754/TelecomX-Churn-Analytics.git
   cd TelecomX-Churn-Analytics
   ```

2. Crie e ative um ambiente virtual (opcional):  
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Instale as dependências:  
   ```bash
   pip install -r requirements.txt
   ```

   **requirements.txt**:
   ```
   pandas
   numpy
   requests
   seaborn
   matplotlib
   scikit-learn
   imbalanced-learn
   ```

***

## 🚀 Uso  

1. Abra o notebook no Jupyter ou Colab:  
   ```bash
   jupyter notebook TelecomX_Parte2.ipynb
   ```

2. Execute as células sequencialmente:
   - **Seção 0**: Verificação de ambiente  
   - **Seção 1**: Cenário de negócio  
   - **Seção 2**: Metodologia  
   - **Seção 3**: EDA  
   - **Seção 4**: Pré-processamento  
   - **Seção 5**: Modelagem  
   - **Seção 6**: Avaliação  
   - **Seção 7**: Interpretabilidade  
   - **Seção 8**: Recomendações  
   - **Seção 9**: Conclusão

***

## 🔬 Metodologia  

- **EDA**: Estatísticas descritivas, gráficos de distribuição, boxplots, heatmap de correlação  
- **Pré-processamento**:  
  - One-Hot Encoding de variáveis categóricas  
  - Z-score normalization para numéricas  
  - SMOTE para balanceamento  
- **Modelagem**:  
  - Logistic Regression  
  - Random Forest  
  - KNN otimizado  
  - VotingClassifier (ensemble)  
- **Avaliação**:  
  - Metrics: accuracy, precision, recall, F1-score, AUC-ROC, cross-val F1  
  - Matrizes de confusão e curvas ROC  
- **Interpretabilidade**:  
  - Feature importance (RF)  
  - Coeficientes (LR)  
  - Odds ratios  
- **Insights e Recomendações**:  
  - Segmentação de risco  
  - Plano de ação em fases  
  - KPIs e thresholds  

***

## 📈 Resultados  

- **Melhor Modelo**: ✅ Logistic Regression (AUC ~ 0.84, Recall ~ 0.80)  
- **Top 5 Fatores de Risco**:  
  1. Contract_Month-to-month  
  2. PaymentMethod_Electronic check  
  3. InternetService_Fiber optic  
  4. PaperlessBilling_Yes  
  5. MonthlyCharges (elevados)  
- **Top 5 Fatores Protetivos**:  
  1. Tenure  
  2. OnlineSecurity_Yes  
  3. TechSupport_Yes  
  4. Contract_Two year  
  5. Dependents_Yes  

***

## 💡 Estratégias e Recomendações  

- **Alto Risco**: intervenção imediata (contato proativo, benefícios exclusivos)  
- **Risco Moderado**: engajamento (campanhas de email, conteúdo educativo)  
- **Baixo Risco**: manutenção e upsell (programas de indicação, cross-sell)  
- **Implementação**: deploy, piloto em 20% da base, rollout completo  
- **KPIs**: Precision@Top10%, Recall, ROI, Model Drift, SLA operacional  

***

## 📊 KPIs & Monitoramento  

- **Modelo**: Precision@Top10%, Recall, AUC, Model Drift  
- **Negócio**: ROI Campanhas, Redução de Churn, Conversão, LTV incremental  
- **Operacional**: Tempo de resposta, Satisfação CS, Taxa de automação  

***

## 📞 Contato  

**Everton Santos**  
- LinkedIn: [linkedin.com/in/evert0n-sant0s](https://www.linkedin.com/in/evert0n-sant0s/)  
- GitHub: [github.com/everton754](https://github.com/everton754)  
- Email: eso.datalab@gmail.com  

***

**© 2025 Telecom X – Advanced Churn Analytics**  
**Confidencial – Uso interno e acadêmico**

[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/9764473/a48988f8-ac32-4816-a190-2ee054e4dd3a/TelecomX_Parte2.ipynb
