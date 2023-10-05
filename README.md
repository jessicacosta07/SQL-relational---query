# SQL Relational Query

## Bootcamp WEX - Desenvolvimento .NET e QA

## Skills
![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white)

 <code>
 SELECT 
	Nome, 
	Ano 
FROM Filmes
 </code>

![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/0b65a8c4-9d7f-403b-9c77-f31f435747c4)


 <code>
SELECT Nome, 
       Ano, 
       Duracao 
FROM Filmes 
ORDER BY Ano
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/fccd5e93-ca85-4ad2-9e1c-62ce51072af3)
 

 <code>
SELECT Nome,
       Ano, 
       Duracao
FROM Filmes
WHERE Nome = 'De Volta para o Futuro'
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/283f1f9c-abad-4ae2-be24-f92ffb7f3952)

 
 <code>
SELECT Nome,
       Ano, 
       Duracao
FROM Filmes
WHERE Ano = 1997
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/9a061723-a21c-4f48-894b-60056bcecf33)


 <code>
SELECT Nome,
       Ano, 
       Duracao
FROM Filmes
WHERE Ano > 2000
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/73ecbb1b-132f-413c-81ab-02fe45a7c7a6)


 <code>
SELECT Nome,
       Ano, 
       Duracao
FROM Filmes
WHERE Duracao > 100 AND Duracao < 150
ORDER BY Duracao
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/f12c11f9-f4e2-48ab-b630-52607a10194f)


 <code>
SELECT Ano, COUNT (*) Quantidade 
FROM Filmes
GROUP BY Ano
ORDER BY Quantidade DESC
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/3aff8063-0ee1-4beb-a114-80a05168aeda)


  <code>
SELECT * FROM Atores
WHERE Genero = 'M'
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/0ead1300-9b3b-4608-a17c-a3a94d06985f)


   <code>
SELECT * FROM Atores
WHERE Genero = 'F'
ORDER BY PrimeiroNome
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/1c5f8f3e-e236-4be5-a818-b4bfc138d75a)


   <code>
SELECT
    F.Nome,
    G.Genero
FROM
    Filmes F
INNER JOIN
  Generos G
INNER JOIN
  FilmesGenero FG
ON G.Id = FG.IdGenero
ON F.Id = FG.IdFilme
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/d99503ee-0cf5-4024-8d8b-021f3036ec69)


   <code>
SELECT
    F.Nome,
    G.Genero
FROM
    Filmes F
INNER JOIN
  Generos G
INNER JOIN
  FilmesGenero FG
ON G.Id = FG.IdGenero
ON F.Id = FG.IdFilme
WHERE Genero = 'Mistério'
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/6c584b49-8527-45e7-99dc-5984dbd8080f)

  <code>
SELECT
    F.Nome,
    A.PrimeiroNome,
    A.UltimoNome,
    EG.Papel
FROM
   Filmes F
INNER JOIN
  Atores A
INNER JOIN
  ElencoFilme EG
ON A.Id = EG.IdFilme
ON F.Id = EG.IdAtor
 </code>

 ![image](https://github.com/jessicacosta07/SQL-relational-query/assets/65916297/2c493c1a-2d74-4411-ab8c-4876186dc761)


 

 



 

 


 


 

 


