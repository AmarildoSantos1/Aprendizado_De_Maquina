Atividade: Prevendo a Doença de Parkinson com Aprendizado de Máquina 
Objetivo: Aplicar os conhecimentos de Aprendizado de Máquina para construir um modelo 
preditivo capaz de identificar pacientes com Parkinson com base em características vocais. 
1. Dados:  
https://archive.ics.uci.edu/ml/machine-learning
databases/parkinsons/parkinsons.data 
Como importar os dados: 
url = "https://archive.ics.uci.edu/ml/machine-learning-databases/parkinsons/parkinsons.data" 
df = pd.read_csv(url) 
2. Preparação dos Dados 
Mostre como foi feita a separação entre variáveis preditoras (X) e variável alvo (y). 
Uma sugestão de separação é a seguinte:  
X = df[["MDVP:Fo(Hz)", "MDVP:Jitter(%)", "MDVP:RAP", "spread1"]] 
y = df["status"] 
a. Detalhe como foi realizada a divisão entre dados de treino e teste (Qual a 
porcentagem usada para treino e teste). 
b. Justifique o uso ou não do random_state. 
3. Criação e Treinamento do Modelo 
a. Utilize o modelo de Regressão Logística e indique quais suas 
caracteristicas. 
b. Altere alguns parâmetros (ex: max_iter), justifique. 
4. Utilize os dados de teste para avaliar o modelo 
a. Gere a acurácia e a matriz de confusão. Explique os resultados gerados. 
b. Analise se o modelo apresentou bom desempenho ou não.
