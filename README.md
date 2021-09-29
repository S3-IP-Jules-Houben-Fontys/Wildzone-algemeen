# algemeen

## Inleiding

In dit project wil ik een fictieve webshop gaan bouwen voor verschillende kleding artikelen. Het doel is om hiermee aan te tonen dat ik kan laten zien dat ik begrijp hoe een JavaScript front-end werkt, dat ik dit kan combineren met een OO gebaseerde back-end taal en dat de software gedistribueerd is zodat het een grote hoeveelheid aan gebruikers tevreden kan stellen. Om dit proces voor de gebruiker zo snel en efficiënt mogelijk te maken zal er gebruik worden gemaakt van asynchrone communicatie om te voorkomen dat een gebruiker lang moet wachten. In combinatie van een intuïtieve UX moet dit ervoor zorgen dat de gebruikservaring van de website zo optimaal mogelijk is. 

De data van de gebruiker zal opgeslagen worden in een relationele database. Aangezien dit gevoelige informatie is zal er gekeken moeten worden naar verschillende beveiligingsopties om de data van de gebruiker te kunnen beschermen. 


## Gedistribueerde Software

### Waarom gedistribueerde software?

Gedistribueerde software is met name belangrijk voor grote bedrijven. Deze bedrijven krijgen per seconde duizenden verzoeken. Als de software allemaal op één server zou draaien, dan zou je ongelofelijke goede hardware moeten hebben. Alle verzoeken zouden namelijk door dezelfde processor verwerkt moeten worden. Van front-end, naar de back-end, naar de database, weer terug naar de back-end om vervolgens bij de user in de front-end te kunnen eindigen. Wanneer er zoveel verzoeken zijn, is het goed voor te stellen dat de processor dit niet allemaal tegelijk kan verwerken.

Om dit probleem op te lossen moet er gebruik worden gemaakt van meerdere servers, met ieder hun eigen rekenkracht. Zo zou je een server kunnen nemen voor alle front-end verzoeken, een server voor alle back-end verzoeken en een server voor alle database verzoeken. Dit verhoogt het aantal gebruikers dat op één moment geholpen kunnen worden, zonder dat ze op elkaar moeten wachten.

Voor kleine softwareapplicaties zijn monolieten acceptabel, deze hoeven namelijk niet duizenden verzoeken per seconde te verwerken. Echter zijn monolithische applicaties niet makkelijk uit te breiden wanneer de applicatie heel populair wordt. Het hele systeem, van voor tot achter, moet namelijk op één server gerund kunnen worden. Als er dus ergens iets fout gaat in dit proces, dan werkt de applicatie niet meer.

In het geval van gedistribueerde applicaties zijn de verschillende servers onafhankelijk van elkaar. Een server kan dus kapotgaan, zonder dat de hele applicatie hierdoor niet meer werkt. Ook zijn gedistribueerde applicaties makkelijker uit te breiden. Mocht de front-end server aan zijn limiet zitten, dan kan er eenvoudig een tweede front-end server erbij genomen worden zonder dat dit een impact heeft op de applicatie.

Het is belangrijk om de verschillende onderdelen echt volledig los van elkaar te kunnen laten draaien. In alle gevallen hoeven de servers dus niet van elkaar te weten dat ze bestaan. Het enige wat ze moeten kunnen, is het ontvangen en het versturen van data in een vooraf gedefinieerde structuur.

