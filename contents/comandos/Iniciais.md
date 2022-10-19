# **Comandos Iniciais**

Apartir desse capítulo irei explicar mais sobre os comandos que existem dentro do SQL que seja necessário para um junior saber ou pelo menos ser um grande passo para avançar nos estudos com SQL.  

**Obs:** Em alguns momentos vou está mostrando tela do terminal e alguns do DBeaver que foi mostrando no capítulo 2.

## **CREATE**

O primeiro comando a se conhecer é o CREATE, ele é responsável por criar seu banco de dados ou uma tabela de banco com suas colunas.

```
CREATE DATABASE he4rt;
```

 ou

 ```
 CREATE TABLE 4noobs{
    lang VARCHAR(255),
    autor VARCHAR(255),
 };
```

## **ALTER**

O comando ALTER é utilizado quando precisamos fazer alguma modificação dentro do banco de dados que corresponda a adicionar uma tabela nova, modificar o datatype dela ou deletar uma coluna.

```
ALTER TABLE 4noobs
ADD data DATE;
```

ou

```
ALTER TABLE 4noobs
ALTER COLUMN data DATETIME;
```

ou

```
ALTER TABLE 4noobs
DROP COLUMN data;
```

## **DROP**

O DROP é bom vocês conhecerem para nunca testar sem querer, ele é responsável por deletar o banco de dados ou uma tabela.

```
DROP DATABASE he4rt;
```

ou

```
DROP TABLE 4noobs;
```

[Aplicativos](contents/configuracao/Aplicativos.md) | [Inicio](/README.md) |[Tipos de Dados](/contents/comandos/Tipos.md)