Methodiek voor Informatiebeveiligingsonderzoek met Auditwaarde
==============================================================

# Over dit document

## Voorwoord
Of een netwerk, systeem of software veilig is, is voor veel mensen lastig weer te geven. Er zijn certificeringen die naar procedures kijken, maar het technisch testen blijft een ingewikkeld thema. Hoe moet je kijken naar een rapportage als je er geen helder kader is? Welke zekerheden heb je dan? En hoe kan een technisch onderzoek dan goed dienen als input voor een certificering? Na diverse incidenten in de industrie, veel ervaringen bij het doen van (technisch) onderzoek naar producten, maar ook naar incidenten is duidelijk dat we meer houvast nodig hebben.  

Bij iets fysieks als een woning zijn de maatregelen makkelijk vanaf lijsten te controleren (heb je buitenverlichting, gecertificeerde sloten, verstevigd deurbeslag, een alarmsysteem, camerasysteem en andere zaken). Bij netwerken en software is het speelveld complexer, maar niet wezenlijk verschillend: er zijn verschillende lijsten met onderzoeken (checklists) die je kunt doorlopen. Het is minder magie dan soms in de industrie wordt beweerd. Maar wat zijn tests die je minimaal wilt hebben doorlopen om een beetje een eerlijk beeld van de staat van beveiliging te hebben?  

Daarvoor is deze methodiek ontwikkeld. Het doel is helder: een technisch gericht onderzoek moet een daadwerkelijk iets op tafel legt dat zekerheden biedt. Niet alleen voor de directe ontvanger, maar ook bij bijvoorbeeld een auditor moet erop kunnen vertrouwen dat dit onderzoek de vragen beantwoordt. Daarom is de methodiek opgesteld om iedere stap niet alleen navolgbaar maar ook onweerlegbaar te maken. De navolgbaarheid en onweerlegbaarheid maken dat er sprake is van enige auditwaarde. Het is duidelijk wat er is onderzocht, hoe dat is gedaan en wat het resultaat van dat onderzoek is, waarbij het onderliggende bewijs beschikbaar is om onderzoek te reproduceren of beschikbaar te stellen aan bijvoorbeeld toezichthouders zoals bijvoorbeeld de NIS2 dat vraagt. Alles bij elkaar geeft het een waarom u vertrouwen in een product heeft.

Centraal bij de methodiek staat dat het onderzoek gericht is op feitelijk onderzoek gebaseerd op belangrijke en relevante (internationale) standaarden. Wij brengen dat bij elkaar brengt voor onderzoek, rapportage en het bepalen van de ernst van een bevinding als er onvolkomenheden worden gevonden. Door dat uniform te doen praten we over hetzelfde, wordt veel emotie uit het debat gehaald en kan een discussie op inhoud worden gevoerd.

Het levert niet alleen informatie, te zetten stappen, een handleiding om informatie-beveiligingsonderzoek goed in te schatten, maar ook inkoopeisen, processchema’s en standaardrapportages. Waar mogelijk worden deze ook in relevante tools meegenomen. Daarmee sluiten we niemand en is voldoen aan de methodiek niet ingewikkeld en bannen we alle magie uit om tot navolgbaar onderzoek te komen. 

Het langslopen van de noodzakelijke eisen kan alleen goed werken als vraag en antwoord goed op elkaar zijn afgestemd. Van vraagstelling tot toetsing van het eindrapport levert de methodiek de nodige informatie en modellen. Waar gaten vielen, zoals bij veel juridische aspecten, hebben we deze zo goed mogelijk opgevuld. Op die manier geeft deze methodiek houvast voor een eerlijk, objectief beeld bij uitgevoerd onderzoek, waarbij de rapportage inkleuring geven bij de eisen die de Europese wetgever meer en meer stelt aan informatiebeveiliging. 

