![](https://chatterbot.readthedocs.io/en/stable/_images/banner.png)
### Como criar o seu primeiro bot em Python com Machine Learning.  
Hoje vamos ver como criar um bot básico em Python, para facilitarmos esse processo usaremos a biblioteca Chatterbot.

Mas o que é "Chatterbot"?  
> O ChatterBot é uma biblioteca Python que facilita a geração de respostas automatizadas para a entrada de um usuário. O ChatterBot usa uma seleção de algoritmos de aprendizado de máquina para produzir diferentes tipos de respostas. Isso facilita para os desenvolvedores criar bots de bate-papo e automatizar conversas com usuários. Para obter mais detalhes sobre as idéias e conceitos por trás do ChatterBot, consulte o [fluxograma](https://chatterbot.readthedocs.io/en/stable/#process-flow-diagram) do processo.  
>Exemplo básico de entrada típica seria algo assim:
>Um exemplo de entrada típica seria algo assim:

```
user: Good morning! How are you doing?
bot:  I am doing very well, thank you for asking.
user: You're welcome.
bot:  Do you like hats?
```
>### Como funciona o ChatterBot:  
>
>O ChatterBot é uma biblioteca Python projetada para facilitar a criação de software que possa envolver-se em conversas.
>
>Uma instância não treinada do ChatterBot começa sem nenhum conhecimento de como se comunicar. Cada vez que um usuário digita uma instrução, a biblioteca salva o texto inserido e o texto em que a instrução respondeu. Como o ChatterBot recebe mais informações, o número de respostas que ele pode responder e a precisão de cada resposta em relação ao aumento da declaração de entrada.
>
>O programa seleciona a resposta correspondente mais próxima pesquisando a declaração conhecida mais próxima que corresponda à entrada e, em seguida, escolhe uma resposta da seleção de respostas conhecidas para essa instrução.

## Instalação:  
#### Pelo PyPi:
```pip install chatterbot```  
#### Pelo github:  
Versão de **desenvolvimento** do ChatterBot:
```
pip install git+git://github.com/gunthercox/ChatterBot.git@master
```
####Verificando a versão do ChatterBot que você instalou:   
Se você já possuir o ChatterBot instalado e quiser verificar qual versão está instalada, execute o seguinte comando.
```
python -m chatterbot --version
```

## Mãos à obra!
Primeiro vamos criar nossa arquivo .py do qual usaremos para criar o bot, você pode usar 'bot.py' ou 'main.py', não importa. Após criarmos o arquivo nós poderemos começar a escrever novas primeiras linhas de código.  
Primeiro iremos importar as bibliotecas necessária para o bom funcionamento do bot:
```python3
from chatterbot import ChatBot  # Para criarmos nosso bot
from chatterbot.trainers import ListTrainer  # Para treinarmos nosso bot
```
A classe chatterbot possui os dois métodos que usaremos para criarmos nosso bot, existem várias outras, mas não usaremos
neste **tutorial básico**. Feito as importações iremos definir o nosso bot.
```python
bot = ChatBot('Gideon')
```
Definimos nosso bot **Gideon**, você pode nomeá-lo como quiser, preferimos usar esse nome por questões pessoais.  
Após definirmos o nosso bot iremos criar uma lista com uma conversação básica  
```python
basic_chat = ['olá',
    'tudo bom?',
    'claro, tudo ótimo!',
    'isso é bom!',
    'você gosta de café?',
    'sim, eu amo!']
```  
Com nossa lista criada vamos definir quem será treinado e com o que:
```python
trainer = ListTrainer(bot)  # Quem será treinado
trainer.train(basic_chat)  # Com o que será treinado
```
Feito isso precisamos criar um looping infinito para que possamos conversar com o bot, não é mesmo?
```python
while True:  # 1
    try:
        user = input('Você: ')  # 2
        response = bot.get_response(user)  # 3
        print(f'Gideon: {response}')  # 4
    except(KeyboardInterrupt, EOFError, SystemExit):  #  5
        break
```
No código anterior fizemos o seguinte:
1. Criamos um looping infinito
2. Pegamos um input do usuário e colocamos numa variável chamada ```user```  
3. Criamos uma variável chamada ```response``` , que guarda a resposta do input do usuário armazenada na variável ```user```
4. Printamos a resposta do bot
5. Adicionamos excessões para que o bot encerre.
6. (Opcional) Você pode adicionar cores ao output do bot alterando o print da seguinte forma:
```python
print(f'\033[0;33mGideon: {response}\033[m')
```
 Assim você terá uma resposta em amarelo.
 ### Visão geral do bot.
 Tendo feito corretamente todos os passos anteriores, teremos um código como esse:
 ```python
from chatterbot.trainers import ListTrainer
from chatterbot import ChatBot

bot = ChatBot('Gideon')

basic_chat = ['olá',
    'tudo bom?',
    'claro, tudo ótimo!',
    'isso é bom!',
    'você gosta de café',
    'tem como não gostar?']

trainer = ListTrainer(bot)
trainer.train(basic_chat)

while True:
    try:
        user = input('Você: ')
        response = bot.get_response(user)
        print(f'\033[0;33mGideon: {response}\033[m')
    except(KeyboardInterrupt, EOFError, SystemExit):
        break
```

# Conclusão
Fizemos um bot básico para uso em CLI (Command Line Interface / Inteface de Linha de Comando), você pode iniciá-lo usando o seguinte comando no seu terminal:
```shell script
$ python3 bot.py
```
> O nosso bot não possui treino e muitas outras funções que seriam muito legais colocar para ficar um bot **fodão!**, por quê?  

Porque, bem, faremos isso em futuras postagens, não sei se você, leitor, sabe, mas pequenos tutoriais como esse que você acabou de consumir levam um considerável tempo para serem feitos!  
E eu acho melhor partir o conteúdo para que o aprendizado não fique maçante!

Prometo trazer mais!

- Escrito por: Kurono
- Revisão e correção: Sam Marx