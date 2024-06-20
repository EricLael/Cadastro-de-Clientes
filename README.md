<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <div class="container">
        <h1>Cadastro de Clientes</h1>
        <p>Este repositório contém um sistema simples de Cadastro de Clientes com funcionalidades de CRUD (criação, leitura, atualização e exclusão). O sistema se conecta a um banco de dados para armazenar e gerenciar os dados dos clientes.</p>
        <h2>Pré-visualização</h2>
        <img src="https://cdn.discordapp.com/attachments/1253118671291941026/1253145048925732975/Captura_de_tela_2024-06-19_213023.png?ex=6674c9c5&is=66737845&hm=a1ad640221d690e4fcd8a4c3f38b2e6adbd4959aacd721cbcb5e96373f9eddad&" alt="Formulário de Cadastro de Clientes">
        <h2>Configuração</h2>
        <p>Para que o sistema funcione corretamente, siga os passos abaixo:</p>
        <ol>
            <li>Configure seu banco de dados, usuário e senha na classe <code>Conexao</code> dentro da pasta <code>conexao</code>.</li>
            <li>Crie o banco de dados e a tabela necessária utilizando o código SQL abaixo:</li>
        </ol>
        <pre><code>CREATE DATABASE CLIENTES_DB;

USE CLIENTES_DB;

CREATE TABLE CLIENTES (
    ID INTEGER NOT NULL PRIMARY KEY AUTO_INCREMENT,
    TIPO_PESSOA CHAR(1),
    CPF_CNPJ VARCHAR(20) UNIQUE,
    NOME VARCHAR(150) NOT NULL,
    LIMITE_CREDITO NUMERIC(10, 2) NOT NULL
);</code></pre>
        <h2>Execução</h2>
        <p>Para iniciar o formulário de cadastro de clientes, execute a classe <code>ClienteFormulario</code> dentro da pasta <code>formularios</code>.</p>
        <h2>Licença</h2>
        <p>Este projeto está licenciado sob a Licença MIT.</p>
    </div>
</body>
</html>
