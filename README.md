# Django User Management

Este projeto é um sistema de autenticação e gerenciamento de usuários desenvolvido com Django. Ele serve como exemplo para introdução aos principais recursos de autenticação, cadastro e administração de usuários em aplicações web.

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Funcionalidades](#funcionalidades)
- [Instalação](#instalação)
- [Como Usar](#como-usar)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Dependências](#dependências)
- [Contribuindo](#contribuindo)
- [Licença](#licença)

---

## Sobre o Projeto

Este repositório apresenta uma aplicação Django focada em autenticação de usuários, incluindo cadastro, login, redefinição e alteração de senha. É ideal para quem quer aprender a implementar autenticação de forma prática e personalizável.

## Funcionalidades

- Cadastro de novos usuários
- Login e logout
- Redefinição de senha via email
- Mudança de senha para usuários autenticados
- Dashboard restrito a usuários autenticados

## Instalação

1. Clone o repositório:
   ```sh
   git clone https://github.com/carvalhocaio/django-user-management
   cd django-user-management
   ```

2. Crie e ative um ambiente virtual:
   ```sh
   python -m venv .venv
   source .venv/bin/activate  # No Windows use .venv\Scripts\activate
   ```

3. Instale as dependências:
   ```sh
   pip install -r requirements.txt
   ```

4. Aplique as migrações:
   ```sh
   python manage.py migrate
   ```

5. Inicie o servidor de desenvolvimento:
   ```sh
   python manage.py runserver
   ```

6. Acesse o projeto em [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## Como Usar

- Acesse `/accounts/register/` para criar uma nova conta.
- Faça login em `/accounts/login/`.
- Para redefinir sua senha, utilize `/accounts/password_reset/`.
- Usuários autenticados terão acesso ao dashboard e poderão alterar sua senha.

## Estrutura do Projeto

```
├── manage.py
├── requirements.txt
├── user_auth_intro/
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── users/
    ├── admin.py
    ├── apps.py
    ├── forms.py
    ├── migrations/
    ├── models.py
    ├── templates/
    ├── tests.py
    ├── urls.py
    └── views.py
```

- **user_auth_intro/**: Configurações principais do projeto Django.
- **users/**: App responsável pela lógica de autenticação, cadastro, views e templates de usuário.
- **requirements.txt**: Lista de dependências do projeto.

> **Nota:** Para detalhes completos da estrutura de pastas, acesse o [repositório no GitHub](https://github.com/carvalhocaio/django-user-management/tree/main).

## Dependências

Principais pacotes utilizados:
- Django 5.1.5
- asgiref
- sqlparse
- typing-extensions

Veja o arquivo [`requirements.txt`](https://github.com/carvalhocaio/django-user-management/blob/main/requirements.txt) para a lista completa.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

## Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
