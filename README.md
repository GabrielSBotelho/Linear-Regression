# Projetos de Regressão Linear

A regressão linear é realizada a a partir do aprendizado supervisionado, ou seja, necessita de dados de entrada que são apresentados na forma de pares ordenados (entrada e saída). O algoritmo de regressão linear é utilizado para prever dados contínuos. Ele tenta escolher os melhores valores para os coeficientes de forma a minimizar a media dos quadrados dos erros (MSE). A fórmula utilizada na regressão linear para criação da reta é `y = a + bx`, sendo 

- `y`, o valor estimado
- `a`, o coeficiente da linear *(altura da reta)*
- `b`,  a inclinação da reta

A *MSE* é obtida a partir do seguinte calculo 

![image](https://user-images.githubusercontent.com/27251597/157294964-50575c92-beee-46c9-9477-03d2118ae1a4.png)

sendo,

- `n`, a quantidade de registros
- `Yi`, o valor real dos dados de entrada seguindo a fórmula da regressão linear
- `ŷi`, o valor estimado pelo algoritmo
    - OBS: é elevado ao quadrado para casos em que a diferença seja negativa

Esse calculo por ser chamado de *função custo*. Desta forma, é criado um gráfico entre a função custo e o valor de `a`  (Função beta) analisado, ao final é procurado o valor de `a` que minimiza ao máximo os valores obtidos no gráfico. 

### Gradiente Descendente

É gráfico gerado quando é computado a função custo em relação a função beta. Através dele é realizada a busca pelo menor valor possível para `a`. Isso é possível através da `derivação dos valores do MSE * taxa de aprendizado (alfa)`. A partir deste calculo é convergido/divergido a reta para o valor do mínimo global, ou seja, o menor valor possível da função de custo. 

- Obs:
    - A taxa de aprendizagem é uma constante;
    - Os valor de `a` e `b` são atualizados juntos.

### Regressão Linear Multivariada

Utiliza mais de uma feature para descobrir o valor ideal da variável target. 

A fórmula da regressão linear multivariada é:

![image](https://user-images.githubusercontent.com/27251597/157295092-1d47f1f3-efa2-4685-8d6a-50afc0d6311e.png)

### *BIAS*, *Underfit/Overfit* & Variância

O *BIAS* é a incapacidade do método de machine learning de capturar a verdadeira relação entre as variáveis.

A Variância é a avaliação dos resultados entre diferentes datasets. Pode se pensar como a *consistência*, ou seja, uma alta variância resulta em uma baixa consistência, e uma baixa variância resulta em uma alta consistência do modelo.

*Overfit* acontece quando os modelo na base de treino tem um baixo *BIAS*, mas ao mesmo tempo tem uma alta Variância.

*Uderfit* acontece quando o modelo na base de treino tem um alto *BIAS*, mas ao mesmo tempo tem uma baixa Variância.

O ideal método de machine learning é aquele com baixo *BIAS*, pois consegue tem um melhor da relação das variáveis. Assim como, também deve ter uma baixa variância, de forma que ao trocar a base de dados ele se mantenha mais consistentes na previsão dos resultados.

Pode ser utilizado de 3 métodos para auxiliar na chegada desse aspecto, bem como encontrar o ponto ideal entre o simple e complexo, sendo eles:

- Regularização
- *Boosting*
- *Bagging*

### *Cross Validation*

A técnica de  *cross validation* (validação cruzada) realiza a criação e avaliação do modelo a partir de todas as combinações possíveis de treino e teste. Desta forma, o *cross validation* permite comparar diferente métodos de machine learning e obter o senso de quão bem eles trabalham na prática. 

O *cross validation* também é útil:

- na seleção de features, ao avaliar modelos com diferentes features
- no *model tuning*, ao alterar os valores dos parâmetros para avaliar qual o melhor.



Caso não consiga visualizar o notebook do projeto NYC Taxi Trip Duration, acesse este [link](https://nbviewer.org/github/GabrielSBotelho/Linear-Regression/blob/main/NYC_Taxi_Duration.ipynb) ou acesse diratamente no [google colab](https://colab.research.google.com/drive/170KUP1j-kwgVFM3QAJS8GkHKj7i4sODh?usp=sharing).