Het informatiebeveiligingsonderzoek met auditwaarde draait om een aantal zekerheden, die aan het onderzoek is te ontleden:
1. Duidelijkheid in deskundigheid. Op basis van de certificering is duidelijk dat het onderzoek is uitgevoerd onder verantwoordelijkheid van iemand die afdoende is geschoold.
2. Duidelijkheid in compleetheid. Op basis van de standaarden, die volledig worden uitgelopen, is er zekerheid dat de testen die minimaal moeten worden uitgevoerd zijn uitgevoerd. Als deze niet relevant zijn of niet kunnen dan is dat gedocumenteerd. U weet dat er een compleet onderzoek is uitgevoerd.
3. Duidelijkheid in proces. Er is een duidelijk en helder omschreven proces dat volledig is uitgelopen. 
4. Duidelijkheid over context. Op basis van de beschikbare informatie is precies duidelijk welke context-informatie wel of niet beschikbaar is. 
5. Duidelijkheid in scope. Het is duidelijk wat er precies is onderzocht.
6. Duidelijkheid in onderzoek. Het is duidelijk welke onderzoeken er precies zijn uitgevoerd en dat deze passend bij het product zijn.
7. Duidelijkheid in bewijsvoering. Het onderzoeksbewijs is beschikbaar om reproduceerbaarheid te bieden aan anderen (en daarmee auditwaarde aan het onderzoek toe te voegen) en bewijs te bieden dat het onderzoek is uitgevoerd.
8. Duidelijkheid in bevindingen. Bij bevindingen wordt uniform en zo objectief mogelijk gecommuniceerd over gevonden problemen, de impact en mogelijke oplossingsrichtingen.

Dit document is het product van het bundelen van veel kennis en lering trekken uit incidenten. Natuurlijk staat informatiebeveiliging niet stil en zal het document regelmatig aan de nieuwe praktijk moeten worden bijgesteld. Ondertussen heeft u eindelijk een stuk houvast in handen. Succes!

## Inrichting van het document
Dit document is opgebouwd in diverse onderdelen, waardoor alle elementen van technisch informatiebeveiligingsonderzoek goed aan bod komen. Het valt uiteen in een aantal secties. 

De eerste sectie ‘Over informatiebeveiligingsonderzoek’ beschrijft de juridische aspecten, de soorten onderzoek en andere relevante onderdelen van informatiebeveiligingsonderzoek. 

In de tweede sectie ‘Informatiebeveiligingsonderzoek uitvoeren’ volgt het (laten) uitvoeren van een dergelijk onderzoek. In de derde sectie ‘Informatiebeveiligingsonderzoek toetsen’ treft u de stappen voor het toetsen van een ontvangen rapportage aan. 

In de derde sectie 'Juridische aspecten' komen de juridische aspecten aan bod. Dit gaat enerzijds over verplichtingen die er zijn om tot deugdelijk onderzoek te komen alsmede de juridische aspecten bij het uitvoeren van het informatiebeveiligingsonderzoek.

Tot slot zijn er in de laatste sectie verschillende onderliggende stukken opgenomen in de appendices.

## Versie historie
* 0.01 - Juli 2020 - Eerste draft met inkoopeisen - Brenno de Winter
* 0.02 - December 2020 - Nadere testeisen - Brenno de Winter
* 0.03 - Mei 2021 - Toetscriteria voor beoordelen pentesten - Brenno de Winter
* 0.04 - Januari 2023 - Uitwerking samenvoeging versie - Brenno de Winter
* 0.1 - Februari 2023 - Aanzet integrale methodologie - Ed Lute
* 0.2 - Augustus 2023 - Nadere inkleuring methodologie op basis feedbackronde - Ed Lute
* 0.5 - December 2023 - Herstructurering, nader in lijn brengen met bestaande standaarden - Jeroen Diel, Mischa van Geelen, Brenno de Winter
* 0.51 - December 2023 - Juridische aspecten - Victor de Pous
* 0.52 - December 2023 - Nieuwe opzet - Brenno de Winter
* 0.53 - Januari 2024 - Herstructureren en herschrijven - Brenno de Winter
* 0.54 - Maart 2024 - Omgezet naar markdown-formaat en beschikbaar stelling via github.com.
* 0.55 - Juni 2024 - verbeteringen in aanloop naar CIP conferentie.

# Over informatiebeveiligingsonderzoek

## Waarom doe je informatiebeveiligingsonderzoek?

