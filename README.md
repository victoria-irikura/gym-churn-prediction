# Análise e Predição de Rotatividade de Clientes em Academia

## 📌 Descrição do projeto

Este projeto tem como objetivo analisar o comportamento dos clientes de uma rede de academias e desenvolver um modelo preditivo de churn (rotatividade). A partir de dados sobre perfil, contratos, frequência de uso e gastos adicionais, buscamos identificar os fatores que mais influenciam a saída dos clientes e propor estratégias para aumentar a retenção.

## 🎯 Objetivos

* Analisar padrões de comportamento entre clientes que permanecem e que cancelam.
* Identificar os principais fatores associados ao churn.
* Treinar modelos de machine learning para prever a probabilidade de rotatividade.
* Segmentar clientes em grupos de risco por meio de técnicas de clusterização.
* Formular recomendações de marketing e retenção com base nos achados.

## 🗂️ Estrutura dos dados

O conjunto de dados utilizado pode ser encontrado em:
`datasets/gym_churn_us.csv`

Ele contém informações como:

* **Perfil do cliente:** gênero, idade, localização, vínculo com empresas parceiras.
* **Contrato:** duração, meses restantes, tempo de relacionamento com a academia.
* **Engajamento:** frequência média de treinos (histórica e recente), participação em grupos.
* **Financeiro:** gastos adicionais em serviços como café, massagem, produtos esportivos.
* **Target:** variável `churn` indicando se o cliente permaneceu (`0`) ou cancelou (`1`).

## ⚙️ Modelos utilizados

* **Regressão Logística** → desempenho superior em precisão e acurácia.
* **Random Forest** → desempenho próximo, útil para capturar relações não lineares.
* **K-Means** → clusterização dos clientes em 5 grupos, destacando perfis fiéis e de risco.

## 📊 Principais descobertas

* Clientes mais velhos, engajados, com contratos longos e vínculos sociais apresentam churn muito baixo.
* Clientes jovens, de contratos curtos e baixa frequência concentram as maiores taxas de rotatividade (\~45–50%).
* Clusters 1 e 2 representam os clientes mais valiosos (churn < 5%).
* Clusters 0, 3 e 4 concentram perfis de alto risco, exigindo estratégias específicas de retenção.

## 💡 Recomendações estratégicas

1. **Incentivar contratos longos** com planos anuais e benefícios extras.
2. **Aumentar o engajamento** com desafios semanais, gamificação e programas de recompensa.
3. **Reforçar vínculos sociais** por meio de convênios corporativos, aulas coletivas e promoções “traga um amigo”.

## 🚀 Tecnologias utilizadas

* Python (pandas, numpy, matplotlib, seaborn, scikit-learn)
* Jupyter Notebook

## ▶️ Como executar o projeto

1. **Clone o repositório**

   ```bash
   git clone https://github.com/victoria-irikura/gym-churn-prediction.git
   cd gym-churn-prediction
   ```

2. **Crie e ative um ambiente virtual** (recomendado)

   ```bash
   python -m venv .venv
   source .venv/bin/activate   # Linux/Mac
   .venv\Scripts\activate      # Windows
   ```

3. **Instale as dependências**

   ```bash
   pip install -r requirements.txt
   ```

4. **Abra o Jupyter Notebook**

   ```bash
   jupyter notebook
   ```

5. **Execute o notebook principal** para rodar a análise:

   * `gym-churn-prediction.ipynb`

---

**Desenvolvido por:**
Victória Irikura
Bootcamp de Análise de Dados | Tripleten
2025

