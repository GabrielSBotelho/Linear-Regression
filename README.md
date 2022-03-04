# Projeto de Regressão Linear

> A regressão linear tenta modelar a relação entre duas (ou mais) variáveis ajustando uma equação linear aos dados observados. Para isso um variável é considerada uma variável independente e a outra é considerada uma variável dependente (alvo). Desta forma, o modelo de regressão linear utiliza dos valores da variável independente para prever os valores da variável dependente. 

A linha de regressão linear tem uma equação da forma 

```math
y = a + bx
```

onde
  * x é a variável independente;
  * y é a variável dependente; 
  * b é a inclinação da linha 
  * a é a interceptação (o valor de y quando x = 0).
 

O método mais comum para ajustar uma linha de regressão é o método dos mínimos quadrados. Esse método calcula a linha de melhor ajuste para os dados observados, minimizando a soma dos quadrados dos desvios verticais de cada ponto de dados para a linha (se um ponto estiver exatamente na linha ajustada, seu desvio vertical será 0) [[1]](http://www.stat.yale.edu/Courses/1997-98/101/linreg.htm#:~:text=Linear%20regression%20attempts%20to%20model,to%20be%20a%20dependent%20variable.).

--- 

## NYC Taxi Trip Duration

O *dataset* contém informações sobre o registro de viagens do *Yellow Cab* em 2016 em Nova York disponibilizados no *Big Query* no *Google Cloud Platform*.

O *dataset* conta com os seguintes atributos
  
  * `id`: o identificador de vada viagem realizada;
  * `vendor_id`: um código indicando o provedor associado ao registro de viagem;
  * `pickup_datetime`: data e hora em que o medidor foi inciado;
  * `dropoff_datetime`: data e hora em que o medidor foi finalizado;
  * `passenger_count`: o número de passageiros no veículo (valor inserido pelo motorista);
  * `pickup_longitude`: a longitude do local de partida da viagem onde o medidor foi inciado;
  * `pickup_latitude`: a latitude do local de partida da viagem onde o medidor foi inciado;
  * `dropoff_longitude`: a longitude do local de chegada da viagem onde o medidor foi desligado;
  * `dropoff_latitude`: a latitude do local de chegada da viagem onde o medidor foi desligado;
  * `store_and_fwd_flag`: indica se o registro da viagem foi retido na memória do veículo antes de ser enviado ao fornecedor
  * trip_duration: duração da viagem (em segundos).

O *dataset* pode ser encontrado [aqui](https://www.kaggle.com/yasserh/nyc-taxi-trip-duration).

Caso não consiga visualizar o notebook, acesse este [link](https://nbviewer.org/github/GabrielSBotelho/Linear-Regression/blob/main/NYC_Taxi_Duration.ipynb) ou acesse diratamente no [google colab](https://colab.research.google.com/drive/170KUP1j-kwgVFM3QAJS8GkHKj7i4sODh?usp=sharing).
