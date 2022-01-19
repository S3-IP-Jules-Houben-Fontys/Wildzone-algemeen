# algemeen

Dit is de verzamel repository van alle microservices in het Wildzone webshop & adminpanel project. Deze repository is alleen bedoeld om de werking van alle microservices uit te proberen, aangezien er hier geen daadwerkelijke code gevonden kan worden. Onder het kopje <a href="#services">Ports & services</a> kan de bijbehorende code gevonden worden door middel van de links.

## Getting started

Om het project op te starten, moet eerst de code gekloond moeten worden naar de eigen pc. 

<ol>
    <li>Dupliceer de sample.env file en hernoem deze naar `.env` </li>
    <li>Vul de waardes in die nog leeg zijn in de env file. Poorten hoeven niet meer benoemd te worden om het opstart proces eenvoudiger te maken zijn deze al ingevuld.</li>
    <li>In de rootfolder van het project moet de volgende command worden uitgevoerd via de opdrachtprompt: <br>

`docker-compose up`

</li>
    <li>Alle services zullen nu opstarten, dit duurt maximaal 5 minuten om volledig opgestart te zijn. Voor die tijd is er kans dat een microservice herstart omdat de database nog niet klaar was met opstarten.</li>
    <li>De microservices kunnen nu allemaal bereikt worden met een unieke link, voor het hele overzicht van deze links zie het kopje <a href="#services">Ports & services</a>.</li>
</ol>

<h2 id="overzicht">Overzicht van project</h2>

![Wildzone-C2 Container diagram drawio (4)](https://user-images.githubusercontent.com/73841047/150106747-7fdbd1af-3710-41b0-9f90-4b4b4f7c9e46.png)

<h2 id="services"> Ports & services </h2>

| Container                     | Address            | Port | Type     | Language/Framework    | In-use             |
|-------------------------------|--------------------|------|----------|-----------------------|--------------------|
| <a href="https://github.com/S3-IP-Jules-Houben-Fontys/Wildzone-front-end-adminpanel">Wildzone-front-end-adminpanel</a> | localhost:3000     | 3000 | Webapp   | ReactJS               | :white_check_mark: |
| Wildzone-front-end-Webshop    | localhost:3001     | 3001 | Webapp   | ReactJS               | :x:                |
| <a href="https://github.com/S3-IP-Jules-Houben-Fontys/Wildzone-api-suppliers">Wildzone-api-suppliers</a>        | localhost:3002/api | 3002 | API      | ExpressJS & Sequelize | :white_check_mark: |
| <a href="https://github.com/S3-IP-Jules-Houben-Fontys/Wildzone-api-products">Wildzone-api-products</a>         | localhost:3003/api | 3003 | API      | Spring Boot           | :white_check_mark: |
| Wildzone-api-inventory        | localhost:3004/api | 3004 | API      | ExpressJS & Sequelize | :x:                |
| <a href="https://github.com/S3-IP-Jules-Houben-Fontys/Wildzone-api-basket">Wildzone-api-baskets</a>          | localhost:3005/api | 3005 | API      | ExpressJS & Sequelize | :x:                |
| Wildzone-api-categories       | localhost:3006/api | 3006 | API      | ExpressJS & Sequelize | :x:                |
| Wildzone-database-suppliers   | localhost:3306     | 3306 | Database | MySQL                 | :white_check_mark: |
| Wildzone-database-products    | localhost:3307     | 27017| Database | MongoDB               | :white_check_mark: |
| Wildzone-database-inventory   | localhost:3308     | 3308 | Database | MySQL                 | :x:                |
| Wildzone-database-baskets     | localhost:3309     | 3309 | Database | MySQL                 | :white_check_mark: |
| Wildzone-database-categories  | localhost:3310     | 3310 | Database | MySQL                 | :x:                |

