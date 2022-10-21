# **Condicionais**

Até mesmo em SQL podemos utilizar condições em determinados comandos, podemos ver isso no tópico anterior de comandos básicos quando utilizamos SELECT, UPDATE e o DELETE.

## **WHERE**

O WHERE já conhecemos do capítulo anterior, traduzido significa "ONDE", com ele especicamos uma condição expecifica.

```
SELECT * FROM 4noobs 
WHERE lang = 'PHP';
```

Nesse exemplo selecionamos todas as linhas na tabela do 4noobs que contém a coluna lang igual a PHP.

## **IN**

O operador IN serve para conseguimos especificar vários valores dentro da condição do WHERE.

```
SELECT * FROM 4noobs
WHERE lang IN ('PHP','JS');
```

E temos também forma negativa.

```
SELECT * FROM 4noobs
WHERE lang NOT IN ('PHP','JS');
```

## **AND, OR e NOT**

Para citar alguns exemplos e reforçar, podemos utilizar operadores como "E", "OU" e "NÃO", eles são usados para complementar condições como o WHERE, alguns exemplos.

```
SELECT lang, autor
FROM 4noobs
WHERE lang = 'php' AND autor = 'danielhe4rt';
```

ou

```
SELECT lang
FROM 4noobs
WHERE lang = 'php' OR lang = 'html';
```

ou

```
SELECT lang
FROM 4noobs
WHERE NOT lang = 'php';
```

## **ORDER BY**

O operador ORDER BY server para quando usarmos o SELECT trazer os dados tanto em ordem crescente ou descrecente, por padrão o ORDER BY tras em ordem crescente mas podemos especificar usando ASC (crescente) e DESC (descrescente).

```
SELECT * FROM 4noobs
ORDER BY lang;
```

ou

```
SELECT * FROM 4noobs
ORDER BY lang ASC;
```

ou

```
SELECT * FROM 4noobs
ORDER BY lang DESC
```

**Obs:** Existem outros comandos para condições só que esses aqui citados são os mais utilizados principalmente para você que está começando ou juninho.

