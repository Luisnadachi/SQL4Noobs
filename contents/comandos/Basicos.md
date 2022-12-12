# **Comandos Básicos**

Os comandos que irei explicar nesse tópico vão ser com mais foco em interagir com as tabelas e as colunas.

## **INSERT**

Esse comando tem como objetivo inserir dados em uma tabela.

``` SQL
INSERT INTO 4noobs (autor, lang)
VALUES ('nadachi', 'html')
```

ou

``` SQL
INSERT INTO 4noobs 
VALUES ('nadachi', 'html')
```

## **SELECT**

Com esse comando podemos trazer os dados de colunas especificas ou de todas colunas de uma tabela.

``` SQL
SELECT lang, autor
FROM 4noobs;
```

ou

``` SQL
SELECT * FROM 4noobs;
```

**Obs:** o * signfica trazer tudo.

## **UPDATE**

Utilizado para atualizar algum dado dentro da tabela.

``` SQL
UPDATE 4noobs
SET lang = 'php', autor = 'danielhe4rt'
WHERE lang = 'html';
```

**Obs:** Irei explicar melhor sobre o WHERE no tópico de **Condicionais** mas sempre que for rodar um UPDATE, lembre-se de utilizar ele por conta de não acabar causando o famoso erro de atualizar a tabela toda.

## **DELETE**

Utilizado para deletar alguma linha na tabela.

``` SQL
DELETE FROM 4noobs WHERE lang = 'PHP';
```

**Obs:** O que falei no Obs do UPDATE vale para o DELETE principalmente.

[Tipos de Dados](./Tipos.md) | [Inicio](../../README.md) | [Relacionamentos](./Relacionamentos.md)