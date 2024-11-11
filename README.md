# Passo a Passo: Criação de um Banco de Dados 
Tutorial de como criar um Bnaco de Dados Sql que organiza
as Informações de 'livros', 'editora', 'autores' e 'assuntos'.
Este guia será dividido em etapas para demonstra desde a 
criação de tabelas, chaves e até manipulação/consulta de dados.

## Resumo de uma Estrutura SQL
*__CREATE__: Para criar 'Banco de Dados' ou 'Tabelas'
*__ALTER__: Para adicionar ou modificar colunas 
*__DROP__: Para remover 'Banco de Dados' ou 'Tabelas'
*__INSERT__: Para adicionar registros na Tabelas
*__UPDATE__: Para atualizar os Registros
*__DELETE__: Para Remover os Registros
*__SELECT__: Para Consultar e Visualizar Dados

## Passo 1:Criação do Banco de Dados e das Tabelas 
#### 1.1 Criando o DB 
```
CREATE DATABASE bibloteca;
USE bibloteca; 
```

#### 1.2 Criando a Tabela 'Editora'
```
CREATE TABLE editora (
    id_editora INT PRIMARY KEY AUTO_INCREMENT,
    nome_editora VARCHAR(100) NOT NUL,
    pais VARCHAR(50)
);
```
#### 1.3 Criando a Tabela 'Autor'
```
CREATE TABLE autor(
    id_autor INT PRIMARY KEY AUTO_INCREMENT,
    nome_autor VARCHAR(200),
    data_nascimento DATE
);
```
#### 1.4 Criando a TAbela 'Assuntos'
```
CREATE TABLE assunto(
    id_assunto INT PRIMARY KEY AUTO_INCREMENT,
    descrição_assunto VARCHAR(300) NOT NULL
);
```