Technisch informatiebeveiligingsonderzoek, zoals een bijvoorbeeld een penetratietest (pentest) of een review van de broncode, wordt uitgevoerd om de beveiliging van een IT-systeem of netwerk te beoordelen. Het doel is om zekerheid te krijgen over de staat van het systeem en de effectiviteit van de bestaande beveiligingsmaatregelen. Het levert inzicht in kwetsbaarheden en zwakke punten in de meeste gevallen voordat kwaadwillende partijen dit doen. Een pentest simuleert aanvallen op het systeem om te bepalen hoe goed het bestand is tegen pogingen tot inbraak of compromittering. Tot slot helpt informatie-beveiligingsonderzoek bij het verbeteren van de algehele beveiligingshouding van de organisatie door het aanbevelen van verbeteringen en versterkingen.

## Definities voor informatiebveiligingsonderzoek 
Eenheid van taal met betrekking tot computersystemen en netwerken ontbreekt soms in de ICT. Dit gebrek strekt zich uit tot zowel de gebruikte terminologie als de betekenis die aan bepaalde termen wordt toegekend. Bovendien ontbreekt vaak de verbinding tussen het technische jargon en het juridische kader. Hierdoor kunnen niet alleen verwarring en problemen ontstaan bij de aanschaf, ontwikkeling en/of het beheer van ICT, maar neemt ook het risico op schending van wettelijke voorschriften en juridische aansprakelijkheid toe.

## Uniforme taal noodzakelijk
In de praktijk kan er verwarring ontstaan omdat er verschillende type digitaal-gerelateerde veiligheidsonderzoeken mogelijk zijn en worden uitgevoerd, omdat er geen eensduidendheid is over terminologie en betekenis. Bovendien kan het schorten aan de verbinding met recht, terwijl ook bestuur en management als eindverantwoordelijke voor ICT en digitale veiligheid algemeen hiermee te maken hebben en bijvoorbeeld als opdrachtgever van veiligheidsonderzoeken in het bijzonder. Van het palet aan onderzoeken maken onder andere deel uit:
* Assessment of cybersecurity risks
* Assume breach-benadering
* Code review
* Conformiteitsbeoordeling
* Failure mode and effects analysis (FMEA)
* Gegevensbeschermingseffectbeoordeling (“data protection impact assessment” of DPIA)
* Penetratietest
* Dreigingsgestuurde penetratietest
* Red Teaming
* Security audit
* Security assessment
* Threat Intelligence Based Ethical (TIBER)
* Vulnerability scan

Afbakening en begripsvorming ondersteunen en verbeteren digitale kwaliteit en weerbaarheid, terwijl tegelijkertijd feitelijke risico’s en juridische aansprakelijkheid wegens niet naleving van wettelijke voorschriften kunnen worden beperkt. Het is dus aan te bevelen om duidelijkheid en consistentie te waarborgen in digitaal veiligheid, het proces digitaal veiligheidsonderzoek en uiteindelijke ICT algemeen. 

Vaste terminologie voor allerhande digitale veiligheidsonderzoeken is echter van beperkte waarde indien een zorgvuldig-geformuleerde omschrijving van de inhoud van een bepaald onderzoek geen verbinding maakt het rechtskader. Of vice versa gesteld: “eenheid van taal” voor digitaal veiligheidsonderzoek in overeenstemming met wettelijke definities, indien beschikbaar, biedt praktische aanknopingspunten voor:
* het upgraden van het veiligheidsonderzoek in het kader van informatiebeveiligingsbeleid om de digitale weerbaarheid te verbeteren
* het aan sluiten op wettelijke voorschriften (zorgplichten, meldplichten, verantwoordingsplichten) en het voorkomen van juridische risico’s en aansprakelijkheid
* het gestructureerd uitvoeren en controleren van digitaal veiligheidsbeleid
* het opstellen van (model)overeenkomsten en clausules

Bij contracten kan bijvoorbeeld worden gedacht aan een samenwerkingsovereenkomst tussen ketenpartners waarvan een digitale veiligheidstestcomponent deel uitmaakt of een opdracht aan een externe dienstverlener voor uitvoeren van een digitaal veiligheidsonderzoek. Hierbij wegen aspecten van goed opdrachtgeverschap en het bereiken van het beoogde resultaat van het onderzoek zwaar, omdat deze voorwaarden binnen de context en omvang van het onderzoek (“scope”) bepalend zijn voor een zo optimaal mogelijke en consistente beoordeling van de status van een onderdeel van de netwerk- en informatiebeveiliging. 

