# Exploração de dados: Drinking Water Potability

## Introdução

O [Drinking Water Potability](https://www.kaggle.com/code/deblina00/drinking-water-potability-eda-and-prediction) é um dataset feito para predição que contém 3277 amostras de água. Existem 10 atributos que nos mostram a qualidade da água, como pH, turbidez, condutividade, entre outros. Por fim, o dataset apresenta um atributo "Potability" que indica se a amostra é potável ou não.

## Análise exploratória

### Caracterização dos dados

| Atributo        | Tipo         |
|       ---       |     ---      |
| pH              | Quantitativo |
| Hardness        | Quantitativo |
| Solids          | Quantitativo |
| Chloramines     | Quantitativo |
| Sulfat          | Quantitativo |
| Conductivity    | Quantitativo |
| Organic_carbon  | Quantitativo |
| Trihalomethane  | Quantitativo |
| Turbidity       | Quantitativo |
| Potability      | Qualitativo |

### Analise de distribuição de classes

| Potável | Quantidade | Porcentagem    |
|   ---   |     ---    |       ---      |
| 0 (Não) | 1998       | 61.99%         |
| 1 (Sim) | 1278       | 39.01%         |

![Image](https://media.discordapp.net/attachments/965672339931025468/1086773263969026218/image.png)

Obviamente, o dataset está desbalanceado, pois a quantidade de amostras potáveis é muito menor que a quantidade de amostras não potáveis. Isso pode ser um problema para o modelo de predição, pois ele pode acabar tendendo a classificar as amostras como não potáveis.

### Análise de valores faltantes

| Atributo        | Valores faltantes |
|       ---       |        ---        |
| pH              | 491               |
| Hardness        | 0                 |
| Solids          | 0                 |
| Chloramines     | 0                 |
| Sulfat          | 781               |
| Conductivity    | 0                 |
| Organic_carbon  | 0                 |
| Trihalomethane  | 162               |
| Turbidity       | 0                 |
| Potability      | 0                 |

Como podemos ver, os atributos "pH" e "Sulfat" e "Trihalomethane" possuem vários valores faltantes. Isso pode ser um problema para o modelo de predição, se esses valores forem importantes para a predição podem acabar afetando a classificação.

### Análise de correlação

![Image](https://media.discordapp.net/attachments/965672339931025468/1086799751665680494/image.png)

Não há uma correlação muito forte entre os atributos do dataset, o que é bom para o modelo de predição, pois ele não vai acabar tendendo a classificar as amostras de acordo com um atributo em específico.

### Scatter plot

![Image](https://media.discordapp.net/attachments/965672339931025468/1086802103084798105/image.png?width=706&height=676)

Todos os atributos não possuem uma relação linear forte com o atributo "Potability", Isso só confirma que o dataset não possui uma correlação muito forte entre os atributos, como foi visto na análise de correlação.
