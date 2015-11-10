# MongoDB - Aula 01 - Exercício
autor: Jonatan H. Garcia (jhgvda)

## Importando os restaurantes

PS C:\Program Files\MongoDB\Server\3.0\bin> .\mongoimport.exe --db be-mean -c restaurantes --drop --file C:\temp\restaur
antes.json
2015-11-10T00:01:46.480-0200    connected to: localhost
2015-11-10T00:01:46.481-0200    dropping: be-mean.restaurantes
2015-11-10T00:01:47.542-0200    imported 25359 documents

## Contando os restaurantes


> show dbs
be-mean  0.078GB
local    0.078GB
> use be-mean
switched to db be-mean
> db.restaurantes.find({}).count()
25359
>
