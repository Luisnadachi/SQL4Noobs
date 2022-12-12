# **Sub Conjuntos**

Dentro da linguagem de SQL os comandos eles podem ser dividos em sub conjuntos para categorizar os mesmos, cada um focando em um tipo de instrução.

![Imagem dos Sub Conjutos de SQL](/assets/SubConjuntos.png)

> Imagem ilustrativa sobre os sub conjuntos.

Esses grupos como na imagem acima são dividos em:

- DQL
- DML
- DDL
- DCL
- DTL

A seguir vamos explicar um pouco deles.

## **DDL**

Pelo seu nome completo de **Data Definition Language**, são os comandos que utilizamos para interagir com o banco em si, desde criar até excluir uma tabela específica. Esses comandos são

- CREATE
- ALTER
- DROP
- TRUNCATE
- COMMENT
- RENAME

## **DQL**

Pelo seu nome completo de **Data Query Language**, é o subconjunto responsável pelo comando de consulta nas tabelas do banco, que seria ele:

- SELECT

## **DML**

Pelo seu nome completo de **Data Manipulation Language**, é o subconjunto responsável pelos comandos que manipulam os dados nas tabelas, são eles:

- INSERT
- UPDATE
- DELETE

## **DCL**

Pelo seu nome completo de **Data Control Language**, é o subconjunto responsável pelos comandos que envolvem a segurança do banco de dados, são eles:

- GRANT
- REVOKE

## **DTL**

Pelo seu nome completo de **Data Transaction Language**, é o subconjunto responsável pelos comandos que gerenciam e controlam transações de dados.

- BEGIN/SET TRANSACTION
- COMMIT
- ROLLBACK
- SAVEPOINT

Por agora não expliquei sobre os comandos porque eles vão ser trazidos no Capitulo 3 onde irei falar expecificamente sobre eles.

[Sintaxe](./Sintaxe.md) | [Inicio](../../README.md) | [Instalando SQL (MYSQL)](../configuracao/Instalacao.md)