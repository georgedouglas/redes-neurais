# Tipos de sistemas do aprendizado de máquina
![](https://www.wrprates.com/wp-content/uploads/2018/09/o-que-e-machine-learning.jpg)
Parte 1/2

Existem diferentes tipos de sistema de aprendizado de máquinas, iremos classificá-las com base em algumas características:  
* Se são treinadas com supervisão ou sem supervisão (Será explicado mais a frente.)
* Se podem aprender continuamente de forma incremental ou não.

Esses critérios não são exclusivos e podem ser usados em conjunto, como um filtro de spam que faz o uso do aprendizado online e o de modelos.  
Iremos falar apenas dos principais/mais usados sistemas atualmente.

## Aprendizado Supervisionado e Não supervisionado:

Podemos classificar o sistema com base no tipo de supervisão que recebe durante o treino. Existem 4 categorias principais: Supervisionado, Não supervisionado, semi-supervisionado e por reforço.

### Aprendizado Supervisionado
No aprendizado supervisionado, como você pode imaginar, o treinamento é feito por nossa supervisão, o que significa que damos os dados e rótulos a eles, que são as soluções que esperamos do algoritmo.

* A **classificação** é uma tarefa na qual você fornece os rótulos e os dados em um conjunto finito e não ordenado, tendo o algoritmo treinado o suficiente ele deve ser capaz de aprender a classificar novos dados.  
Exemplo: Filtro de Spam

* A **Regressão** é uma tarefa na qual o algoritmo tenta prever um valor numérico a partir de um conjunto de características denominadas __previsores__
Exemplos: Preço de um carro de acordo com sua (idade, quilometragem, marca, tempo de uso)  
![](https://miro.medium.com/max/700/1*GZ85Pfb2-PRKaLYFjGHUvA.png)

* A **Regressão Linear** usará os pontos de dados para encontrar o melhor modelo linear para os seus dados. A regressão linear simples utiliza apenas 1 variável independente, enquanto a Regressão linear múltipla define várias.  
Exemplos: Classificar notas de alunos de acordo com a quantidade de horas estudadas  
![](https://upload.wikimedia.org/wikipedia/commons/4/41/LinearRegression.svg)

* A **Regressão Logística** estima a probabilidade associada à ocorrência de determinado evento   
Exemplo: Prever se a chuva irá ocorrer ou não  
![](https://estatsite.files.wordpress.com/2018/08/320px-logistic-curve.png)

* **Outros** importantes porém não abordados: k-Nearest Neighbours, Máquinas de Vetores de Suporte, Árvores de decisão, Florestas Aleatórias e Redes Neurais.

### Aprendizado Não Supervisionado
No aprendizado não supervisionado os dados não são rotulados. O sistema aprende sem saber qual o resultado esperado.

* **Clustering** 
    - Na verdade o Clustering é um conjunto de técnicas que visa fazer agrupamentos automáticos de acordo com seu grau de semelhança.  
    Exemplos: K-means, Clustering Hierárquico [HCA, do inglês] e Maximização de Expectativa.  
    ![](https://i.imgur.com/S65Sk9c.jpg)
    
* **Visualização e redução da dimensionalidade**
    - A visualização é um algoritmo no qual você os alimenta com muitos dados complexos e não rotulados e eles exibem um representação 2d ou 3d de seus dados que podem facilmente serem plotados.  
    Exemplos: tdistributed Stochastic Neighbor Embedding(t-SNE), Locally-Linear Embedding(LLE)
    - A redução de dimensionalidade é uma tarefa relacionada na qual o objetivo é simplificar os dados sem perder muita informação.  
    Exemplos: Kernel PCA, Análise de Componentes Principais[PCA, do inglês]
    ![](https://i.stack.imgur.com/g6LHQ.png)

* **Detecção de anomalias**
    - O sistema é treinado com instâncias normais e, quando vê uma nova instância, pode dizer se ela parece normal ou se é uma provável anomalia.  
    Exemplos: Detectar defeitos de fabricação, transações incomuns em cartões de crédito.  
    ![](http://zerum.com/wp-content/uploads/2018/09/grafico-detec%C3%A7%C3%A3o-anomalias-rede-com-machine-learning.png)
    Imagem by: Zerum.com
    
* **Aprendizado de Regras de Associação** 
    - É uma tarefa na qual o objetivo é se aprofundar em grandes dados e descobrir relações interessantes entre atributos. Como uma associação Se-Então.  
    Exemplo: **Se** um comprador compra carne de churrasco e sal **então** ele comprará carvão. Modelos assim são comumente usados em mercados.  
    ![](https://i0.wp.com/www.datageeks.com.br/wp-content/uploads/2019/06/Aprendizagem-de-regras-de-associa%C3%A7%C3%A3o.png?w=350&ssl=1)
    
### Aprendizado Semi-supervisionado

O aprendizado Semi-supervisionado é basicamente uma junção de algoritmos supervisionados e não supervisionados.  
Exemplo: Google Photos que reconhece automaticamente uma pessoa em diversas fotos, você pode rotular a pessoa somente uma vez e ele reconhecerá ela em todas.

### Aprendizado por Reforço

* O **sistema de aprendizado por reforço** chama-se agente e pode observar o ambiente, selecionar e executar ações e obter recompensas em troca - ou penalidade na forma de recompensas negativas. Ele deve aprender por si só qual é a melhor estratégia para o maior número possível de recompensas ao longo do tempo.  
Exemplos: O Victor Dias é um  mestre no aprendizado por reforços, você pode ver um (ou vários) vídeo(s) dele [aqui](https://www.youtube.com/watch?v=gnfkfUQvKDwhttps://www.youtube.com/watch?v=gnfkfUQvKDw)!


### Parte 2 em breve! 
Ei, que tal participar do nosso grupo no Telegram?  
Fontes usadas para a criação desse tutorial:  
Wikipedia  
Aprendizado de Máquina com Scikit-learn & Tensorflow, do Aurélien Géron  
Link [aqui](t.me/abhackerspace)