De noodzaak tot het volgen van vaste terminologie en de bijbehorende inhoudelijke omschrijving van een digitaal veiligheidsonderzoek in samenhang met het rechtskader wint nog verder aan gewicht indien regulering een bepaald type onderzoek expliciet voorschrijft. Zo kunnen organisaties onder de AVG, de Wet politiegegevens (Wpg) en de Wet justitiële en strafvorderlijke gegevens (Wjsg) verplicht zijn een gegevensbeschermingseffectbeoordeling (DPIA) uit te voeren.  

In dit hoofdstuk vindt u een aantal gangbare digitaal-gerelateerde veiligheidsonderzoeken op, (ii) wijst op door de wetgever benoemde en soms daarbij gedefinieerde onderzoeken en (iii) doet bij gebreke daarvan voorstellen voor werkdefinities voor gebruik binnen WVS Concern. Door de eenduidige wijze van vastlegging wil het WVS/CISO Concern Office onduidelijkheid en misverstand voorkomen, de kwaliteit van onderzoeken verder beteren en daarmee de digitale weerbaarheid verhogen. 

Digitale veiligheidsonderzoeken kunnen verschillende kenmerken hebben. Enkele mogelijkheden. Wie voorafgaand aan levering dan wel livegang van een applicatie gaat testen, voert proactief een veiligheidsonderzoek uit. Van reactief handelen is in dit geval sprake indien er tijdens het draaien in productie een incident heeft voorgedaan.  

Een onderzoek kan verder van buiten naar binnen worden uitgevoerd (offensief) of van binnenuit. Ook een combinatie is mogelijk. Bij ieder digitaal veiligheidsonderzoek stelt de onderzoeker, als regel in nauwe samenspraak met de opdrachtgever, mede van tevoren vast of het onderzoek impact mag hebben. Een **“non-intrusive” digitaal veiligheidsonderzoek** kan bijvoorbeeld het proactief en scannen van openbaar toegankelijke netwerk- en informatiesystemen van essentiële en belangrijke entiteiten behelzen, zoals een benoemde wettelijke taak voor een computer security incident respons team (CSIRT), maar zonder negatieve gevolgen voor de bedrijfsvoering. 

> “Een dergelijk scannen wordt uitgevoerd om kwetsbare of onveilig geconfigureerde netwerk- en informatiesystemen op te sporen en de betrokken entiteiten te informeren. Een dergelijk scannen mag geen negatieve gevolgen hebben voor de werking van de diensten van de entiteiten” (art. 11, lid 3 NIS2).

Het is overigens goed om te beseffen dat digitale veiligheid-gerelateerde begrippen, ook indien deze juridisch zijn geformaliseerd, kunnen wijzigen, zoals uit Europese wetgeving blijkt.

