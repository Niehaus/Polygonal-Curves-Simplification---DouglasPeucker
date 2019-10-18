# Polygonal Curves Simplification - DouglasPeucker
 Algoritmo de Simplificação de Curvas Poligonais de DouglasPeucker em Ruby

## 1º Passo: 
 ```
 É dada uma entrada com N pontos, para formar um vetor de pontos com que possuem coordenadas x,y. 
 E também um valor para tolerância, que deve ser o indicador de quais pontos serão eliminados
 nas demais iterações do algoritmo. 
```
## 2º Passo: 
```
 Após ter o vetor de pontos completo, deve-se calcular a equação da reta que passa entre o primeiro ponto 
 do vetor, e o último ponto do vetor. E então deve-se determinar, para todos os pontos dentro do intervalo 
 entre o primeiro e o último, sua distância até essa reta formada, assim, o ponto que possuir a maior distância
 é selecionado. Dessa forma, o algoritmo está pronto para de fato começar a eliminar pontos. 
```
## 3º Passo:
```
 Ao encontrar o ponto de maior distância até essa reta, o algoritmo deve acontecer recursivamente nos 
 seguintes intervalos de pontos, se a maior distância é maior que a tolerância:
       1.	Entre o 1º ponto do vetor, e o ponto mais distante.
       2.	Entre o Ultimo ponto do vetor, e o ponto mais distante.

 Dessa maneira, é gerado um vetor resultado formado pela concatenação dos resultados da recursão para 1 e 2.  
 Caso a maior distância não seja maior que a tolerância, o vetor de pontos resultantes será a concatenação 
 do 1º ponto do vetor, e do  último ponto do vetor daquela chamada da função. 
```
