# **Sintaxe**

A sintaxe de SQL é bem simples, por padrão colocamos os comandos em Caps Lock (letra maiuscula) e os dados em minusculo, geralmente seguindo assim:

```
COMANDO dados COMANDO dados;
```

Um exemplo na prática temos um comando que vamos aprender lá na frente que seria:

```
SELECT * FROM Clientes;
```

Aqui temos o comando SELECT utilizando todos os dados que é representado por *, em seguida o comando FROM para finalizar com a tabela chamada Clientes.

Um detalhe para se atentar também na sintaxe do SQL, lembrando que próximos tópicos veremos diferentes comandos então não se importe se não entender isso agora mas lembre-se de voltar aqui no final para entender novamente, mas existe uma ordem para se escrever os comandos por conta da ordem de exececução do SQL:

**Ordem de Escrita SQL**

- SELECT
- FROM
- WHERE
- GROUP BY
- HAVING
- ORDER BY

**Ordem de Execução SQL**

- FROM
- WHERE
- GROUP BY
- HAVING
- SELECT
- ORDER BY

[Diferença entre BDs relacionais e não relacionais](contents/Introducao/Diferenca.md) | [Inicio](/README.md) | [Sub Conjuntos](contents/Introducao/Conjuntos.md)