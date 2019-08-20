# Redes Neurais

![](https://www.bixtecnologia.com.br/home/wp-content/uploads/2018/05/machine-learning-o-que-%C3%A9.png)  
##### Este repositório será atualizado semanalmente, pretendemos compartilhar tudo o que aprendemos para ajudar a comunidade Livre.
By [J.Junqueira](https://github.com/kuroninho), [Sam](https://github.com/Sam-Marx) and [Pedro](https://github.com/ShowTiime).
ㅤㅤ  

Acervo no Telegram: [Clique aqui](https://t.me/AcervoDoSam)

Grupo no Telegram: [Clique aqui](https://t.me/abhackerspace)

* Data prevista para postagens:  
    * Sexta
    * Sábado
    * Assim que possível
    
---

- Redes Neurais
   - [Introdução](https://github.com/Sam-Marx/redes-neurais#introdu%C3%A7%C3%A3o)
      - [O que é uma Rede Neural Artificial](https://github.com/Sam-Marx/redes-neurais#o-que-%C3%A9-uma-rede-neural-artificial)
      - [Aplicações das Redes Neurais Artificiais](https://github.com/Sam-Marx/redes-neurais#aplica%C3%A7%C3%B5es-das-redes-neurais-artificiais)
   - [O Início de Tudo](https://github.com/Sam-Marx/redes-neurais#o-in%C3%ADcio-de-tudo)
      - [O Neurônio Biológico](https://github.com/Sam-Marx/redes-neurais#o-neur%C3%B4nio-biol%C3%B3gico)
      - [O Neurônio Matemático](https://github.com/Sam-Marx/redes-neurais#o-neur%C3%B4nio-matem%C3%A1tico)

- Aprendizado de máquina
   - [Tipos de sistemas do aprendizado de máquina - parte um](https://github.com/Sam-Marx/redes-neurais/blob/master/tutoriais/sistemas_de_aprendizado_parte1.md)

- Outros
   - [Conteúdo recomendado](https://github.com/Sam-Marx/redes-neurais/blob/master/recomendados.md#conteúdos-recomendados)
---

## Introdução

### O que é uma Rede Neural Artificial

Redes neurais artificiais são técnicas computacionais baseados em redes neurais biológicas através de modelos matemáticos inspirados no sistema nervoso central do ser humano. Praticamente são tentativas de replicar o comportamento do cérebro humano, já que é visto como um processador extremamente complexo.

![modelo grafico de uma RNA](https://i.imgur.com/gg28OLm.jpg)

A imagem acima demonstra uma representação gráfica de como é uma rede neural artificial (RNA) profunda (por ter mais de uma camada), também chamada de Deep Learning. A arquitetura da rede acima é chamada de FeedForward (cada camada se conecta à próxima camada, porém não há caminho de volta, ou seja, as camadas têm a mesma direção, à saída), com camada de entrada conectada (os "links" podem ser chamados de pesos) à camadas ocultas (não é nem entrada nem saída; também chamadas de camadas intermediárias) e estas conectadas à camada de saída.

### Aplicações das Redes Neurais Artificiais

As redes neurais artificiais podem ser usadas em diversas áreas, com **classificação**, **predição** e **clustering**.

1. **Classificação**:
   Técnica para categorizar os dados em um número desejado e distinto de classes, onde é possível atribuir um rótulo a cada classe.
   
   Exemplo: reconhecimento de voz.
   
   Tipo de rede normalmente usada: FeedForward.

2. **Predição**:
   Refere-se à saída de um algoritmo depois de ter sido treinado em um conjunto de dados histórico e aplicado em novos dados, a fim de "prever" o resultado através dos dados treinados.

   Exemplo: recomendação de produtos ou filmes.
   
   Tipo de rede normalmente usada: FeedForward.

3. **Clustering**:
   É o conjunto de técnicas de data mining (prospecção de dados) que visa fazer agrupamentos automáticos de dados segundo o seu grau de semelhança.
   
   Exemplo: pode ser usado para classificação entre diferentes espécies de plantas e animais.
   
   Tipo de rede normalmente usada: rede Hemming; Maxnet; redes competitivas.

![foto de dentro do Tesla e o que ele vê](https://www.teslarati.com/wp-content/uploads/2016/11/Tesla-autonomous-self-driving-vision-sensors.jpg)
*Sensores de visão de um carro autônomo da Tesla, usando redes neurais convolucionais (CNN / Convolutional Neural network) para detecção de objetos.*

Na realidade, podem ser usadas em sistemas diferentes, como no comércio (recomendação de produto através de escolhas de usuário), na medicina (reconhecimento de doenças), nos automóveis (carros autônomos) etc.

---

## O Início de Tudo

Na tentativa de criar sistemas inteligentes, uma ideia que vem quase que instantaneamente às nossas cabeças é a de simular o sistema mais rápido e mais potente que conhecemos hoje em dia em máquinas, o cérebro humano. A rede neural, é um ramo do aprendizado de máquina que tenta simular o comportamento do cérebro humano, usando para isso conceitos da álgebra linear, da estatística, do cálculo e da biologia.

Por mais que isso possa assustar de primeira, CALMA!!! Sempre que tento aprender algo que parece extremamente complexo, a abordagem que sigo é a de sempre ir no fundamento da coisa, o famoso “começar do começo”, e é isso que você está fazendo agora, conhecendo o início de uma base de conceitos que irá lhe ajudar a entender melhor as Redes Neurais Artificiais.

### O Neurônio Biológico

Por que então não começar do mais básico? O nosso cérebro faz parte do sistema nervoso, esse por sua vez possui um sistema extremamente complexo de células que são determinantes para a vida dos seres vivos. A unidade fundamental do sistema nervoso é a célula nervosa, ou, como vamos chamá-la daqui em diante, o neurônio.

A estrutura básica de um neurônio é a apresentada na figura abaixo. Nela podemos observar três partes principais, os dendritos (1), que são ramificações onde a principal função é receber estímulos nervosos vindos do ambiente ou, mais comumente, de outros neurônios. Esses estímulos chegam até o corpo celular (2, alguns chamam de soma), onde são processados e por fim vão até o axônio (3) que pega o novo estímulo gerado pelo corpo celular e o envia para outros neurônios através de seus terminais. 

Tais estímulos que são conduzidos pelo axônio e que passa pelos seus terminais, entram em contato com os dendritos de outros neurônios. A esse contato damos o nome de **sinapse**. Assim a nossa rede neural é formada, pela junção de bilhões desses neurônios, que conseguem realizar todo o processamento em frações de segundos.

<p align="center">
  <img src="https://www.sistemanovi.com.br/basenovi/image/ConteudosDisciplinas/5/13/41/300411/neuronio.png">
</p>

É importante conhecermos a ordem de funcionamento do neurônio biológico, visto que ele é a base para o neurônio matemático que se comporta de forma semelhante. Os dendritos e o corpo celular, atuam como uma camada de entrada para o neurônio, onde o estímulo vindo de sensores (retina, papilas, epiderme, etc) ou de outros neurônios chegam aos dendritos e são processados pelo corpo celular. Após isso, esses sinais são encaminhados para o axônio, e ,se forem superior a um limiar de disparo, seguem pelo axônio até os seus terminais. Caso contrário, são considerados irrelevantes e são bloqueados. Os sinais que passam e chegam aos terminais servem como entrada para outros neurônios através da interação terminal axônico ⇒ dendrito.

Foi com essa inspiração que o componente base das redes neurais artificiais foi criado, o neurônio matemático, o qual você vai conhecer agora mesmo.

### O Neurônio Matemático

Assim como o neurônio biológico é a célula base que compõe a rede neural do nosso cérebro, o neurônio matemático é o elemento base para as Redes Neurais Artificiais, e por serem provenientes dos neurônios biológicos, podemos traçar vários paralelos para entendermos melhor o seu funcionamento.

Um neurônio (a partir de agora irei usar apenas a nomenclatura *neurônio* para me referir aos neurônios matemáticos, caso me refira aos neurônios biológicos, deixarei explícito) se parece com o mostrado na figura abaixo e possui um funcionamento bem simples. As unidades de entrada, que simulam os dendritos, recebem os sinais; esses sinais são ponderados pelos seus respectivos pesos sinápticos e combinados por uma função matemática *f*, simulando assim o procedimento realizado pelo corpo celular.

A saída do neurônio faz o papel do axônio, essa saída pode ser a resposta da rede ou pode ser uma conexão com as unidades de entrada de outro neurônio. Essa conexão é justamente a interação entre os terminais do axônio e os dendritos do próximo neurônio, e como vimos anteriormente, essa interação é chamada de sinapse.

<p align="center">
  <img width="600" height="279" src="https://www.researchgate.net/profile/Cesar_Celis4/publication/301290092/figure/fig1/AS:350792205783040@1460646787765/Figura-1-Diagrama-esquematico-do-modelo-matematico-do-neuronio-de-uma-RNA-10-Na_W640.jpg">
</p>

Para entendermos melhor como cada parte do neurônio funciona, vamos aprofundar melhor nos conceitos matemáticos por trás disso. Suponha o objeto *x* com *p* atributos que serão representados na forma de um vetor como *x = [x1, x2, x3, ..., xp]* e um neurônio *n*, como o da figura acima, com *p* terminais de entrada, onde os pesos são *wk1, wk2, ..., wkp* que também podem ser representados de forma vetorial como *w = [wk1, wk2, wk3,..., wkp]*, onde *p* representa a entrada a qual o peso está associado e *k* o neurônio ao qual aquele peso corresponde (em um neurônio, todo o *k* é uma constante, por isso será ocultado das equações que estão por vir). As entradas de um neurônio são ponderadas e passam por uma junção aditiva para gerar a saída que chamaremos de *u*; *u* é a entrada total recebida pelo neurônio *n* e pode ser definido pela equação abaixo:

<p align="center">
   <img src="https://latex.codecogs.com/svg.latex?u&space;=&space;\sum_{j&space;=&space;1}^{p}x_{j}\cdot&space;w_{j}" title="u = \sum_{j = 1}^{p}x_{j}\cdot w_{j}" />
</p>

Se você não é muito familiarizado com essas letras que aparecem em equações matemáticas, eu vou explicar essa equação melhor para você. Suponha que um determinado neurônio possua três terminais de entrada *x = [x1, x2, x3]*, cada entrada possui um peso associado à ela, *w = [w1, w2, w3]*, a primeira função do neurônio é pegar os sinais recebidos e ponderá-los usando seus pesos, ou seja *u = [(x1*w1) + (x2*w2) + (x3*w3)]*.* Os pesos sinápticos, representados pela letra *w*, servem para ponderar as entradas recebidas pelo neurônio, ou seja, alguns estímulos recebidos pelo neurônio podem ser mais importantes que outros e o peso serve justamente para fazer esse ajuste.

Após isso o neurônio passa por uma função de ativação, que irá definir a saída do neurônio. Se o valor resultante da junção aditiva das entradas, que nós definimos sendo *u*, for maior que um certo limiar (threshold), então o neurônio é ativado, caso contrário o neurônio não é ativado. Vale salientar que, na computação, quando nos referimos à ativado e não ativado, ligado e desligado, estamos falando da base binária, ou seja, a saída de um neurônio se comporta de forma binária dada as suas entradas. 

Se o conjunto de entradas, após ponderadas e somadas, ultrapassarem um certo limiar, a  função de ativação gera como saída 1, caso contrário 0. Como podemos ver, a função de ativação tem papel fundamental na saída do neurônio e muitas delas já foram proposta na literatura, hoje falarei das três mais simples, mas em artigos futuros vamos nos aprofundar em outras funções de ativações.

A função linear (a) retorna apenas o valor de *u* (*u* é o soma de todas entradas ponderadas pelos seus respectivos pesos sinápticos). A função limiar (b) é a função em que o limiar (threshold) irá definir a saída da função. Quando a soma das entradas ultrapassa esse limiar, o resultado é igual a 1 e o neurônio é ativado. Quanto maior o limiar, mais difícil será para o neurônio ser ativo. Por último, a função sigmoidal (c) representa uma aproximação contínua e diferencial da função limiar.

<p align="center">
   <img width="600" height="179" src="https://imu.gr/images/2019/08/10/fucntions.md.png" />
</p>

O neurônio matemático pode conter o bias (tendência), -![\theta](https://latex.codecogs.com/svg.latex?\theta) representado na figura abaixo, que é incluído ao somatório das entradas com o intuito de aumentar o grau de liberdade da função de ativação e a capacidade de aproximação da rede. O valor do bias, assim como os dos pesos sinápticos é ajustado durante o aprendizado do neurônio (cenas dos próximos capítulos) e ele possibilita que um neurônio apresente uma saída não nula mesmo se todas as suas entradas forem nulas. Sem isso não seria possível fazer com que o neurônio aprendesse o “ou exclusivo” (![\oplus](https://latex.codecogs.com/svg.latex?\oplus)), algo que mudou o rumo das pesquisas em Rede Neural, mas vamos falar sobre isso depois .

<p align="center">
   <img width="600" height="279" src="https://upload.wikimedia.org/wikipedia/commons/b/b4/Sadssa.png" />
</p>

É assim que o neurônio matemático simula um neurônio biológico e é assim que começa nosso estudo por esse ramo da IA. O neurônio é a unidade básica de tudo que vamos ver pela frente, desde as redes Perceptron e Adaline (que serão nossos próximos objetos de estudo) à Redes Neurais mais complexas, como as Redes Recorrentes, as Redes Convolucionais e a famosas Deep Learning. Além dessas redes básicas, veremos como é o aprendizado de uma rede neural, a partir do algoritmo mais simples de correção de erros e uma amostra da limitação dessas arquiteturas iniciais.

---
