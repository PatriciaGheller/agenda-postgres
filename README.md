# Agenda CLI com PostgreSQL

Este projeto é uma aplicação de linha de comando (CLI) desenvolvida em **Python** utilizando a biblioteca **psycopg2** para integração com o banco de dados **PostgreSQL**.  
O objetivo é demonstrar operações **CRUD** (Create, Read, Update, Delete) de forma prática, eficiente e segura.

# 📋 Pré-requisitos

Antes de rodar a aplicação, certifique-se de ter instalado e configurado:

- **Python 3.10** (ou superior)  
  - Recomenda-se criar um ambiente virtual com `venv`:
    ```powershell
    python -m venv venv310
    .\venv310\Scripts\Activate.ps1
    ```

- **PostgreSQL 16** (ou versão compatível)  
  - Durante a instalação, configure o usuário `postgres` com uma senha (ex.: `admin123`).  
  - Certifique-se de que o serviço PostgreSQL está em execução.  

- **Pacote psycopg2-binary**  
  - Instale dentro do ambiente virtual:
    ```powershell
    pip install psycopg2-binary
    ```

- **Banco de dados e tabela**  
  - Conecte-se ao banco `postgres`:
    ```powershell
    & "C:\Program Files\PostgreSQL\16\bin\psql.exe" -U postgres -h localhost -p 5432 -d postgres
    ```
  - Crie a tabela `AGENDA`:
    ```sql
    CREATE TABLE public."AGENDA" (
        id SERIAL PRIMARY KEY,
        nome VARCHAR(100) NOT NULL,
        telefone VARCHAR(20) NOT NULL
    );
    ```


## 🚀 Funcionalidades
- Adicionar novos contatos
- Listar todos os contatos
- Atualizar informações de um contato existente
- Deletar contatos
- Interface simples via linha de comando

## 🛠️ Tecnologias utilizadas
- Python 3.10+
- PostgreSQL
- psycopg2

## 📦 Instalação
1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/agenda-cli-postgres.git

2. Instale as dependências:
    pip install psycopg2

3. Configure o banco de dados PostgreSQL:

sql
```
    CREATE TABLE public."AGENDA" (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(100),
    telefone VARCHAR(20)
);
```
# ▶️ Uso

Ative o ambiente virtual (se ainda não estiver ativo):

```powershell
.\venv310\Scripts\Activate.ps1

python crud_app.py 
```


---

🎯 Assim, quem baixar seu repositório vai saber que:
1. Precisa ativar o ambiente virtual.  
2. O arquivo correto para rodar é `crud_app.py`.  

# 🗄️ Configuração do Banco de Dados

Antes de executar o programa, é necessário criar a tabela `AGENDA` no banco de dados PostgreSQL.

1. Conecte-se ao banco `postgres` com o usuário padrão:
   ```powershell
   & "C:\Program Files\PostgreSQL\16\bin\psql.exe" -U postgres -h localhost -p 5432 -d postgres

2. Dentro do prompt psql, crie a tabela:

Sql
```
CREATE TABLE public."AGENDA" (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    telefone VARCHAR(20) NOT NULL
);
```
3. Verifique se a tabela foi criada:

Sql
```
\dt
```
4. (Opcional) Insira alguns contatos de exemplo:

Sql
```
INSERT INTO public."AGENDA" (nome, telefone) VALUES ('Patricia', '21999999999');
INSERT INTO public."AGENDA" (nome, telefone) VALUES ('Davi', '21988888888');
```
5. Agora você já pode rodar o programa normalmente:

Powershell
```
python crud_app.py
```
---
🎯 Assim, quem baixar seu repositório vai saber:

- Que precisa ter Python e PostgreSQL instalados.

- Que deve instalar o pacote psycopg2-binary.

- Que deve criar a tabela AGENDA antes de rodar o programa.





## 📌 Objetivo

Este projeto foi criado para fins de estudo e prática de integração entre Python e PostgreSQL, servindo como base para aplicações mais complexas.




