# **Tipos de Dados**

Quando criamos as colunas das tabelas, precisamos dizer qual tipo de dados irá receber que nem acontece em algumas liguagens com as variáveis.

**Obs:** Existem muitos tipos de tipos de dados, só colocarei aqui os principais, se quiser ver mais sobre tem o site do [w3schools](https://www.w3schools.com/sql/sql_datatypes.asp) que é da onde estou utilizando como base para as informações mais precisas.

## **Tipos de String**

**Obs:** Size = quantidade/tamanho que a variável vai receber.

- CHAR(size): tamanho fixado para uma string (pode ser letras, números ou caracteres especiais), pode ir de 0 a 255.
- VARCHAR(size): tamanho de string variável (letras, números ou caracteres especiais), pode ser de 0 a 65535.
- BINARY(size): funciona igual ao CHAR
- BLOB(size): é o Binary Large Object que aguentam até 65,535 bytes, utilizado geralmente para armazenar imagens ou arquivos.
- ENUM(valor1, valor2, valor3, ...): um objeto string que pode ter apensas um valor, escolhido em uma lista de valores possíveis, com tamanho máximo de até 65535 valores.
- LONGTEXT: para string com o tamanho máximo de 4.294.967.295 bytes.

## **Tipos de Númerico**

- BOOL: zero é considerado falso e valores não zero considerado verdadeiros.
- BOOLEAN: igual ao BOOL.
- INT(size): são para números tanto negativo e positivo, com tamanho de -2147483648 até 2147483647 ou 0 até 4294967295.
- INTEGER(size): igual ao INT.
- FLOAT: são os números de pontos fluantes.
- DOUBLE(size, d): são os números de pontos fluantes normais, os números decimais depois da virgula são definidos pelo parâmetro d com o máximo de 30.
- DECIMAL(size, d): são os números de pontos fluantes exatos, os números decimais depois da virgula são definidos pelo parâmetro d com o máximo de 30.
## **Tipos de Datas**

- DATE: suporta datas com o formato 'YYYY-MM-DD'.
- DATETIME(fsp): suporta datas com o formato de 'YYYY-MM-DD hh:mm:ss' e tem o tamanho de '1000-01-01 00:00:00' até '9999-12-31 23:59:59'.
- TIMESTRAMP(fsp): são geralmente utilizados para registrar a data atual, tem o mesmo tamanho do DATETIME.
- YEAR: suporta somente ano com 4 dígitos 1901 até 2155, e 0000.