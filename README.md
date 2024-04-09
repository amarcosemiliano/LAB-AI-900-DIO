# LAB-AI-900-DIO
Neste LAB, aprendemos a criar uma conta no Azure e exploramos as capacidades de Machine Learning da plataforma, a fim de desenvolver uma automação prática no AutoML, relacionada ao contexto de uma empresa que aluga bicicletas. 
Ao aplicar implementações e soluções escaláveis de aprendizado de máquina na nuvem da Microsoft, exploramos conhecimentos valiosos e ganhamos experiência na construção de soluções eficientes.

# Desenvolvimento do Lab
Antes iniciarmos o Lab, no Azure Machine Learning Studio, acessamos a página Automated ML (em Authoring). Posteriormente, criamos um novo trabalho de ML automatizado, respeitando as seguintes etapas:

### Configurações básicas:
- **Nome do trabalho:** mslearn-bike-automl
- **Novo nome do experimento:** mslearn-bike-rental
- **Descrição:** Aprendizado de máquina automatizado para previsão de aluguel de bicicletas
- **Marcadores:** nenhum

### Tipo de tarefa e dados:
- **Tarefa:** Regressão
- **Conjunto de dados:** Aluguel de bicicletas
- **Tipo de dados:** Tabular
- **Fonte de dados:** [URL da Web](https://aka.ms/bike-rentals)

### Configuração da tarefa:
- **Coluna de destino:** Aluguéis (inteiro)
- **Métrica primária:** raiz do erro quadrático médio normalizado
- **Modelos permitidos:** RandomForest e LightGBM

### Limites:
- **Máximo de testes:** 3
- **Máximo de testes simultâneos:** 3
- **Máximo de nós:** 3
- **Limite de pontuação da métrica:** 0,085 (finalizar o trabalho caso a pontuação da métrica de erro quadrático médio normalizado for igual ou inferior a 0,085).
- **Tempo limite:** 15
- **Tempo limite de iteração:** 15

