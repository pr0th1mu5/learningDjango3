#### Por que aprender django3?
Framework python mais completo que já estudei. Caso tenha uma ideia legal para complementar esse trabalho, por favor, fique à vontade. O interesse aqui é ensiar a qualquer um que queira aprender.

> Por onde começar?
  1. Você terá que utilizar linux (As explicações aqui apresentadas são feitas em uma distro Linux derivada do ubuntu)
  2. Familiaridade com terminar Linux. Você precisará saber o básico de manipulação de arquivos no terminal linux.
  3. IDE de desenvolvimento? Sim, é legal usar uma. Irei utilizar o vscode mas você pode usar que gostar.

> O que instalar?
  1. VirtualEnv para isolar sua aplicação web do restante do sistema;
  2. Python não versão a apartir da 3;
  3. Django na versão também a partir da 3;

> Ordem das coisas na instalação:
  ##### Instalando VirtualEnv:
  ``` userLinux~$ sudo apt install virtualenv ```
  ##### Instalando o Python 3 no sistema (caso ele não venha já instalado por padrão)
  ``` userLinux~$ sudo apt install python3```
  ##### Criando a pasta que irá isolar o ambiente do sistema já com o python na versão 3
  ``` userLinux~$ virtualenv -p usr/bin/python3.8 devDjango ```
  ##### Ativando o ambiente isolado criado já com Python 3.8
  Nesse momento criamos um ambiente isolado chamado "devDjango" com o comando **virtualenv** já com Python na versão 3 passando como parâmetro o local onde o python3.8 está instalado no meu sistema.
  Para verificar se realmente está com Python 3.8 instalado corretamente, vamos ativar o ambiente isolado conforme abaixo.
  ##### Comando para ativar o ambiente:
  ``` userLinux~$ . devDjango/bin/activate ```
  ##### O que acontece?
  Após realizar essa ativação, você irá perceber que antes do nome do usuário do sistema irá ficar entre parênteses, o nome do diretório dado para o ambiente de isolamento, em nosso caso, devDjango conforme segue.
  ##### Identificação visual do ambiente isolado no terminal
  ```(devDjango)userLinux~$```
  ##### O que vem agora?
  Temos que instalar o django usando um recurso que já foi instalado no momento em que nós criamos nosso ambiente isolado devDjango, o **pip**. Iremos usar ele para instalar o django. Vamos lá!
  ##### Instalando o Django
  ```(devDjango)userLinux~$ pip install django ```
  ##### Verificando a versão do Python e do django instalados
  ###### Python
  ``` (devDjango)userLinux~$ python --version ```
  ###### Django
  ``` (devDjango)userLinux~$ python -m django --version ```
  
  
---
### INICIANDO O DESENVOLVIMENTO E CRIANDO O PRIMEIRO PROJETO DJANGO
###### Para criar nosso projeto django precisamos inserir no terminal com o ambiente ativado o seguinte comando:
``` (devDjango)userLinux~$ django-admin startproject reverFilmes ```
###### Lista de arquivos criados após o comando de criação do projeto é conforme a seguir:
![alt text](https://github.com/pr0th1mu5/learningDjango3/blob/main/git01.png "Arquivos gerados")
