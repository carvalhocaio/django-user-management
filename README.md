# User Authentication

Este é um projeto de exemplo para introduzir a autenticação de usuários usando Django.

## Configuração

1. Clone o repositório:
    ```sh
    git clone https://github.com/carvalhocaio/django-user-management
    cd django-user-management
    ```

2. Crie um ambiente virtual e ative-o:
    ```sh
    python -m venv .venv
    source venv/bin/activate  # No Windows use `venv\Scripts\activate`
    ```

3. Instale as dependências:
    ```sh
    pip install -r requirements.txt
    ```

4. Execute as migrações:
    ```sh
    python manage.py migrate
    ```

5. Inicie o servidor de desenvolvimento:
    ```sh
    python manage.py runserver
    ```

6. Acesse o projeto em `http://127.0.0.1:8000/`.

## Funcionalidades

- Cadastro de usuários
- Login e logout
- Redefinição de senha
- Mudança de senha
- Dashboard para usuários autenticados

## Estrutura de Templates

- `base.html`: Template base para todas as páginas.
- `registration/`: Templates relacionados à autenticação de usuários.
- `dashboard.html`: Dashboard para usuários autenticados.

---
