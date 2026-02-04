# Agenda CLI com PostgreSQL

Este projeto é uma aplicação de linha de comando (CLI) desenvolvida em **Python** utilizando a biblioteca **psycopg2** para integração com o banco de dados **PostgreSQL**.  
O objetivo é demonstrar operações **CRUD** (Create, Read, Update, Delete) de forma prática, eficiente e segura.

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
    CREATE TABLE public."AGENDA" (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(100),
    telefone VARCHAR(20)
);

# ▶️ Uso

Execute o programa:

python main.py

## 📌 Objetivo

Este projeto foi criado para fins de estudo e prática de integração entre Python e PostgreSQL, servindo como base para aplicações mais complexas.