## Definitielijst
Omdat het vaak bij informatiebeveiligingsonderzoek onduidelijk is wat een bepaalde term betekent, leidt dit tot spraakverwarring en onduidelijk wat er nu van diensten verwacht mag worden. In sommige gevallen is in wetgeving vastgelegd wat woorden betekenen en soms is gezocht naar een heldere beschrijving. Daarom is een definitielijst opgesteld, waarbij zoveel mogelijk aansluiting is gezocht bij wettelijke kaders, zodat dit bij een informatiebeveiligingsonderzoek met auditwaarde de terminologie zoveel mogelijk zekerheid biedt:
* Actively exploited vulnerability. An actively exploited vulnerability is “a vulnerability for which there is reliable evidence that execution of malicious code was performed by an actor on a system without permission of the system owner”. (art. 2 , punt 39 ontwerp-CRA)
* Assessment of cybersecurity risks. Een assessment of cybersecurity risks is “de door de fabrikant uit te voeren beoordeling van de cybersecurity-risico’s in verband met een product met digitale elementen om relevante risico’s en relevante essentiële vereisten te identificeren en om geschikte geharmoniseerde normen of gemeenschappelijke specificaties op de juiste manier toe te passen”. (overweging 32 juncto art. 10, lid 2 ontwerp-CRA)
* Assume breach benadering. Een assume breach benadering is “een digitaal veiligheidsonderzoek waarbij een organisatie haar interne computersystemen en netwerken onderzoekt met de aanname dat er al een inbreuk op de beveiliging ervan heeft plaatsgevonden, om voorbereid op dit scenario te zijn en door snel reageren schade te kunnen beperken”.
* Bijna incident. Een bijna incident is een gebeurtenis die de beschikbaarheid, authenticiteit, integriteit of vertrouwelijkheid van opgeslagen, verzonden of verwerkte gegevens of van de diensten die worden aangeboden door of toegankelijk zijn via netwerk- en informatiesystemen, in gevaar had kunnen brengen, maar die met succes is voorkomen of zich niet heeft voorgedaan. (art. 6, onder 5 NIS2).
* Codereview. Een codereview is “een door eigen personeel of derden uit te voeren onderzoek naar de technische kwaliteit van de broncode van software, inclusief veiligheidsaspecten, door anderen dan degenen die aan het ontwerp en de bouw hebben gewerkt”.
* Conformiteitsbeoordeling. Een conformiteitsbeoordeling is “the process of verifying whether the essential requirements set out in the standard have been fulfilled.” (naar art. 2, punt 28 ontwerp-CRA).
* Cyberdreiging. Een cyberdreiging is “elke potentiële omstandigheid, gebeurtenis of actie die netwerk- en informatiesystemen, de gebruikers van dergelijke systemen en andere personen kan schaden, verstoren of op andere wijze negatief kan beïnvloeden”. (art. 2, onder 1 CSA en art. 2, punt 8 Verordening EU/2019/881)
* Digitale Operationele Weerbaarheid. Digitale operationele weerbaarheid is “het vermogen van een financiële entiteit om haar operationele integriteit en betrouwbaarheid op te bouwen, te waarborgen en te evalueren, door direct of indirect via gebruik van diensten die door derde aanbieders van ICT-diensten worden verleend te voorzien in het volledige scala van ICT-gerelateerde capaciteiten die nodig zijn voor de beveiliging van de netwerk- en informatiesystemen waarvan een financiële entiteit gebruikmaakt, en die de permanente verlening van financiële diensten en de kwaliteit ervan, onder meer gedurende storingen, ondersteunen”  (art. 3, lid 1 DORA)
* Data Protection Impact Assessment (DPIA). Een DPIA is “een met het oog op een mogelijk hoog privacyrisico voor betrokkenen door de verwerkingsverantwoordelijke door eigen personeel of derden uit te voeren beoordelingsonderzoek naar het effect van beoogde of reeds bestaande verwerkingsactiviteiten op de bescherming van persoonsgegevens”. (artikel 35 AVG)
* Dreigingsgestuurd penetratietesten. Het dreigingsgestuurd penetratietesten (threat led penetration testing — TLPT) is “een kader waarin de tactiek, technieken en procedures van levensechte, als een reële cyberdreiging ervaren dreigingsactoren worden nagebootst en waarin een gecontroleerde, op maat gesneden, door inlichtingen gestuurde (red team) test van de kritieke reëel bestaande productiesystemen van de financiële entiteit wordt voorgebracht”. (art. 3, lid 17 DORA). Zie in dit kader ook Red Teaming.
* Failure Mode and Effect Analysis (FMEA). Een FMEA is “een intern of extern uit te voeren onderzoek om risico’s op basis van het werken van fouten binnen ICT-projecten of processen te identificeren en te prioriteren alsmede het benoemen van preventieve, detectieve en repressieve acties.”
* Gegevensbeschermingseffectbeoordeling. Zie DPIA
* Grootschalig cyberbeveiligingsincident. Een grootschalig cyberbeveiligingsincident is “een incident dat leidt tot een verstoringsniveau dat te groot is om door een getroffen lidstaat alleen te worden verholpen of dat significante gevolgen heeft voor ten minste twee lidstaten”. (art. 6, onder 7 NIS2).
* Inbreuk in verband met persoonsgegevens. Een inbreuk in verband met persoonsgegevens is “een inbreuk op de beveiliging die per ongeluk of op onrechtmatige wijze leidt tot de vernietiging, het verlies, de wijziging of de ongeoorloofde verstrekking van of de ongeoorloofde toegang tot doorgezonden, opgeslagen of anderszins verwerkte gegevens”. (art. 4, onder 12 AVG).
* Incident. Een incident is “een gebeurtenis die de beschikbaarheid, authenticiteit, integriteit of vertrouwelijkheid van opgeslagen, verzonden of verwerkte gegevens of van de diensten die worden aangeboden door of toegankelijk zijn via netwerk- en informatiesystemen, in gevaar brengt”. (art. 6, onder 6 NIS2).
* Incidentafhandeling. Incidentafhandeling zijn “alle acties en procedures die gericht zijn op het voorkomen, opsporen, analyseren en indammen van of het reageren op en het herstellen van een incident”. (art. 6, onder 8 NIS2)
* Informatiebeveiligingsonderzoek met auditwaarde is “een door eigen personeel of derden uitgevoerde security assessment met inbegrip van een security assessment dat conform de beschirjving in dit document is uitgevoerd, waarbij de testen conform open standaarden, het onderzoek volledig reproduceerbaar is en is gedocumenteerd conform de daarvoor geselecteerde standaard”.
* Kwetsbaarheid. Een kwetsbaarheid is “een zwakheid, vatbaarheid of gebrek van ICT-producten of ICT-diensten die door een cyberdreiging kan worden uitgebuit”. (art. 6, punt 15 NIS2)
* Penetratietest. Een penetratietest (pentest) is “een door eigen personeel of derden uit te voeren offensief veiligheidsonderzoek, waarbij gecontroleerd wordt gezocht naar kwetsbaarheden in een of meer beveiligde netwerk- en informatiesystemen of onderdelen daarvan, die kunnen worden gebruikt voor het inbreken in deze systemen en/of die zonder opzet en autonoom de gegevensverwerking van de onderzochte organisatie kunnen verstoren of anderszins nadelige gevolgen kunnen hebben”.
* Thread Lead Pentesting. Zie dreigingsgestuurde penetratietesten.
* Red Teaming. Red Teaming is “het door eigen personeel en/of derden uit te voeren onderzoek naar zwakheden van netwerk- en informatiesystemen, processen en mensen op een manier die verder kan gaan dan een pentest en bijvoorbeeld mede fysieke toegangsverschaffing en social engineering omvat, waarbij de relatie tussen het digitale en fysieke domein centraal staat”.
* Risico. Een risico is “de mogelijkheid van verlies of verstoring als gevolg van een incident, wat wordt uitgedrukt als een combinatie van de omvang van een dergelijk verlies of verstoring en de waarschijnlijkheid dat het incident zich voordoet”. (art. 3, onder 14 NIS2) 
* Security assessment. Een security assessment is “het door eigen personeel en/of derden uit te voeren onderzoeken van de management-, operationele en technische beveiligings-controls in netwerk- en informatiesystemen om te bepalen in hoeverre de controls correct worden geïmplementeerd, werken zoals bedoeld en de gewenste uitkomst produceren met betrekking tot het voldoen aan de beveiligingsvereisten voor deze systemen”.
* Security audit. Een security audit is “een door in beginsel een externe register auditor uit te voeren onderzoek om de naleving te controleren van de bij wet- en regelgeving en/of bij overeenkomst voorgeschreven veiligheidsvoorschriften in verband netwerk- en informatiesystemen of onderdelen daarvan”.
* Significant Cybersecurity Risk. A significant cybersecurity risk is “a cybersecurity risk which, based on its technical characteristics, can be assumed to have a high likelihood of an incident that could lead to a severe negative impact, including by causing considerable material or non-material loss or disruption”. (art. 3, onder 36 ontwerp-CRA)
* Verwerking van gegevens. Verwerking van gegevens is “een bewerking of een geheel van bewerkingen met betrekking tot gegevens of een geheel van gegevens, al dan niet uitgevoerd via geautomatiseerde procedés, zoals het verzamelen, vastleggen, ordenen, structureren, opslaan, bijwerken of wijzigen, opvragen, raadplegen, gebruiken, verstrekken door middel van doorzending, verspreiden of op andere wijze ter beschikking stellen, aligneren of combineren, afschermen, wissen of vernietigen van gegevens”. (AVG aangepast naar gegevens).
* Vulnerability scan. Een vulnerabilityscan is “een door eigen personeel en/of derden uit te voeren geautomatiseerd onderzoek naar bekende kwetsbaarheden waarvan misbruik is en/of wordt gemaakt (CVE’s) in ICT-producten of ICT-diensten die door een cyberdreiging kunnen worden uitgebuit”.
* Een omgeving. Met omgeving wordt het geheel van servers en software bedoeld dat nodig is om specifieke functionaliteiten aan te kunnen bieden.


