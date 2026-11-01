# CRUD de Usuários em PHP

Uma aplicação web simples para gerenciamento de cadastros (Criar, Ler, Atualizar e Deletar) desenvolvida para praticar conceitos fundamentais de PHP e integração com banco de dados MySQL.

## 🚀 Funcionalidades

- **Cadastrar:** Adicionar novos usuários ao banco de dados.
- **Listar:** Visualizar todos os usuários cadastrados em uma tabela.
- **Editar:** Atualizar as informações de um usuário existente.
- **Excluir:** Remover um cadastro do sistema.

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** PHP
- **Banco de Dados:** MySQL
- **Frontend:** HTML5, CSS3, Bootstrap
- **Servidor Local:** XAMPP / WAMP (ou equivalente)

## 📌 Pré-requisitos

Antes de iniciar, certifique-se de ter instalado em sua máquina:
- Servidor web local com suporte a PHP e MySQL (ex: XAMPP).
- Navegador web.

## 🗄️ Configuração do Banco de Dados

1. Abra o **phpMyAdmin** (ou seu gerenciador MySQL de preferência).
2. Crie um banco de dados chamado `crud_usuarios`.
3. Importe ou execute o script SQL abaixo para criar a tabela de usuários:

```sql
CREATE DATABASE IF NOT EXISTS crud_usuarios;
USE crud_usuarios;

CREATE TABLE IF NOT EXISTS usuarios (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL,
    data_nascimento DATE,
    criado_em TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
