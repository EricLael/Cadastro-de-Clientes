<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <div class="container">
        <h1>Cadastro de Clientes</h1>
        <p>Este projeto contém um sistema simples de Cadastro de Clientes com funcionalidades de CRUD (criação, leitura, atualização e exclusão). O sistema utiliza o MySQL Workbench para modelagem do banco de dados e se conecta a um banco de dados MySQL para armazenar e gerenciar os dados dos clientes.</p>
        <h2>Configuração</h2>
        <p>Para que o sistema funcione corretamente, siga os passos abaixo:</p>
        <ol>
            <li>Este projeto utiliza o IntelliJ IDEA como ambiente de desenvolvimento integrado (IDE). Certifique-se de que o IntelliJ IDEA esteja instalado em sua máquina.</li>
            <li>O projeto também utiliza o Maven como ferramenta de automação de build. Verifique se o Maven está configurado corretamente no IntelliJ IDEA.</li>
            <li>Utilize o MySQL Workbench para configurar seu banco de dados. Configure o banco de dados, usuário e senha na classe <code>Conexao</code> dentro da pasta <code>conexao</code>.</li>
            <li>Crie o banco de dados e a tabela necessária utilizando o código SQL abaixo no MySQL Workbench:</li>
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
        <p>Para iniciar o formulário de cadastro de clientes, abra o projeto no IntelliJ IDEA e execute a classe <code>ClienteFormulario</code> dentro da pasta <code>formularios</code>.</p>
        <h2>Licença</h2>
        <p>Este projeto está licenciado sob a Licença MIT.</p>
    </div>
</body>
</html
