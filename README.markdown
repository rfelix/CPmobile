CP Mobile
=========
por Carlos Fonseca - carlosefonseca at gmail


Actualmente em [http://carlosefonseca.com/cp](http://carlosefonseca.com/cp)

Webservice:

*   getdata.php
*   estacoes.[txt,js,php]


O resto é tudo relacionado com a mobile webapp



Breve explicação do Webservice:
-------------------------------

Este "webservice" está em [http://carlosefonseca.com/cp/getdata.php](http://carlosefonseca.com/cp/getdata.php) e recebe os seguintes seguintes argumentos por GET:

* **departure** > estação de partida
* **arrival** > estação de chegada
* **day** > dia no formato YYYY-MM-DD
* **hour** > hora (entre 0 e 23; opcional)

Por exemplo:

[http://carlosefonseca.com/cp/getdata.php?departure=Sacavem&arrival=Monte Abraao&day=2010-08-23&hour=20](http://carlosefonseca.com/cp/getdata.php?departure=Sacavem&arrival=Monte%20Abraao&day=2010-08-23&hour=20)

resulta em JSON que representa um array de comboios em que cada comboio é um array composto pelos campos:

* **i** > numero do resultado
* **t** > tipo do comboio (U - Urbano; IC - Inter-Cidades…)
* **d** > hora de partida
* **a** > hora de chegada
* **l** > duração da viagem


Não nos foi possível obter mais informações do site. Este realiza um pedido para obter detalhes de cada comboio e nunca conseguimos reproduzir esse pedido fielmente, sendo sempre devolvidas mensagens de erro.
