
# 001 Django 4 Basic Project

## COMO RODAR ESSE PROJETO EM SEU COMPUTADOR:

### Requisitos

- **Python 3.12**  
  [Baixar Python 3.12](https://www.python.org/downloads/release/python-3122/)

  Confira o vídeo para saber como trabalhar com múltiplas versões do Python e com venv (ambiente virtual): [Trabalhando com Múltiplas Versões do Python + venv](https://youtu.be/eetDeQrv0Rs?si=rAIDmLCgdeh7ouXa)

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
    cd 001-django4-basic-project
    ```

2. **Crie  um ambiente virtual**:
    ```bash
     python3 -m venv myvenv  # Linux
     python -m venv myvenv  # Windows
    ```

4. **Ative o ambiente virtual criado**:
    ```bash
    source myvenv/bin/activate  # Linux
    myvenv\Scripts\activate  # Windows
    ```

5. **Instale o Django**:
    ```bash
    pip install django==4.2.15
    ```

6. **Execute o servidor de desenvolvimento**:
    ```bash
    python manage.py runserver
    ```

### Acesse no seu navegador o enderço a seguir:

http://127.0.0.1:8000/


###  Após executar o servidor, você deve ver a página inicial padrão do Django, semelhante à django_running.png acima

### O que é um Projeto Django?

Um projeto Django é uma coleção de configurações e aplicativos para um site web específico. É a estrutura báisca para construir uma aplicação web com o framework Django. 

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

```

### Sobre Nosso Treinamento Prático-Profissional com projeto real para iniciantes e avançados em web DevOps Full-stack com Python, Django, Bootstrap e Linux. 

[Django Developers Brasil - Aprenda programando enquanto programa aprendendo!](https://django.dev.br/)

Nosso treinamento oferece uma experiência prática de aprendizado de programação, adequada tanto para iniciantes quanto para desenvolvedores avançados. Você participará de um projeto real de desenvolvimento de software em um ambiente corporativo autêntico, onde pessoas com diferentes níveis de conhecimento irão colaborar, aprendendo umas com as outras.

**Junte-se a nós!** E desenvolva as habilidades necessárias para o mercado de trabalho, aprimorando tanto seus conhecimentos técnicos quanto suas soft skills em um ambiente colaborativo e realista.
