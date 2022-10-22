## **Joins**

Os "Joins" tem o intuito de combinarmos durante o SELECT duas ou mais tabelas para realizar uma exibição, e temos vários tipos de "Joins" só que dentro deles temos também outros tipos só que bem mais complexos, então irei explicar os iniciais e caso você deseje se aprofundar mais, saiba que para o que você deseja fazer possivelmente existe um "Join" para isso.

- (INNER) Join
- LEFT (OUTER) JOIN
- RIGHT (OUTER) JOIN
- FULL (OUTER) JOIN

**Obs:** INNER são dados em comum entre a tabela e OUTER são os dados que não são em comum. 

**Obs2:** Caso você queira treinar na prática, rode esses comandos para ter duas tabelas para testar.

``` SQL

CREATE TABLE 4noobs (
id4noobs INT NOT NULL AUTO_INCREMENT,
lang VARCHAR(255),
alunos VARCHAR(255),
PRIMARY KEY (id4noobs)
);

create table cursos (
idcurso INT NOT NULL AUTO_INCREMENT,
lang VARCHAR(255),
alunos VARCHAR(255),
PRIMARY KEY (idcurso)
);

INSERT INTO 4noobs (lang, alunos)
VALUES ('php', 'daniel');
INSERT INTO 4noobs (lang, alunos)
VALUES ('sql', 'nadachi');
INSERT INTO 4noobs (lang, alunos)
VALUES ('UI', 'neex');
INSERT INTO 4noobs (lang, alunos)
VALUES ('UX', '7k');
INSERT INTO cursos (lang, alunos)
VALUES ('php', 'daniel');
INSERT INTO cursos (lang, alunos)
VALUES ('UI', 'neex');
INSERT INTO cursos (lang, alunos)
VALUES ('testes', 'joaozinho');
INSERT INTO cursos (lang, alunos)
VALUES ('java', 'joaozinho2');

```

## **INNER JOIN**

Como explicado no obs acima, vai nos trazer os dados em comum entre as tabelas.

``` SQL
SELECT * 
FROM 4noobs
INNER JOIN cursos ON 4noobs.lang = cursos.lang;
```

## **LEFT JOIN**

Vai retornar todos os dados da primeira tabela chamada junto com os dados que são em comum com a segunda tabela chamada.

``` SQL
SELECT *
FROM 4noobs
LEFT JOIN cursos 
ON 4noobs.lang = cursos.lang;
```

## **RIGHT JOIN**

Vai retornar todos os dados da segunda tabela chamada junto com os dados que são em comum com os dados da primeira tabela chamada.

``` SQL
SELECT *
FROM 4noobs
RIGHT JOIN cursos 
ON 4noobs.lang = cursos.lang;
```

## **FULL OUTER JOIN**

Retorna todos os dados que são iguais entre as duas tabelas.

``` SQL
SELECT 4noobs.lang, cursos.idcurso 
FROM 4noobs
FULL OUTER JOIN cursos 
ON 4noobs.id4noobs = cursos.idcurso
ORDER BY 4noobs.id4noobs;
```

Obs: Full outer join não funciona no MySQL.

[Primary Key e Foreign Key](contents/comandos/Keys.md) | [Inicio](/README.md) | [Views](contents/comandos/Views.md)