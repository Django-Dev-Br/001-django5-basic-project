
# 001 Django 4 Basic Project

### O que é um Projeto Django?

Um projeto Django é a estrutura básica para construir uma aplicação web com o framework Django. Ele é uma coleção de configurações e pacotes para um sistema web com python. 

### O que é o PIP?

O pip é um gerenciador de dependências do Python. Ele baixa e instala, automaticamente, pacotes de [https://pypi.org/](https://pypi.org/) para seu projeto Python. O PyPi é o repositório oficial de pacotes Python. O Próprio Django é composto por vários pacotes, formando assim um framework. Essa é a descrição técnica de um Framework, ou seja, um conjunto de pacotes. 

### O que é um Virtual Environment (Ambiente Virtual ou venv)?

Um ambiente virtual é um container de isolamento para instalação de pacotes python. Na prática, é uma pasta ou diretório no Sistema operacional. Ela permite que as instalações sejam feitas nela e não no computador. Isso permite que vc trabalhe com diferentes versões da linguagem Python e diferente pacotes e respectivas versões em difentes ambientes, evitando qualquer conflito e/ou incompatibilidade. 


## COMO RODAR ESSE PROJETO EM SEU COMPUTADOR:

### Requisitos

- **Python 3.12**  
  [Baixar Python 3.12](https://www.python.org/downloads/release/python-3122/)

  Confira o vídeo para saber como trabalhar com múltiplas versões do Python e com venv (ambiente virtual):
 [![Watch the video](https://img.youtube.com/vi/eetDeQrv0Rs/0.jpg)](https://youtu.be/eetDeQrv0Rs)

- **Virtualenv**

  Para instalar o pacote `virtualenv` no Python, utilize os seguintes comandos:

  - **Linux**:
    ```bash
    python3 -m pip install virtualenv
    ```

  - **Windows**:
    ```bash
    python -m pip install virtualenv
    ```

### Passos para Executar

1. **Clone o repositório**:
    ```bash
    git clone https://github.com/Django-Dev-Br/001-django4-basic-project.git
    ```

2. **Crie  um ambiente virtual no diretório root**:

   **Windows**
    ```bash
     python -m venv myvenv  # Windows
    ```
      **Linux**
     ```bash
     python3 -m venv myvenv  # Linux
    ```

4. **Ative o ambiente virtual criado**:

   **Windows**
    ```bash
    myvenv\Scripts\activate  # Windows
    ```

     **Linux**
    ```bash
    source myvenv/bin/activate  # Linux
    ```

6. **Instale o Django**:

   Fazer a instalação após a ativação da virtual env fará com que a instalação seja feita nessa pasta ao invés do computador. Isso significa que o pacote Django não estará disponivel para todos os usuários do computador, mas apenas para o contexto no qual essa venv esteja ativada. Veremos sua ativação logo abaixo.

    **Instalação via gerenciador de dependências PIP**
    ```bash
    pip install django==4.2.15
    ```
    ----- **OU** -----

    **Instalação via arquivo requirements**
    ```bash
    pip install -r requirements.txt
    ```
    O arquivo requirements.txt é um arquivo de texto que contém uma lista de pacotes a ser instalado em uma venv. É uma boa prática de programação do ecossistema Python.

7. **Acesse a pasta do projeto Django**:
    ```bash
    cd 001-django4-basic-project
    ```

8. **Execute o servidor de desenvolvimento**:
    ```bash
    python manage.py runserver
    ```

### Acesse no seu navegador o endereço a seguir:

http://127.0.0.1:8000/


###  Após executar o servidor, você deve ver a página inicial padrão do Django, semelhante à django_running.png acima


### Estrutura de Diretórios do Projeto

```
001-django4-basic-project/
├── myproject/
│   ├── __init__.py      # Marca o diretório como um pacote Python, o que permite a importação de outros módulos
│   ├── asgi.py          # Configurações para o servidor ASGI (usado para aplicações assíncronas)
│   ├── settings.py      # Configurações do projeto (banco de dados, apps instalados, etc.)
│   ├── urls.py          # Mapeamento de requisições https e redirecionamento para os templates html
│   └── wsgi.py          # Configurações para o servidor WSGI (usado para servir a aplicação)
└── manage.py            # CLI (Command line interface) do Django, ou seja, um script de linha de comando que recebe e executa os comandos do Django via terminal (linha de comando)
└── requirements.txt     # arquivo de texto com uma lista de pacotes python. 
```
### OBS: Como Criar um Projeto Django

Se desejar criar seu próprio projeto Django, use o seguinte comando após criar e ativar a virtual env e instalar o django nela, conforme orientações acima:

  ```bash
  django-admin startproject myproject
  ```
O comando acima cria o projeto em uma subpasta myproject

**OU**

  ```bash
  django-admin startproject myproject .
  ```
O comando acima cria os arquivos do projeto Django na pasta atual. Não cria uma subpasta com o mesmo nome do projeto, no caso, "myproject".

### OBS: Como criar um arquivo de requirements.txt?

  Após ativar um venv e instalar pacotes neles, é possível salvar a lista dessas instalações no arquivo requirements.txt. Para isso, utilize o comando:
    
    ```bash
    pip freeze > requirements.txt
    ```
    
  Esse comando exporta todas as dependências instaladas em um venv para o arquivo requirements.txt.

### Sobre Nosso Treinamento Prático-Profissional com projeto real para iniciantes e avançados em web DevOps Full-stack com Python, Django, Bootstrap e Linux. 

[Django Developers Brasil - Aprenda programando enquanto programa aprendendo!](https://django.dev.br/)

Nosso treinamento oferece uma experiência prática de aprendizado de programação, adequada tanto para iniciantes quanto para desenvolvedores avançados. Você participará de um projeto real de desenvolvimento de software em um ambiente corporativo autêntico, onde pessoas com diferentes níveis de conhecimento irão colaborar, aprendendo umas com as outras.

### Junte-se a nós! 
E desenvolva as habilidades necessárias para o mercado de trabalho, aprimorando tanto seus conhecimentos técnicos quanto suas soft skills em um ambiente colaborativo e realista.
