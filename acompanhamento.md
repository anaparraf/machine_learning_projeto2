# Objetivo


# Entregas

## Terça-feira (14/05/2024)

- Descobrir quais modelos de machine learning classico podem ser treinados com dados out-of-core (ou seja, dados que não cabem completamente na RAM)

    - Batch training

        -Regressão Linear/Stochastic Gradient Descent (SGD): O SGD é especialmente útil para treinamento out-of-core, porque atualiza os pesos do modelo incrementalmente, utilizando um subconjunto dos dados (mini-batch) a cada iteração. Isto é ideal para grandes conjuntos de dados.

        -Regressão Logística com SGD: Assim como a regressão linear, a regressão logística também pode ser treinada usando SGD. Esta abordagem é eficaz para classificação binária em grandes conjuntos de dados.

        -Máquinas de Vetores de Suporte (SVM): Algumas implementações de SVM, especialmente aquelas que utilizam SGD, são capazes de lidar com dados out-of-core, permitindo o treinamento com grandes conjuntos de dados que não cabem na memória.

        -Naive Bayes: Dependendo da implementação, o Naive Bayes pode ser adaptado para treinamento out-of-core, processando os dados em partes para construir o modelo probabilístico.

        -Árvores de Decisão / Florestas Aleatórias: Embora as implementações tradicionais de árvores de decisão e florestas aleatórias não sejam tipicamente adequadas para dados out-of-core devido à sua necessidade de várias passagens pelos dados, existem versões modificadas que podem lidar com grandes conjuntos de dados de maneira incremental.

        -k-Means: Algoritmos de clustering como o k-Means podem ser adaptados para uso out-of-core ao atualizar os centróides do cluster incrementalmente em vez de em memória completa.


- Analise exploratoria simples

    - Dask - Pandas-like para dados que não cabem na RAM

- Se possivel, já um primeiro modelo preditivo