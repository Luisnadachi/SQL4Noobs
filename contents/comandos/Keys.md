# **Primary Key e Foreign Key**

Nesse tópico iremos apresentar sobre as chaves primárias e as chaves estrangeiras dentro do SQL, antes disso, aconselho a procurar um pouco sobre "relacionamentos em banco de dados" que pode ser um assunto que vai auxiliar a entender mais para o que server as Keys no SQL. 

## **Primary Key**

Só pode haver uma chave primária (Primary Key) em uma tabela, porque o intuito dela é nunca receber vazio (NULL) e ser auto incrementada (1,2,3,4,..) para ser utilizada como identificador de uma linha da tabela, como se fosse um código ou um ID.

Ex:

``` SQL
CREATE TABLE 4noobs(
ID int NOT NULL AUTO_INCREMENT,
lang varchar (255),
autor varchar (255),
PRIMARY KEY (ID)
);
```

## **Foreign Key**

O intuito da chave estrangeira (Foreign Key) é servir de referencia para uma chave primária de outra tabela, se você entender um pouco sobre POO (programação orientada a objeto) pode ver isso como igual funciona relação de pai para filho.

Ex:

``` SQL
CREATE TABLE Languages (
    langID int NOT NULL AUTO_INCREMENT,
    name varchar(255) NOT NULL,
    PRIMARY KEY (langID)
);

CREATE TABLE 4noobs(
    conteudoID int NOT NULL AUTO_INCREMENT,
    autor varchar(255),
    PRIMARY KEY (conteudoID),
    FOREIGN KEY (langID) REFERENCES Languages(langID)
);
```

[Condicionais](contents/comandos/Condicionais.md) | [Inicio](/README.md) | [Joins](contents/comandos/Joins.md)