# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).


## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

- Dê um fork neste projeto e reescreva este `README.md`. Sinta-se à vontade para detalhar todo o processo de criação do seu Modelo de ML para uma "Previsão de Estoque Inteligente".
- Para isso, siga o [passo a passo] descrito a seguir e evolua as suas habilidades em ML no-code com o Amazon SageMaker Canvas.
- Ao concluir, envie a URL do seu repositório com a solução na plataforma da DIO.


## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Navegue até a pasta `datasets` deste repositório. Esta pasta contém os datasets que você poderá escolher para treinar e testar seu modelo de ML. Sinta-se à vontade para gerar/enriquecer seus próprios datasets, quanto mais você se engajar, mais relevante esse projeto será em seu portfólio.
-   Escolha o dataset que você usará para treinar seu modelo de previsão de estoque.
-   Faça o upload do dataset no SageMaker Canvas.

### 2. Construir/Treinar

-   No SageMaker Canvas, importe o dataset que você selecionou.
-   Configure as variáveis de entrada e saída de acordo com os dados.
-   Inicie o treinamento do modelo. Isso pode levar algum tempo, dependendo do tamanho do dataset.

### 3. Analisar

-   Após o treinamento, examine as métricas de performance do modelo.
-   Verifique as principais características que influenciam as previsões.
-   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

-   Use o modelo treinado para fazer previsões de estoque.
-   Exporte os resultados e analise as previsões geradas.
-   Documente suas conclusões e qualquer insight obtido a partir das previsões.

## 🤔 Dúvidas?

Esperamos que esta experiência tenha sido enriquecedora e que você tenha aprendido mais sobre Machine Learning aplicado a problemas reais. Se tiver alguma dúvida, não hesite em abrir uma issue neste repositório ou entrar em contato com a equipe da DIO.

# Passo a passo 

### 1. Selecionar Dataset

-   Será utilizado o único dataset que foi disponibilizado no repositório.

### 2. Construir/Treinar

-   Será utilizado o Product_ID como ID e o Stock_level base para as previsões com as 90 linhas.
-   eu usei o quick build para geração de modelo.

### 3. Analisar

-   Métricas do modelo - o modelo não foi considerado muito bom, mas será utilizado.
![image](https://github.com/JoaoricardodeOA/lab-aws-sagemaker-canvas-estoque/assets/83128494/1072b433-34fa-4844-9478-d3cb6eac18a2)

-   Principais impactos - No modelo foi verificado uma dependência maior das vendas e dias da semana
![image](https://github.com/JoaoricardodeOA/lab-aws-sagemaker-canvas-estoque/assets/83128494/7a7fbb52-de51-4f18-99b9-c4b7b30bd92e)

### 4. Prever

-   Previsões de estoque:
![image](https://github.com/JoaoricardodeOA/lab-aws-sagemaker-canvas-estoque/assets/83128494/f38097db-6f30-42db-817f-8a63e91485b6)

![image](https://github.com/JoaoricardodeOA/lab-aws-sagemaker-canvas-estoque/assets/83128494/b5f70f0c-271b-4a2e-a104-d6dcefc74c48)

![image](https://github.com/JoaoricardodeOA/lab-aws-sagemaker-canvas-estoque/assets/83128494/f0b7a08a-c1dd-495f-ae07-2da964a275d5)

Dos itens somente o item 2 teve alta de estoque.

-  Para uma boa gestão de estoque, deve ser feito maiores compras do item 2 em detrimento dos outros e para prevenção de perdas o item 3 e principalmente o 1 devem evitar as compras deles.
