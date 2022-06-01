# **Project Plan**

### _ **Foodies** _

### _Info Support_

| **Datum : 15/2** |
| --- |
| **Versie : 2** |
| **Status : Afgerond** |
| **Auteur : Zie versie historie** |

**Versie historie**

| **Versie** | **Datum** | **Auteur(s)** | **Veranderingen** | **Status** |
| --- | --- | --- | --- | --- |
| v1 | 15-02-2022 | Justin van de Laar, Julian Janssen, Thisoban Mahalingam, Francois Haan, Bas Onrust, David Hellinga | Project plan opgezet en uitgewerkt. | afgerond |
| v2 | 21-02-2022 | Zie bovenstaand | PBS toegevoegd, c4 model gemaakt, formatting bijgewerkt, risico&#39;s toegevoegd, basis pipelines opgezet | afgerond |
| v3 | 07-03-2022 | Zie bovenstaand | PBS aangepast, |
| v4 | 29-03-2022 | Zie bovenstaand | Redenen voor technische keuzes |
| V5 | 30-05-2022 | Francois Haan | Commentaar toegevoegd | afgerond |



**// binnen dit project hebben we natuurlijk alles samen besproken en elkaar geholpen met teksten bedenken etc ik zal meer zetten bij dingen waar ik specifiek aan mee heb gewerkt.**

Contents

