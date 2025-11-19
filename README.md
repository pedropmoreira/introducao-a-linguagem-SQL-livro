# LIVRO : INTRODUÇÃO AO SQL 
Repositório destinado ao livro Introdução à Linguagem SQL: Abordagem prática para iniciantes
## OS BANCOS USADOS SERÃO OS DO LIVRO
## CAPITULO 4 : 
Pasta CAP4. 

Foi um capitulo que focou em consultas básicas SQL, Calculos em consultas, e Alias.  
```
-- Conhecendo as tabelas 
SELECT * FROM CUSTOMER;
SELECT * FROM CUSTOMER_ORDER;
SELECT * FROM PRODUCT;

-- OPERAÇÕES + ALIAS

SELECT PRODUCT_ID, PRICE, PRICE * 1.07 AS TAXED_PRICE FROM PRODUCT;

-- USANDO ROUND PRA ARREDONDAR.

SELECT PRODUCT_ID, PRICE, ROUND(PRICE * 1.07,2) AS TAXED_PRICE FROM PRODUCT;

-- CONCATENANDO

SELECT name, city || state AS LOCATION from customer;
```

## CAPITULO 5:

Neste capítulo aprendemos a trabalhar com filtros em SQL usando a cláusula WHERE.  
Os principais conceitos apresentados foram:
- Uso básico do WHERE para filtrar linhas.
- Comparações com =, !=, <>.
- Filtros por intervalo usando BETWEEN.
- Uso de OR, IN e NOT IN.
- Expressões matemáticas dentro do WHERE (ex.: % para módulo).
- Comparações com texto e uso de LENGTH.
- Busca por padrões usando LIKE, % e _.
- Como trabalhar com valores booleanos no SQLite (1 e 0).
- Como tratar valores NULL com IS NULL e coalesce().
- Como combinar condições usando parênteses.  

O script completo com todos os exemplos está dentro da pasta CAP5 (nome: capitulo_5).