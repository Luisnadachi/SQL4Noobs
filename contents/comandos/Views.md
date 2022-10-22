# **Views**

Uma coisa que eu achei bem importante que aprendi no meu antigo trabalho foi sobre Views em SQL, funcionam como uma tabela virtual com dados vindo de uma ou mais tabelas definidas por uma query, com isso podemos trazer filtrado os dados, agrupados e protegidos.  
Um detalhe a se colocar, o diferencial principal da View é que diferente das chamadas em SELECT que fazemos, as Views continuam de pé e não ocupam espaço no banco. No geral, pontos da View:

 - **Reuso**: As views são permanentes, então não precisamos chamar toda hora ela e vários usuários podem ler ao mesmo tempo.
 - **Segurança**: Podemos ocultar algumas determinadas coluna se quisermos.
- **Simplificação**: Código limpo mas ao mesmo tempo com um SELECT complexo.  

Agora vamos ver na prática como montar uma View.

Ex:

``` SQL
CREATE VIEW vw4noobs AS 
SELECT lang, alunos
FROM 4noobs 
ORDER BY lang;

SELECT * FROM vw4noobs;
```

Explicando um pouco a estrutura, primeiramente usamos o **CREATE VIEW** acompanhado do nome da view, geralmente colocamos um "vw" para indentificar, em seguida um **AS** acompanhado do nosso select com as nossas condicionais. A outra linha de **SELECT** que utilizei em seguida é so para vocês visualizarem os resultados da View.

[Joins](contents/comandos/Joins.md) | [Inicio](/README.md) 