[Project opdracht](#_heading=h.3dy6vkm) **4**

[Context](#_heading=h.1t3h5sf) 4

[Doel van het project](#_heading=h.4d34og8) 4

[Scope and preconditities](#_heading=h.2s8eyo1) 4

[Strategie](#_heading=h.17dp8vu) 4

[Onderzoeksvragen en methodologie](#_heading=h.3rdcrjn) 5

[Eind producten](#_heading=h.26in1rg) 6

[Architectuur](#_heading=h.wijzfr64mhbf) 7

[Technische keuzes](#_heading=h.1cl4tlkk2rkb) 8

[Restaurant App](#_heading=h.wcy1zo8ydpl9) 8

[Admin App](#_heading=h.7gerjqjj5a6g) 8

[Project organisatie](#_heading=h.lnxbz9) **9**

[Stakeholders en teamgenoten](#_heading=h.35nkun2) 9

[Communicatie](#_heading=h.1ksv4uv) 9

[Activiteiten en planning](#_heading=h.44sinio) **10**

[Fases van het project](#_heading=h.2jxsxqh) 10

[Planning en doelstellingen](#_heading=h.z337ya) 10

[Strategisch testen en configurerend management](#_heading=h.1y810tw) **11**

[Strategisch Testen](#_heading=h.2xcytpi) 11

[Test omgeving en vereiste bronnen](#_heading=h.3whwml4) 11

[Configuratie management](#_heading=h.2bn6wsx) 11

[Financien en risico&#39;s](#_heading=h.qsh70q) **12**

[Risico en Mitigatie](#_heading=h.49x2ik5) 12

# 1.Project opdracht

## 1.1Context

Info Support is een consultancy bedrijf dat ook software pakketten oplevert aan andere bedrijven. Info Support heeft ons gevraagd om een applicatie te maken voor restaurantketens. Het moet een applicatie worden voor een restaurant via een bestelsysteem. Een klant moet kunnen bestellen via een tablet. De kok krijgt via een scherm door wat een klant van welke tafel aan eten heeft besteld. Het barpersoneel krijgt de bestellingen voor de drankjes door via de bestelapplicatie. Zij kunnen aangeven op een scherm waarmee het personeel bezig mee is.Tot slot is er een scherm voor de beheerder om aanpassingen op te doen bijvoorbeeld het menu van wat klanten kunnen bestellen.

## 1.2Doel van het project

Het doel van dit project is om een bestelling systeem te maken voor Info Support. De reden dat ze dit nodig hebben is omdat ze in de nabije toekomst een restaurant willen beginnen, waarvoor ze dit bestelling systeem willen toepassen. De gewenste situatie is dat we op het eind van het semester een volledig werkend bestelling systeem hebben.

De voordelen van dit project zijn dat het systeem voor beide de medewerkers en de klanten van het restaurant veel duidelijkheid breng. Het is namelijk een overzichtelijke manier om te bestellen voor klanten. Medewerkers weten wat zij naar de klanten moeten brengen qua gerechten en dranken.

De mogelijkheden die dit project oplevert is een websocket systeem dat aan de keuken en de bar aangeeft wat de klanten bestellen zonder dat ze hiervoor hoeven te herladen. Aangezien de applicatie op real-time werkt zal het voor de betrokkenen altijd duidelijk zijn wat zij kunnen verwachten of moeten uitvoeren.

## 1.3Scope and preconditities

| **Inside scope:** | **Outside scope:** |
| --- | --- |
| Digitaal Menu en Bestelsysteem | Betalingssysteem implementeren |
| Work Tracking Systeem | Hosting |
| Admin Dashboard |
| Centrale backend |
| Data storage |
| Bestaande betalingssystemen koppelen |

## 1.4Strategie

Wij hebben besloten om om de SCRUM methodiek te gebruiken. Alle methoden behalve Scrum hebben issues waardoor ze niet voor dit project geschikt zijn. Hieronder zal worden toegelicht waarom andere agile methodes niet geschikt zijn voor ons project.

Kanban en Lean werken niet in sprints maar met continue verbetering waarbij op elk moment het belangrijkste iets wordt opgepakt - vanuit Fontys wordt verwacht dat wij in sprints van drie weken werken, dus is dit voor ons geen optie. XP vereist dat de klant deel is van het ontwikkelteam en op elk moment aanspreekbaar is - dit is bij zulke opdrachten voor Fontys niet mogelijk of gewenst. Crystal is gericht op grootschalige teams en niet buitengewoon geschikt voor een enkel klein team van zes man.&quot;

Bron: &#39;Agile Onderzoek&#39; hoofdstuk &#39;Welke Agile methode is geschikt voor het project?&#39; op pagina 20.

![Scrum](https://user-images.githubusercontent.com/71487939/171167406-58c4cd1a-5ed1-4272-907a-40ab3574cda9.png)

# 1

## 1.5Onderzoeksvragen en methodologie

Not decided yet.

## 1.6Eind producten 

![PBS-versie2 drawio (1)](https://user-images.githubusercontent.com/71487939/171140824-463f10b9-5ea1-4ecf-8dde-690dd31007da.png)

/ **/ binnen het pbs heb ik meegedacht met de verschillende delen van de website die we nodig zouden gaan hebben en gekeken hoe we dit moesten noteren**

Hierboven ziet u het Product Breakdown Structure. Het PBS werkt als volgt:

Je begint bovenaan hier heb je het eindproduct. In ons geval is het ordersysteem voor het restaurant. Bij het eindresultaat komen een aantal producten kijken. Dit hebben we onderverdeeld na feedback van onze docent in de volgende twee categorieën. Deze categorieën zijn gekleurt in het blauw in de bovenstaande afbeelding.

Onder deze subcategorieën komen een aantal producten die we aan het eind opleveren. De verschillende soorten subproducten staan in de rode vakken.Voor documentatie kan je denken aan de volgende soort producten:

1. Het project plan
2. Het database ontwerp
3. Het C4 model

Voor het kopje software is hetzelfde van toepassing als bij documentatie. Aan de volgende producten zou je kunnen denken:

1. FrontEnd voor de Admins
2. FrontEnd voor het Restaurant
3. BackEnd voor de Admins
4. BackEnd voor het Restaurant

## 1.7Architectuur

![v2 - Architectuur](https://user-images.githubusercontent.com/71487939/171140605-e438f971-022c-411d-8eff-b339711a0355.png)

## 1.8Technische keuzes

Voor software projecten moeten aan het begin - en in de loop van het project - keuzes worden gemaakt over welke technologieën en talen gebruikt worden. In dit hoofdstuk zullen we de tot nu toe gemaakte keuzes uitleggen.

    1.
### Restaurant App

De restaurant app is het eerste deel van het project waar de meeste &quot;core&quot; functionaliteit in zal zitten. Hierdoor hebben we gekozen voor technologieën waar we al een basis kennis van hebben zodat we een goede basis kunnen leggen.

1. **.NET Core 6**

C# / .NET Core was de backend taal waar de meeste van ons bekend mee waren. Daarnaast wilden we gebruik maken van oa. EF Core en Identity.

1. **Vue.js + Typescript**

Vue was het frontend framework waar de meeste van ons bekend mee waren. Typescript is gekozen om strong typing te hebben - iets dat basis javascript niet ondersteunt. Dit maakt de code leesbaarder en minder foutgevoelig.

1. **SQLite voor ontwikkeling**

Sqlite is een lightweight database die geen eigen server nodig heeft. Het draait op een bestand dat in het project zelf kan worden aangemaakt. Voor productie is het niet geschikt - de functionaliteit en performance en veiligheid zijn niet optimaal daarvoor - maar voor de vroege stadia van ontwikkelen biedt het alle nodige functies. In de loop van het project zal het dus ook vervangen moeten worden met een andere technologie.

1. **PostgreSQL als vervanger van SQLite**

Bij het kiezen van een database oplossing moeten een paar vragen beantwoord worden. De eerste is of een SQL, NoSQL of ander type database het meest geschikt is. Hierbij hebben we gekozen voor SQL omdat het de eerdere keuzes het beste ondersteunt. We willen in onze .NET applicatie gebruik maken van EF Core - het ORM van .NET Core - om met de database te werken (zie hierboven waarom). Dit vereist het gebruik van een SQL database waarmee onze keuze daarover vaststaat. De volgende vraag is welke SQL database we gebruiken. Gezien dit een studieproject is zijn alleen oplossingen met een redelijke market share relevant: Oracle, MySQL, SQL Server en PostgreSQL. Oracle valt af omdat het erg gericht is op grootschalige enterprise projecten. SQL Server is ook erg gelimiteerd voor gratis gebruik en vereist bij opschalen al snel een prijzige licentie. Dit geeft dus twee opties: MySQL of PostgreSQL. Beide bieden de nodige functionaliteit, zijn voor onze doeleinden volledig gratis bruikbaar en zouden dus een acceptabele keuze zijn. We hebben hierbij gekozen om voor PostgreSQL te gaan omdat die open source is.

    1.
### Admin App

De admin app wordt een losstaande en redelijk minimale applicatie met focus op functionaliteit. Dit geeft ons de kans om technologieën te kiezen waar we minder bekend mee zijn zodat we daar ervaring mee op kunnen doen.

**Java + Spring**

Java is naast C# een van de meest wijd verspreide backend talen voor web API&#39;s en Spring is een van de meest gebruikte Java frameworks. Daarom hebben we gekozen om voor de admin app deze combinatie te proberen.

**Angular**

Naast Vue.js zijn er twee andere grote javascript frameworks: React en Angular. We hebben voor Angular gekozen omdat die het meeste lijkt op backend talen zoals C# en Java en we willen testen hoe dat bevalt als frontend framework.

# 2.Project organisatie

## 2.1Stakeholders en teamgenoten

| **Naam** | **Afkorting** | **Rol en functies** | **Beschikbaarheid** |
| --- | --- | --- | --- |
| Thisoban Mahalingam | _Thiso_ | _Developer_ | _Maandag en dinsdag 09:00 tot 16:00_ |
| Justin van de Laar | _Justin_ | _Developer_ | _Maandag en dinsdag 09:00 tot 16:00_ |
| Julian Janssen | _Julian_ | _Developer_ | _Maandag en dinsdag 09:00 tot 16:00_ |
| Francois Haan | _Francois_ | _Developer_ | _Maandag en dinsdag 09:00 tot 16:00_ |
| Bas Onrust | _Bas_ | _Developer_ | _Maandag en dinsdag 09:00 tot 16:00_ |
| David Hellinga | _David_ | _Contactpersoon_
 | _Maandag en dinsdag 09:00 tot 16:00_ |
| Samuil Angelov | _Samuil_ | _Project begeleider_ | _Maandag 09:00 - 12:00 en 13:00 - 16:00
 Woensdag 09:00 - 12:00_ |
| Leon Bokhorst | _Leon_ | _Individueel begeleider_ | _Woensdag 09:00 - 12:00__Donderdag 09:00 - 12:00 en 13:00 - 16:00_ |
| Jeroen Uittenbosch | _Jeroen_ | _Product owner_ |
| Sander Klijsen | _Sander_ | _Product owner_ |

## 2.2Communicatie

Communicatie gaat via een persoon in de groep. DIt is om de communicatie soepel te laten verlopen via een lijn. Hiermee willen we voorkomen dat iedereen de product owner mailt. Dit voorkomt ook dat er verwarring ontstaat over het project omdat, persoon A iets anders heeft gekregen dan persoon C aan informatie van de product owner.

David Hellinga is de contactpersoon van de groep. Tijdens de kennismaking met Info Support hebben we besloten contact te houden via de mail. We hebben afgesproken met Info Support dat we de mogelijkheid krijgen om feedback te vragen via de mail over bepaalde producten.

Sprints worden gedaan om de 3 weken. Na iedere 3 weken worden een sprint opgeleverd aan de product owner. De oplevering vindt plaats op school of als het is afgesproken bij de product owner op kantoor.

Als we over het team spreken dan spreken we over de groep Foodies

Verder communiceert het team via microsoft teams. Mocht het voorkomen dat op de dag dat we naar school gaan dat een teamlid te laat komt is er ook nog een whatsapp groep aangemaakt. Hier kan het teamlid dan melden waarom de persoon te laat. Als team hebben hebben we de afspraak dat er minimaal een keer per 24u op teams worden gekeken. Dit met uitzondering van het weekend. Hiermee willen voorkomen dat er berichten ongezien blijven bij mensen van het team.

# 3.Activiteiten en planning

**// Ik heb dit hoofdstuk opgezet stelt functioneel niet veel voor naderhand gezien kloppen de datums tenminste wel**

## 3.1Fases van het project

De hoofd fases binnen het project zijn de planning en implementatie fases waar we ervoor zorgen dat we in de volgende sprint kunnen beginnen met user stories te verwerken. Dan hebben we de development phase waar alle user stories verwerkt worden en we meer en meer van de applicatie gaan opleveren. Tenslotte hebben we dan nog een afronding/ test fase waar we de laatste dingen toevoegen er ervoor zorgen dat alles goed werkt.

## 3.2Planning en doelstellingen

| **Fases** | **Start datum** | **Eind datum** |
| --- | --- | --- |
| Planning en implementatie fase (spring 0)| 14/2/2022 | 7/3/2022 |
| Sprint 1 | 7/3/2022 | 28/3/2022 |
| Sprint 2 | 28/3/2022 | 19/4/2022 |
| Sprint 3 | 19/4/2022 | 16/5/2022 |
| Sprint 4 | 16/5/2022 | 7/6/2022 |
| Afronding en test fase | 7/6/2022 | 20/6/2022 |

# 4.Strategisch testen en configurerend management

## 4.1Strategisch Testen

Voor het testen van de back-end gaan we unit tests gebruiken. Met de unit tests kunnen we losse stukken code onafhankelijk controleren op eventuele bugs. Wanneer deze tests succesvol zijn uitgevoerd wordt via SonarCloud nogmaals over de code heen gekeken. Dit externe software hulpmiddel zorgt ervoor dat duplicated code, coding standards, unit tests, code coverage en security recommendations worden gedetecteerd of weergegeven. Zowel de unit tests als SonarCloud werken automatisch wanneer zij eenmaal zijn opgezet.
# 2

Voor het controleren van endpoints en responses tussen de back-end en de front-end maken we gebruik van het programma Postman. Ook kan het worden gebruikt voor het debuggen van de API&#39;s en het bouwen van onze applicatie op een relatief eenvoudige manier. Kortom het is een handige tool voor het creëren, delen, testen en documenteren van RESTful API&#39;s.

De Front-end word getest met selenium test om te checken of de buttons werken en of er een element veranderd. Om te Controleren of het werkende elementen en componenten zijn. Die voldoen aan de eisen.

## 4.2Test omgeving en vereiste bronnen

Voor de continuous integration, afgekort CI, willen we Azure DevOps gebruiken. Tijdens het pushen van de code via Github kan via deze CI pipelines worden bijgehouden welke testen slagen en welke niet. Het idee erachter is dat deze testen automatisch worden gedraaid wanneer Github een verandering in de code ontvangt. Voor de continues deployment, afgekort CD, gedeelte willen we het via Docker gaan gebruiken. We plaatsen de backend, frontend en de database ieder als aparte image op Docker.

## 4.3Configuratie management

Voor de configuratie management gebruikt ons team Github (https://github.com/s3gp-foodies)

We hebben drie repos voor de drie softwarecomponenten van het project. Elke repo heeft een main branch waar de &quot;productie&quot; versie van de applicatie staat, een dev branch waar de meest recente stabiele versie op staat en een set feature branches waarop aan user stories wordt gewerkt. Directe commits naar de main en dev branches zijn niet mogelijk. Merge requests naar de dev worden na het halen van de CI tests, code review en acceptatie tests uitgevoerd. Wanneer een nieuwe &quot;productie&quot; versie klaar is wordt een merge request van dev naar main gemaakt. Deze moet ook aan dezelfde tests voldoen voordat het uit wordt gevoerd.

# 5.Financien en risico&#39;s

**// hier heb ik de meerderheid van de risico&#39;s en preventie en mitigatie activiteiten bedacht en opgeschreven**

## 5.1Risico en Mitigatie

| **Risico** | **Preventie activiteiten** | **Mitigatie activiteiten** |
| --- | --- | --- |
|1. Groepslid is ziek| Eigen verantwoordelijkheid | Corona check doen voordat naar locatie komen. |
|1. Docent is ziek|| Is aan de docent | Vragen voorbereiden voor als de docent weer beter is. |
|1. Treinen rijden niet|| Op de NS site site kijken | Vanuit huis werken. |
| 4 Treinen hebben vertraging | Op de NS site site kijken | Melden in WhatsApp groep |
| 5 Groepslid doet minder of zijn werk niet | Stand up check en in contact blijven | Aanspreken erop en bij herhalend gedrag consequenties opleggen. |

[1](#sdfootnote1anc) &quot;Wat is Scrum? Hoe werkt het? - Lean Six Sigma Groep.&quot; [https://leansixsigmagroep.nl/lean-agile-en-six-sigma/scrum/](https://leansixsigmagroep.nl/lean-agile-en-six-sigma/scrum/). Geopend op 15 feb.. 2022.

[2](#sdfootnote2anc) &quot;Wat is Postman? — SYSQA — Quality Assurance.&quot; [https://sysqa.nl/veelgestelde-vragen-over-quality-assurance-in-it/veelgestelde-vragen-over-testautomatisering-en-test-tools/wat-is-postman/](https://sysqa.nl/veelgestelde-vragen-over-quality-assurance-in-it/veelgestelde-vragen-over-testautomatisering-en-test-tools/wat-is-postman/). Geopend op 15 feb.. 2022.

Projectplan page 15 from 15
