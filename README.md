# Forked repo CSS to the Rescue @cmda-minor-web 2021 - 2022

In deze repo vind je een pure css vuurwerk show(tje). Het doen van de opdracht was om een interactieve vuurwerkshow te maken met alleen HTMl en CSS. Je kunt geen Id's en Classes gebruiken (alleen als het echt niet anders kan). Je moet gebruik maken van de CCS selectoren.

![Eindresultaat](https://github.com/norakramer1/firework-show/blob/main/img/week-4.png?raw=true)

## Week 1
De opdracht die ik gekozen heb om uit te werken is de vuurwerkshow. Ik wil 2 of 3 verschillende soorten vuurwerk laten zien met een `ul` waar de `li` van bewegen naar buiten en naar beneden vallen. Als interactie wil ik de kleur van de vuurwerkshow veranderen.

Ik ga als eerste aan de slag met keyframe animaties en custom properties om de order van de `li` aan te geven.

Mijn grootste uitdagingen liggen bij het animaties van de `li` en het positioneren van de elementen.

De eerste schets van mijn ontwerp waren bergen waar het vuurwerk uit en achter vandaan kwam. Ik heb hier de fysieke schets iets netter gemaakt in Photoshop

![eerste schets photoshop](https://github.com/norakramer1/firework-show/blob/main/img/eerste-schets-vuurwerk.png raw=true)

Na de eerste week liep ik al aardig vast. Ik ben begonnen met een pijl de lucht in te krijgen, en dat is eigenlijk het enige wat lukte. Ik had moeite met het positioneren van het vuurwerk, de `li's` in een cirkel.
![Na de eerste week](https://github.com/norakramer1/firework-show/blob/main/img/eerste-week.png?raw=true)

## Week 2
Na week 2 een stond ik er nog niet goed voor. Ik heb een tutorial gevolgd die met `::before` en `::afters` werkte. Hierdoor gingen de individuele `li's` uit elkaar. Elk `li` was apart gepositioneerd met een top en left, ik wist dat dit op een andere manier zou moeten kunnen maar hier had ik veel moeite mee.

![Na de tweede week](https://github.com/norakramer1/firework-show/blob/main/img/tweede-week.png?raw=true)

- Wat ging er soepel en wat was lastig.
Ik vond het erg lastig om de `li` te postioneren van elkaar zodat ze in een cirkel zouden staan. Ik heb uiteindelijk het advies gekregen om met `calc` te werken zodat je niet elk `li` apart hoef te berekenen. Ik heb naar een codepen van het voorbeeld van Julian gekeken om te snappen hoe `calc` in elkaar zit.

- Ik ben hier erg lang mee bezig geweest, een soepel punt is er niet echt geweest

- Welke experimenten heb je gedaan die die 'mislukt' zijn.
Ik heb geprobeerd te werken met `::before` en `::after`, dit was hieroor toch niet handig maar ik ben er wel meer over te weten gekomen en ga het zeker nog een keer gebruiken.

- Heb je nieuwe inzichten hoe je de kracht CSS kunt benutten (of juist niet).
Ik heb geleerd hoe je met `calc` en css variabelen berekeningen kan maken die meerdere malen terug moeten komen. In dit geval de `li's` positioneren op basis van elkaar zodat ze uit elkaar kunnen.

- Neem wijzigingen aan je 1e plan op.
Ik ga me in deze fase niet focussen op de bergen. Als ik er tijd voor heb wil ik nog dingen toevoegen aan de achtergrond maar het vuurwerk moet eerst af.

- Waar liggen je (nieuwe) uitdagingen voor komende week.
Ik wil kijken hoe ik het vuurwerk interactief kan maken. Ik wil er voor zorgen dat de gebruiker de kleur van het vuurwerk kan kiezen.

## Week 3
- Laat je voortgang zien ('praatje met plaatjes').
Deze week heb ik interactie in het vuurwerk gekregen doormiddel van checkboxes. Ik heb hier labels aan toegevoegd en deze gestyled als buttons. Ook heb ik het vuurwerk beter werkend gekregen, het verschijnt, wordt groter terwijl het draait en fade dan weg. 

![Week 3](https://github.com/norakramer1/firework-show/blob/main/img/week-3.png?raw=true)
![Week 3](https://github.com/norakramer1/firework-show/blob/main/img/week-3-2.png?raw=true)

- Wat ging er soepel en wat was lastig.
Wat ik moeilijk vond is het aanpassen van de berekening. Ik heb deze in de vorige week overgenomen uit een codepen, maar ik snapte er niks van, ook was het niet wat ik zocht. Ik heb de berekening uiteindelijk versimpelt door alle `li's` een custom propery met een index te geven en dan `360deg / 8` 8 is hier het aantal li's. Dit berekend de hoek van elke `li`. Daarna kun je dit custom property weer gebruiken om dat `*` de index te delen. 

- Welke experimenten heb je gedaan die die 'mislukt' zijn.
Ik ben veel aan de slag geweest met andere soorten vuurwerk. Ik ben begonnen met het de `li's ` bolletjes te maken om zo hopelijk een soort draaiend vuurwerk te krijgen maar dit is allemaal mislukt, ik heb hier besloten verder te gaan met het het langwerpige vuurwerk in verband met de tijd.

- Heb je nieuwe inzichten hoe je de kracht CSS kunt benutten (of juist niet).
Ik ben meer te weten gekomen over `calc()` en hoe je dit kan gebruiken samen met variabelen. Ook kun je hierdoor rekensommen maken om iets uit te rekenen.

- Neem wijzigingen aan je 1e plan op.
Ik wil me vanaf hier focussen op één soort vuurwerk. Ik had graag meer gewild maar ik heb er de tijd niet meer voor. Ik vind dit erg jammer want het had veel variëteit toegevoegd aan dit project.

- Waar liggen je (nieuwe) uitdagingen voor komende week.
Uitdagingen liggen bij het stylen van de pagina. Dit is op het moment erg saai. Ook moet ik mijn code opschonen en zitten er nog veel fouten in de animaties. Ze gaan af zonder dat de boxes gecheckt zijn op random momenten. Wat ik als laatste nog zou willen doen is een achtergrond schaduw toevoegen op de `li's` zodat de elementen echt licht lijken te geven.

## Week 4
- Bespreek je eindresultaat. ('praatje met plaatjes').
Dit is het eindresultaat. Je ziet een gradient achtergrond met een maan die een klein beetje beweegt. Het vuurwerk kun je aansturen met de knoppen 'Start vuurwerk' lanceert het vuurwerk in regenboog kleuren. De andere knoppen veranderen het vuurwerk van kleur. Ook hebben de `li's` een box shadow om ze een beetje op te laten lichten. Op de achtergrond zie je ook nog een aantal sterren. Deze fonkelen door ze te vergroten. Ik wilde hierbij experimenteren door bijvoorbeeld`nth-of-type(3n)` te gebruiken, ik had `nth-of-type()` nog neit gebruikt om bijvoorbeeld alle 3e elementen aan te spreken en een soort mini berekeningen te maken. Dit wilde ik wel graag nog leren, alle sterren zijn divjes die ik op random plekken gepositioneert heb met `position: absolute` en `top: en left:`.

![Week 4](https://github.com/norakramer1/firework-show/blob/main/img/week-4.png?raw=true)
![Week 4](https://github.com/norakramer1/firework-show/blob/main/img/week-4-1.png?raw=true)
![Week 4](https://github.com/norakramer1/firework-show/blob/main/img/week-4-2.png?raw=true)

- Wat ging er soepel , wat was lastig en waar ben je trots op.
Wat uiteindelijk soepel ging was het stylen van de achtergrond. Ik ben hier zonder grote problemen doorheen gekomen. 
Wat ik lastig vond was een hele hoop. Ik vind het positioneren en animeren van het vuurwerk een stuk lastiger en frustrender dan verwacht. Ik heb hier 80% van de tijd aan besteed. Waar ik ook lang mee bezig ben geweest is het zorgen dat met de knoppen de vuurwerk kleur veranderd, dit had te maken met de specifiteit van de selectoren in het regenboog vuurwerk. Ik vind het jammer dat daardoor veel andere dingen niet lukte, ik denk namelijk dat ik nog veel had kunnen toevoegen en meer had kunnen leren.
Ik ben uiteindelijk toch wel blij dat er in ieder geval *iets* gelukt is. Ik vind het geheel er wel mooi uitzien, maar ik vind het eindproduct eigenlijk te simpel en te klein.

- Welke experimenten heb je gedaan die die 'mislukt' zijn.
1. Vuurwerk maken met `::before` en  `::after`
2. Meerdere soorten vuurwerk maken
3. Werken met `svg` paths en `clip paths` voor de bergen (door de tijd)
4. Ik wilde in het begin ook iets doen met een textuur, zodat het meer zou lijken op een tekening
5. De hele `main` van kleur veranderen als elk vuurwerkje afgaat

- Heb je nieuwe inzichten hoe je de kracht CSS kunt benutten (of juist niet).
Ik heb veel geleerd over wat er allemaal mogelijk is op het gebied van CSS. Ik dacht aan het begin dat ik wel oke was met CSS maar ik kwam er snel achter dat er nog veel te leren valt. Ik heb geleerd beter na te denken over selectoren voordat je begint met id's en classes. Ook weet ik meer over het gebruik van variabelen en in welke gevallen ze echt handig zijn. Ik ben er achter gekomen dat je een deel van de interactie ook zou kunnen doen met checkboxes en radiobuttons. 


- Waar wil je meer mee gaan doen.

- `calc()`
- `css variabelen`
- Gradients animeren met houdini en `@property`, en dit ook op andere manieren gaan gebruiken
- Meer gebruik maken van `nth-of-type`, vooral door bijvoorbeeld elke 3e in een `ul` te pakken
- Dingen animeren, laten zien/ verdwijnen met checboxes en labels ipv. altijd Javascript te gebruiken voor interactie