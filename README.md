# Projeto Produtos

Este repositório consiste em uma aplicação de gerenciamento e manipulação de produtos. O projeto combina scripts de banco de dados PostgreSQL, rotas/endpoints para visualização e cadastro em PHP, além de utilitários em Python para processamento de dados.

---

## 🛠️ Tecnologias Utilizadas

* **PHP:** Responsável pela lógica da aplicação web e integração backend.
* **Python:** Utilizado para scripts auxiliares ou automações do projeto.
* **PostgreSQL:** Banco de dados relacional para persistência de dados.

---

## 📁 Estrutura do Repositório

```text
projetoprodutos/
├── .gitignore                      # Arquivos e pastas ignorados pelo Git
├── CREATE TABLE produtos(.pgsql    # Script de criação da tabela no PostgreSQL
├── produtos.php                    # Script PHP para listagem/manipulação de produtos
└── projeto.py                      # Script em Python com funções do sistema   

🚀 Como Executar o Projeto
Pró-requisitos
Antes de começar, certifique-se de ter instalado em sua máquina:

PHP 8.x+

Python 3.x+

Servidor de Banco de Dados PostgreSQL

1. Configuração do Banco de Dados
Abra o gerenciador de banco de dados PostgreSQL de sua preferência (ex: pgAdmin, DBeaver) ou utilize o terminal via psql.

Execute o script contido no arquivo CREATE TABLE produtos(.pgsql para estruturar a tabela necessária:

SQL
CREATE TABLE produtos (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    preco NUMERIC(10, 2) NOT NULL,
    quantidade INT DEFAULT 0
);
2. Configuração e Execução da Aplicação PHP
Certifique-se de alterar as credenciais de conexão com o banco de dados dentro do arquivo produtos.php (se aplicável).

Inicie o servidor embutido do PHP na raiz do projeto:

Bash
php -S localhost:8000
Acesse a aplicação no seu navegador:
http://localhost:8000/produtos.php

3. Execução dos Scripts Python
Para rodar o script auxiliar em Python:

Bash
python projeto.py
📄 Licença
Este projeto está sob a licença aberta para estudos e modificações.