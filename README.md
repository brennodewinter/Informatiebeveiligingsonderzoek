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
2. Duidelijkheid in proces. Op basis van het te doorlopen proces is duidelijk welke taken er worden uitgevoerd.
3. Duidelijkheid over context. Op basis van de beschikbare informatie is precies duidelijk welke context-informatie wel of niet beschikbaar is. 
4. Duidelijkheid in scope. Het is duidelijk wat er precies is onderzocht.
5. Duidelijkheid in onderzoek. Het is duidelijk welke onderzoeken er precies zijn uitgevoerd en dat deze passend bij het product zijn.
6. Duidelijkheid in bewijsvoering. Het onderzoeksbewijs is beschikbaar om reproduceerbaarheid te bieden aan anderen (en daarmee auditwaarde) en bewijs te bieden dat het onderzoek is uitgevoerd.
7. Duidelijkheid in bevindingen. Bij bevindingen wordt uniform en zo objectief mogelijk gecommuniceerd over gevonden problemen, de impact en mogelijke oplossingsrichtingen.

Dit document is het product van het bundelen van veel kennis en lering trekken uit incidenten. Natuurlijk staat informatiebeveiliging niet stil en zal het document regelmatig aan de nieuwe praktijk moeten worden bijgesteld. Ondertussen heeft u eindelijk een stuk houvast in handen. Succes!

## Inrichting van het document
Dit document is opgebouwd in diverse onderdelen, waardoor alle elementen van technisch informatiebeveiligingsonderzoek goed aan bod komen. Het valt uiteen in een aantal secties. De eerste sectie ‘Over informatiebeveiligingsonderzoek’ beschrijft de juridische aspecten, de soorten onderzoek en andere relevante onderdelen van informatiebeveiligingsonderzoek. In de tweede sectie ‘Informatiebeveiligingsonderzoek uitvoeren’ volgt het (laten) uitvoeren van een dergelijk onderzoek. In de derde sectie ‘Informatiebeveiligingsonderzoek toetsen’ treft u de stappen voor het toetsen van een ontvangen rapportage aan. Tot slot zijn er in de laatste sectie verschillende onderliggende stukken opgenomen in de appendices.

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
* Penetratietest. Een penetratietest (pentest) is “een door eigen personeel of derden uit te voeren offensief veiligheidsonderzoek, waarbij wordt gezocht naar kwetsbaarheden in een of meer beveiligde netwerk- en informatiesystemen of onderdelen daarvan, die kunnen worden gebruikt voor het inbreken in deze systemen en/of die zonder opzet en autonoom de gegevensverwerking van de onderzochte organisatie kunnen verstoren of anderszins nadelige gevolgen kunnen hebben”.
* Thread Lead Pentesting. Zie dreigingsgestuurde penetratietesten.
* Red Teaming. Red Teaming is “het door eigen personeel en/of derden uit te voeren onderzoek naar zwakheden van netwerk- en informatiesystemen, processen en mensen op een manier die verder kan gaan dan een pentest en bijvoorbeeld mede fysieke toegangsverschaffing en social engineering omvat, waarbij de relatie tussen het digitale en fysieke domein centraal staat”.
* Risico. Een risico is “de mogelijkheid van verlies of verstoring als gevolg van een incident, wat wordt uitgedrukt als een combinatie van de omvang van een dergelijk verlies of verstoring en de waarschijnlijkheid dat het incident zich voordoet”. (art. 3, onder 14 NIS2) 
* Security assessment. Een security assessment is “het door eigen personeel en/of derden uit te voeren onderzoeken van de management-, operationele en technische beveiligings-controls in netwerk- en informatiesystemen om te bepalen in hoeverre de controls correct worden geïmplementeerd, werken zoals bedoeld en de gewenste uitkomst produceren met betrekking tot het voldoen aan de beveiligingsvereisten voor deze systemen”.
* Security audit. Een security audit is “een door in beginsel een externe register auditor uit te voeren onderzoek om de naleving te controleren van de bij wet- en regelgeving en/of bij overeenkomst voorgeschreven veiligheidsvoorschriften in verband netwerk- en informatiesystemen of onderdelen daarvan”.
* Significant Cybersecurity Risk. A significant cybersecurity risk is “a cybersecurity risk which, based on its technical characteristics, can be assumed to have a high likelihood of an incident that could lead to a severe negative impact, including by causing considerable material or non-material loss or disruption”. (art. 3, onder 36 ontwerp-CRA)
* Verwerking van gegevens. Verwerking van gegevens is “een bewerking of een geheel van bewerkingen met betrekking tot gegevens of een geheel van gegevens, al dan niet uitgevoerd via geautomatiseerde procedés, zoals het verzamelen, vastleggen, ordenen, structureren, opslaan, bijwerken of wijzigen, opvragen, raadplegen, gebruiken, verstrekken door middel van doorzending, verspreiden of op andere wijze ter beschikking stellen, aligneren of combineren, afschermen, wissen of vernietigen van gegevens”. (AVG aangepast naar gegevens).
* Vulnerability scan. Een vulnerabilityscan is “een door eigen personeel en/of derden uit te voeren geautomatiseerd onderzoek naar bekende kwetsbaarheden waarvan misbruik is en/of wordt gemaakt (CVE’s) in ICT-producten of ICT-diensten die door een cyberdreiging kunnen worden uitgebuit”. 

# Informatiebeveiligingsonderzoek met auditwaarde
Om te kunnen spreken van een Informatiebeveiligingsonderzoek met auditwaarde moet aan een aantal zaken worden voldaan:

## Duidelijkheid in deskundigheid. Op basis van de certificering is duidelijk dat het onderzoek is uitgevoerd onder verantwoordelijkheid van iemand die afdoende is geschoold.
Om het onderzoek deugdelijk te kunnen uitvoeren wordt het onderzoek uitgevoerd door iemand, die over een minimaal niveau van kennis beschikt met betrekking tot het doen van informatiebeveiligingsonderzoek met auditwaarde. Deze persoon is de rapporteur voor het onderzoek en staat in voor de correctheid van het onderzoek. Deze gecertificeerde persoon voert het onderzoek uit of laat het onderzoek (deels)onder zijn of haar auspiciën uitvoeren. Van het gecertificeerd zijn, levert de rapporteur bewijs aan in de vorm van een validatielink of een kopie van een diploma. Er vindt ondertekening plaats dat de verstrekte informatie in de rapportage correct is.   

### EIS: 1.1 Aanwijzing rapporteur, opsteller of hoofdonderzoeker.
**EIS:**
> De rapportage vermeldt de naam van de rapporteur.

Wat levert het op: Dit maakt het mogelijk vast te stellen wie het onderzoek heeft uitgevoerd en wie professionele verantwoordelijkheid draagt. Het maakt het mogelijk te valideren dat deze persoon beschikt over voldoende certificering om professioneel te kunnen optreden.

### EIS 1.2 Benoeming van de certificering, waarover de rapporteur beschikt
**EIS:**
> De rapportage benoemt de certificering(en), waarover de rapporteur beschikt. Geldige certificeringen zijn:
> * OffSec Certified Professional (OSCP)
> * OffSec Experienced Pentester (OSEP)
> * OffSec Offensive Security Certified Expert (OSCE of OSCE³)
> * OffSec Web Expert (OSWE)
> * Web application Penetration Tester eXtreme (eWPTX)

Wat levert het op: Deze certificeringen bieden een niveau van zekerheid dat de onderzoeker beschikt over een minimaal niveau aan opleiding en deze beschikt over voldoende kennis om een examen te kunnen doorstaan. Dat maakt de onderzoeker een professionele partner voor het onderzoek. 

De geselecteerde certificeringen zijn gebaseerd op het kwalificatieschema van het [CCV Keurmerk Pentesten](https://hetccv.nl/app/uploads/2023/09/20230921-Kwalificaties-pentester.pdf).

### EIS 1.3 Bewijs certificering
**EIS:**
> De rapportage levert bewijs van de certificering in de vorm van een link naar een online validatieplatform om de authenticiteit van de geclaimde certificering te valideren of een kopie van het diploma, waardoor andere validatie mogelijk is.

Wat levert het op: Dit maakt het mogelijk om vast te stellen dat de rapporteur van de rapportage inderdaad beschikt over de geclaimde certificering, waaruit professionaliteit blijkt.

### EIS 1.4 Benoemen van de versie van de rapportage
**EIS:**
Er wordt in de passage over de deskundigheid melding gemaakt van het versienummer van het document.

Wat levert het op: Dit maakt duidelijk voor welke versie van het document wordt getekend.

### EIS 1.5 Handtekening voor waarheidsgetrouwe rapportage
**EIS:**
> De rapportage wordt voorzien van een tekst, waaruit blijkt dat de rapportage:
> 1. accuraat en naar waarheid is opgesteld;
> 2. er een review op deze versie van het document heeft plaatsgevonden door andere een niet bij het onderzoek betrokken persoon.
> Deze tekst voorzien van een handtekening van de rapporteur. Deze handtekening kan een fysiek gezette handtekening zijn of een digitale handtekening.

**Voorbeeld passage om in rapportage op te nemen**
> Deze rapportage (versie XX.YY) is opgesteld door [NAAM VAN DE HOOFDONDERZOEKER], deze is in het bezit van [NAAM CERTIFICERING] ([LINK NAAR DE VALIDATIESITE VOOR CERTIFICERING VAN DE PERSOON]). Deze rapportage is accuraat en naar waarheid opgesteld. Op deze versie van het document heeft een review plaatsgevonden door iemand, die zelf niet betrokken is bij het uitvoeren van dit informatiebeveiligingsonderzoek.
> 
> __________________________________ (handtekening)

Wat levert het op: Een handtekening onder een rapportage dient als een formeel bewijs van goedkeuring, verantwoordelijkheid en authenticiteit. Het toont aan dat de ondertekenaar instemt met de inhoud van het document, bevestigt dat de informatie naar beste weten correct en compleet is, en draagt juridische en professionele verantwoordelijkheid voor wat erin staat. Dit versterkt het vertrouwen en de geloofwaardigheid van het rapport, zowel intern binnen een organisatie als extern naar stakeholders, klanten, of toezichthoudende instanties. 

## Duidelijkheid in proces. 

## Duidelijkheid over context. Op basis van de beschikbare informatie is precies duidelijk welke context-informatie wel of niet beschikbaar is. 

## Duidelijkheid in scope. Het is duidelijk wat er precies is onderzocht.

## Duidelijkheid in onderzoek. Het is duidelijk welke onderzoeken er precies zijn uitgevoerd en dat deze passend bij het product zijn.

## Duidelijkheid in bewijsvoering. Het onderzoeksbewijs is beschikbaar om reproduceerbaarheid te bieden aan anderen (en daarmee auditwaarde) en bewijs te bieden dat het onderzoek is uitgevoerd.

## Duidelijkheid in bevindingen. Bij bevindingen wordt uniform en zo objectief mogelijk gecommuniceerd over gevonden problemen, de impact en mogelijke oplossingsrichtingen.


# Juridische Aspecten van Informatiebeveiligingsonderzoek
## Algemeen 
Al jaren is het in Nederland een verplichting om maatregelen te nemen om de ICT-omgevingen te beschermen tegen inbreuken en andere incidenten. Voor overheidsorganisaties geldt bovendien de verplichting om daarnaast beleid uit te voeren, zoals bijvoorbeeld in de Baseline Informatiebeveiliging Overheid (BIO) staat. Als uitgangspunt maakt het informatiebeveiligingsrecht gebruik van normen. Deze zijn in Nederland en Europa veelal open en gebaseerd op risico. Op basis daarvan moeten beschermingsmaatregelen worden genomen. Dat is de inkleuring van de zorgplichten, die er zijn. 

Maar met het nemen van de maatregelen ben je er niet. Wie verantwoordelijk is voor beveiliging dient ook te verifiëren of daadwerkelijk aan de zorgplicht wordt voldaan. Zijn de vereiste organisatorische en technische beschermingsmaatregelen daadwerkelijk geïmplementeerd, worden ze nageleefd en zijn nog altijd adequaat. De regelgeving vraagt meer en meer dat hierover verantwoording wordt afgelegd. Om hieraan te kunnen voldoen moet er zorgvuldig onderzoek worden uitgevoerd met voldoende bewijs. Daarbij was het vroeger misschien voldoende om te leunen op een certificering. Inmiddels vereist regelgeving het kunnen leveren van het onderliggende bewijs. Dat bewijs maakt duidelijk dat maatregelen zijn genomen en dat er validatie in de vorm van onderzoek heeft plaatsgevonden. 

## Beschikbaarheid, Integriteit en Vertrouwelijkheid 
Computersystemen kunnen fouten en andere onvolkomenheden in soorten en maten bevatten, waardoor de veiligheid van het systeem, netwerk of onderdeel daarvan, zoals een computerprogramma of protocol, wordt verzwakt. Computer- of informatiebeveiliging (“information security”2) ziet toe op het beveiligen van elektronische gegevensverwerking op basis van risicobeperking en betreft het geheel van maatregelen dat zich traditioneel richt op de volgende onderdelen: 
* vertrouwelijkheid (uitsluitend geautoriseerde gebruikers hebben toegang tot de systemen en gegevens);
* integriteit (de verwerkte gegevens zijn volledig en juist); en
* beschikbaarheid (van systemen, waarbij gebruikers toegang hebben).  

Internationaal wordt gesproken van “CIA”: confidentiality, integrity, availability (ISO/IEC 27000:2009). Bij informatiebeveiliging weegt het recht zwaar. Enerzijds zijn er wettelijke definities en voorschriften, zoals zorgplichten en andere regels in de vorm van meldplichten en bijvoorbeeld verantwoordingsplichten. Anderzijds bevatten contracten hierover specifieke afspraken in het concrete geval. Schending van juridische normen uit wet of overeenkomst kan leiden tot privaat-, bestuurs- en/of strafrechtelijke aansprakelijkheid.  

Voor Nederland is mede het communautaire recht van belang. De Europese Commissie kiest daar waar mogelijk tegenwoordig voor het wetgevingsinstrument verordening. Haar rechtstreekste werking ondervangt het probleem van een EU richtlijn van de omzetting van een richtlijn in het nationale recht van 27 lidstaten, waardoor er beleidsmatige, legislatieve en vervolgens jurisprudentiële verschillen in de interne markt ontstaan. Dit laatste is bijvoorbeeld gebeurd met Richtlijn beveiliging netwerk- en informatiesystemen (EU/2016/11480), of wel “NIS”. 

De Richtlijn NIS omschrijft beveiliging van netwerk- en informatiesystemen uitgebreider dan de gangbare CIA-benadering en spreekt mede van authenticiteit:  
> “het vermogen van netwerk- en informatiesystemen om met een bepaalde mate van betrouwbaarheid bestand te zijn tegen acties die de beschikbaarheid, authenticiteit, integriteit en vertrouwelijkheid van de opgeslagen, verzonden of verwerkte gegevens of de daaraan gerelateerde diensten die via die netwerk- en informatiesystemen worden aangeboden of toegankelijk zijn, in gevaar brengen” (art. 4, onder 2 NIS). 

De huidige omschrijving van beveiliging van netwerk- en informatiesystemen wijzigt licht in de Richtlijn NIS2 ((EU)2022/2555) die op 16 januari 2023 in werking trad en van toepassing wordt op 18 oktober 2024: 
> “het vermogen van netwerk- en informatiesystemen om op een bepaald niveau van betrouwbaarheid weerstand te bieden aan elke gebeurtenis die de beschikbaarheid, authenticiteit, integriteit of vertrouwelijkheid van opgeslagen, verzonden of verwerkte gegevens of van de diensten die door of via deze netwerk- en informatiesystemen worden aangeboden, in gevaar kan brengen” (art. 6, onder 2 NIS2). 

De zinsnede “bepaalde *mate* van betrouwbaarheid bestand te zijn tegen *acties*” is gewijzigd in “bepaald *niveau* van betrouwbaarheid weerstand te bieden aan *elke gebeurtenis*”. 

Daarnaast geldt Verordening (EU) 2019/881 die het EU-Agentschap voor cyberveiligheid (ENISA) versterkt en een raamwerk voor cybersecurity-certificering voor producten en diensten vaststelt. Deze Cybersecuirty Act (CSA) definieert cyberbeveiliging als: 
> “de activiteiten die nodig zijn om netwerk- en informatiesystemen, de gebruikers van dergelijke systemen, en andere personen die getroffen worden door cyberdreigingen, te beschermen” (art. 2, onder 1 CSA).
Dezelfde definitie komt onder meer terug in Richtlijn NIS2 (Art. 4, onder 3). 

Een ander Europese wet - Verordening (EU) 2022/868; Data Governance Act of DGA4 - spreekt van beveiligde verwerkingsomgeving en omschrijft deze omgeving als: 
> “de fysieke of virtuele omgeving en organisatorische middelen om te zorgen voor de naleving van het Unierecht, zoals Verordening (EU) 2016/679, met name wat betreft de rechten van datasubjecten, intellectuele-eigendomsrechten, en handels- en statistisch geheim, integriteit en toegankelijkheid, alsook van het toepasselijke nationale recht, en om de entiteit die de beveiligde verwerkingsomgeving biedt in staat te stellen alle gegevensverwerkingsactiviteiten te bepalen en er toezicht op te houden, met inbegrip van het tonen, opslaan, downloaden en exporteren van gegevens en het berekenen van afgeleide gegevens door middel van computeralgoritmen” (art 2, onder 20 DGA).  

Steeds vaker maken criminele en statelijke actoren gebruik van fouten en andere problemen die digitale technologie en gegevensverwerkingsprocessen verzwakken. Dit vormt een aanzienlijk maatschappelijk probleem, en de trend is stijgende. Het is echter belangrijk om te realiseren dat zwakke informatietechniek in producten en diensten, op zichzelf (autonoom) ook tot incidenten kan leiden, zonder dat daarbij sprake is van opzettelijke handelingen van zowel externe als interne partijen binnen de organisatie. Dit kan directe gevolgen hebben voor de bedrijfsvoering, inclusief verstoringen in of uitval van bedrijfsprocessen. 

## Wettelijke zorgplicht
Voor iedere organisatie geldt vandaag een geconsolideerde, in beginsel risico-gebaseerde, wettelijke zorgplicht, zowel algemeen als soms aanvullend sectoraal, om maatregelen te treffen gericht op bescherming van ICT. Beveiligen van informatie, computersystemen en netwerken moet dus. Hierbij gaat het om dwingend recht op grond van diverse wet- en regelgeving. Daarvan kan niet worden afgeweken. Wel heeft een organisatie in beginsel het recht om zijn verplichtingen te laten vervullen door een derde via uitbesteding, zoals een informatiebeveiligingsdienstverlener. Iedere organisatie blijft echter zelf verantwoordelijk voor haar informatiebeveiliging, onder meer ten opzichte toezichthouders, zoals de Autoriteit Persoonsgegevens en de Rijksinspectie Digitale Infrastructuur (RDI). 

Wie juridisch verplicht is *beschermingsmaatregelen* te treffen, moet daarbij ook controleren en in toenemende mate verantwoording afleggen of de maatregelen zijn geïmplementeerd, worden nageleefd en blijvend passend zijn. Zo zijn aanbieder van een essentiële dienst en digitaledienstverlener verplicht tot het treffen van “*passende en evenredige technische en organisatorische maatregelen om de risico’s voor de beveiliging van hun netwerk- en informatiesystemen te beheersen*”. Hiertoe behoort in ieder geval mede “*toezicht, controle en testen*” (art. 7, lid 1 onder d Wbni).

Ook de Algemene verordening gegevensbescherming ((EU)2016/679) schrijft dit voor. Het gaat om “*een procedure voor het op gezette tijdstippen testen, beoordelen en evalueren van de doeltreffendheid van de technische en organisatorische maatregelen ter beveiliging van de verwerking*” (art. 32, lid 1 onder d AVG). De NIS2 bepaalt dat een van te treffen maatregelen moet zijn “*beveiliging bij het verwerven, ontwikkelen en onderhouden van netwerk- en informatiesystemen, met inbegrip van de respons op en bekendmaking van kwetsbaarheden*” (art. 21, lid 1 onder e NIS2). 

Daarnaast vereist controle op veiligheidsincidenten aandacht en uitvoering. Hiervoor gelden rechtstreekse wettelijke voorschriften (art. 7, lid 1 onder b Wbni, art. 32, lid 1 AVG en bijvoorbeeld art. 21, lid 1 onder b NIS2). Een dergelijk incident kan voor de getroffen organisatie bovendien de algemene juridische verplichting met zich meebrengen tot het voorkomen of beperken van schade (volgens het leerstuk onrechtmatige daad en/of een schadebeperkingsplicht op grond van het overeenkomstenrecht). 

Bovendien geldt er bij de omstandigheid van een veiligheidsincident in bepaalde gevallen complementair een wettelijke meldplicht, zoals onder ander uit de Algemene verordening gegevensbescherming (AVG), Telecommunicatiewet (Tw) en Wet bescherming netwerk- en informatiesystemen (Wbni, de Nederlandse omzetting van de NIS) blijkt. 
 
Controleren of minimaal de verplichte digitale veiligheidsmaatregelen zijn ingevoerd, worden nageleefd en voortdurend adequaat zijn, vereist onderzoek. Anders gezegd, het uitvoeren van veiligheidsonderzoek is aan te merken als een verplichting voor leverancier en gebruikersorganisatie, als onderdeel van wettelijke zorgplichten in dit domein. Daarbij kunnen we twee fases onderscheiden:
1. van ontwerp tot en met levering van een ICT-product of ICT–dienst (ex ante);
2. en de periode dat het ICT-product of ICT-dienst in gebruik is / gedurende de levensduur (ex post). 

#Verplichting om beveiliging te doen
Iedere organisatie, ongeacht sector moet vandaag digitale technologie en gegevens beveiligen, want de juridische vrijblijvendheid van het treffen van beschermingsmaatregelen ligt achter ons. Voor de houder van een persoonsregistratie gold deze verplichting sinds de gefaseerde inwerkingtreding van de eerste Nederlandse privacywet, de Wet persoonsregistraties, op 1 juli 1989 van kracht werd. Sterker nog, informatiebeveiliging wordt steeds vaker in wet- en regelgeving voorgeschreven, ook door de Europese Unie. Denk aan de Richtlijn privacybescherming uit 1994, die Nederland door middel van de Wet bescherming persoonsgegevens implementeerde (inwerkingtreding op 1 september 2001). Daarnaast is er beleid en zijn organisaties gebonden aan overeenkomsten met een digitale beveiligingscomponent. 

Speciaal voor rijksoverheidsorganisaties gold sinds 1 januari 1995 het Besluit Voorschrift Informatiebeveiliging Rijksdienst (VIR 1994) en op dit moment de versie uit 2007 (VIR 2007). Voor 1995 waren er ook al beveiligingsvoorschriften voor de rijksoverheid van kracht. Hierbij gaat het om: 
1. Aanwijzingen inzake de beveiliging van persoonsgegevens, verwerkt en opgeslagen in geautomatiseerde gegevensverwerkende systemen bij de Rijksoverheid, en het  
2. Voorschrift inzake de beveiliging van gerubriceerde gegevens, verwerkt en opgeslagen in geautomatiseerde systemen bij de Rijksoverheid.

Anders gezegd, de beveiliging van computersystemen, netwerken en de informatie die ze verwerken, is al decennia een wettelijke verplichting, terwijl voor overheidsorganisaties aanvullende regulering en aanvullend beleid, zoals de Baseline Informatiebeveiliging, geldt. 

De huidige juridische normering van digitale beveiliging kent een belangrijke feitelijke reden. Van fouten en andere onvolkomenheden die digitale technologie en processen verzwakken, wordt in toenemende mate misbruik wordt gemaakt door criminele en statelijke actoren. Zo spreekt het Cyber Security Beeld Nederland (CSBN) 2021 van een acute dreiging. Verder kan zwakke digitale technologie autonoom en zonder opzet tot een digitaal incident leiden, eveneens met vaak directe gevolgen voor de bedrijfsvoering, zoals uitval.  

Om een technisch veiligheidsprobleem (‘vulnerability’ of kwetsbaarheid) te ontdekken, voert een onderzoeker een zogenoemde penetratietest of pentest uit die tot een of meer – bij voorkeur herleidbare en controleerbare - bevindingen leidt. Binnendringen in beveiligde computersystemen of een poging hiertoe vindt ook zonder opdracht en dus toestemming plaats, namelijk door misdadigers, statelijke actoren en ethische hackers die zich hiermee uit maatschappelijke betrokkenheid bezighouden. 

Of een digitaal veiligheidsonderzoek nu intern of extern wordt uitgevoerd, handmatig of geautomatiseerd, statisch of dynamisch, eenmalig, periodiek of continu (monitoring) of op basis van een combinatie hiervan, het structureel testen van de eigen organisatie geldt als cruciaal onderdeel om - de proactieve aanpak van - informatiebeveiliging te verbeteren en te versnellen. Dit geldt des te meer voor producent en leverancier van digitale producten en dienst, als startpunt.

Uit oogpunt van goed bestuur is het onvermijdelijk om mede en ten minste basale kennis te hebben van het rechtskader van ICT, inclusief informatiebeveiliging. Dit verklarend document richt zich dan ook in het bijzonder op opdrachtgevers van pentesten. Hieronder passeren een aantal belangrijke juridische aspecten van offensieve digitale veiligheidstesten, intern uitgevoerd of uitbesteed, beknopt de revue.  

Het recht vervult bij veiligheidsonderzoeken een duale rol. De rechtsregels bieden om te beginnen richtsnoeren voor het zorgvuldig uitvoeren en optimaliseren van de veiligheidsonderzoeken binnen de juridische piketpalen en daarnaast het ondersteunen bij het treffen van beveiligingsmaatregelen die verplicht zijn op grond van wet- en regelgeving en beleid; dat wil zeggen de naleving van zorgplichten en ander verplichtingen, inclusief de controle hierop en het afleggen van verantwoording. 

Wie zorgvuldig en zo optimaal als in redelijkheid mogelijk is test, verhoogt de digitale weerbaarheid van zijn organisatie. Daarmee zijn pentesten een noodzakelijk offensief veiligheidsinstrument geworden, die bijvoorbeeld mede uitgevoerd kunnen worden om te controleren of een organisatie de acht basismaatregelen die het Nationaal Cyber Security Center (NCSC) van het ministerie van Justitie en Veiligheid aanbeveelt, in voldoende mate heeft getroffen. 

 Daarbij gaat het telkens om het algemene probleem van een gebrek aan vertrouwelijkheid van gegevensverwerking het hoofd te bieden. Verplichte maatregelen moeten incidenten voorkomen of tenminste de gevolgen daarvan te beperken. Wie uitzoomt, denkt mede aan het veiligstellen van continuïteit en betrouwbaarheid van de dienstverlening en, uiteindelijk, de publieke belangen. De digitale zorgplichttrend zet zich verder door.  

In beginsel zijn de voorgeschreven beveiligingsmaatrelen open normen, dat wil zeggen een globaal geformuleerde doelstelling of resultaatsverplichting die de beoogde doelgroep ruimte biedt om zelf te bepalen op welke wijze het doel of het resultaat wordt bereikt. Met open normen biedt de wetgever een organisatie de mogelijkheid tot maatwerk, toegesneden op de omstandigheden in het concrete geval. 

Het open en risico-gebaseerde karakter van beveiligingszorgplichten voor het treffen van beveiligingsmaatregelen blijkt onder meer uit de AVG. Zo bepaalt de privacywet dat verwerkingsverantwoordelijke en verwerker ‘*passende technische en organisatorische maatregelen*’ moeten nemen ‘*om een op het risico afgestemd beveiligingsniveau te waarborgen*’ (Art. 32, lid 1 AVG). Nader bezien bevat de Europese privacywetgeving een reeks veiligheidszorgplichten, inclusief privacy-by-design and security-by-design (art. 25 AVG), terwijl bijvoorbeeld voor de zorgsector aanvullend de norm NEN 7510 verplicht gesteld is. Ondertussen heeft de Inspectie Zorg en Jeugd (IGJ) van het ministerie van VWS ziekenhuizen een deadline gesteld: voor 31 december 2023 moet er aan deze beveiligingsnorm worden voldaan. 

Verder hebben we te maken met de Europese Cybersecurity Act (CSA) die onder andere over de vrijwillige certificering voor ICT-producten, -diensten en -processen gaat (Verordening (EU) 2019/880). Daarnaast is een wetgevingsproces in gang gezet voor een Cyber Resiliance Act (CRA), een verordening gericht op het instellen van gemeenschappelijke cybersecurity-normen voor verbonden apparaten. 

Uit Brussel komt verder de Richtlijn netwerk- en informatiebeveiliging (EU-Richtlijn 2016/1148), welke regeling opgezet is in onze Wet beveiliging netwerk- en informatiesystemen (Wbni) en het bijhorende besluit (Bbni). Aanbieders van essentiële diensten en digitale dienstverleners zijn verplicht tot het treffen van beveiligingsmaatregelen, die passend zijn bij de beveiligingsdoelstellingen van de Wbni. Hiervoor en voor andere controles heeft het Agentschap Telecom op 1 juli 2022 een zelftest beschikbaar gesteld. De beide regelingen worden nu herzien en uitgebreid.  

Zo stuurde Minister Yeşilgöz-Zegerius (JenV) op 20 april 2022 de Koning het nader rapport over het wetsvoorstel Wijziging van de Wbni. Dit voorstel betrof de inmiddels in werking getreden uitbreiding van de bevoegdheid van deze minister om informatie te verstrekken over de netwerk- en informatiesystemen van niet-vitale aanbieders. Het gaat dan om dreigings- en incidentinformatie. Aanzienlijk meer ingrijpend wordt de aanpassing van de Wbni als gevolg van de implementatie van Richtlijn bescherming netwerk- en informatiesystemen 2 (NIS2 - (EU) 2022/2555) van 24 december 2022. De richtlijn zal op 18 oktober 2024 van toepassing worden. 

Op grond van weer een andere Europese wet zijn verkopers sinds 27 april 2022 wettelijk verplicht om digitale apparaten en diensten werkend en veilig te houden door het leveren van software- en beveiligingsupdates. Hetzelfde geldt bij de aanschaf van bijvoorbeeld games of apps en voor streamingdiensten. 

Kortom diverse regelgeving maken het testen van omgevingen en producten noodzakelijk. We ontkomen er dan ook niet aan deugdelijk onderzoek te plegen.  

 ## Juridische punten die helpen bij het onderzoek 
 ### Contractvoorwaarde 
 In toenemende mate worden digitale veiligheidstesten en andere onderzoeken, inclusief risico-inschattingen, zoals een DPIA, opgenomen in contracten, bijvoorbeeld voorafgaand aan (op)levering van een applicatie of digitale dienst of voorafgaand aan samenwerking, al dan niet in een keten. Dit geldt eveneens voor een pentest. De belangstelling voor deze juridische route, laat zich verklaren door de toenemende aandacht voor informatiebeveiliging en de zoektocht naar meer kwaliteitswaarborgen en zekerheden in het domein, mede in het licht van de controle van een beveiligingsverantwoordelijkheid. 

Opname in een contract strekt tot voordeel van beide partijen: de uitkomsten van digitaal beveiligingsonderzoek geven inzicht in aspecten van de status van digitale veiligheid in het concrete geval, op een bepaald moment en kunnen discussies en conflicten voorkomen. Daarbij kunnen DPIA code review, security assessment, de penetratietest of een informatiebeveiligingsonderzoek met auditwaarde elkaar aanvullen. Voor de goede orde: een dergelijke clausule leidt tot een afzonderlijke overeenkomst tussen opdrachtgever en pentester: de pentestovereenkomst.

### De onderzoeksovereenkomst
De hoofdregel staat buiten kijf. In beginsel geen technisch onderzoek op systemen uitvoeren zonder toestemming van een bevoegde vertegenwoordiger van de eigenaar of bestuurder van de organisatie die de te onderzoeken ICT in gebruik heeft. Ontbreekt deze toestemming dan kan alleen al de handeling scannen van netwerk- en informatiesystemen onder het delict computervredebreuk (art. 138ab WvS) vallen (zie #15). De toestemming is nauw verbonden met de scope van het veiligheidsonderzoek, vastgelegd in een overeenkomst. 

Naast toestemming verleent de opdrachtgever als regel diverse vrijwaringen aan de pentester. Bij uitbesteding kwalificeren de afspraken met een externe veiligheidsdienstverlener als een overeenkomst tot opdracht (art. 7:400 BW). Op basis van een in het contract opgenomen vrijwaringsbeding wordt iets of iemand gevrijwaard. In deze context verkrijgt de pentester bescherming tegen een vordering, zoals een claim tot betalen van door de test ontstane schade, die een derde (of de opdrachtgever) bij hem neerlegt. In geval van claims van derden, neemt de opdrachtgever deze over en blijft de onderzoeker buiten schot. 

Wanneer een contractspartij zijn eigen aansprakelijkheid beperkt of uitsluit noemen we dat exoneratie. Aan het gebruik van een vrijwaringsbeding en exoneratiebeding in algemene voorwaarden stelt het Burgerlijk Wetboek kaders. 

Dat laat onverlet dat een – offensieve - digitale veiligheidstest altijd zorgvuldig moet worden uitgevoerd. ‘De opdrachtnemer zal bij de uitvoering van zijn werkzaamheden de zorg van een goed opdrachtnemer in acht moeten nemen’, aldus art. 401 BW. Daarbij gaat het om handelen conform objectieve kwaliteitseisen die aan een redelijk bekwaam en redelijk handelend pentester in het concrete geval mag worden gesteld. Dit betreft een open, minimumnorm. Er wordt getoetst aan het niveau van een gemiddeld vakgenoot, tenzij anders blijkt. Je kunt onder meer zeggen dat de pentester zijn opdrachtgever niet onnodig mag blootstellen aan voorzienbare en vermijdbare risico’s. Ook bestaat de mogelijk dat een pentester zijn opdrachtgever vrijwaart tegen claims van derden, indien hij bijvoorbeeld buiten de afgesproken scope handelde of – anderszins - grove schuld heeft bij een incident. Dan handelt de pentester de claims van derden af. 

Nota bene. Zowel het element toestemming als vrijwaring kan mede afhankelijk zijn van de gebruikte tooling bij het uitvoeren van een pentest, dat wil zeggen de digitale (technische) hulpmiddelen zoals scanning software. Uit theorie en praktijk blijkt dat de scope (reikwijdte) van een digitaal veiligheidsonderzoek veelal pas wordt ontdekt c.q. vastgesteld tijdens de uitvoering van scans.  

Dat betekent dat toestemming gegeven en vrijwaren voor de inzet soms dan wel eerder een iteratief proces is dan een eenmalige, voorafgaande handeling op basis van vaststaande gegevens. Goed beschouwd vraagt dit proces van herhaling om continue aandacht van een beslissingsbevoegde medewerker of manager van de geteste organisatie (opdrachtgever); iemand die deze verantwoordelijk formeel heeft en de toestemming mag geven om een object op een bepaald niveau te scannen. 

### Verwerkersovereenkomst
Bij uitbesteding van een digitaal veiligheidsonderzoek – dus het geven van een opdracht aan een externe dienstverlener - is veelal onvermijdelijk om met de externe pentester, naast de overeenkomt van opdracht, een verwerkersovereenkomst in de zin van de AVG te sluiten. Dat heeft te maken met een onzeker vooral, namelijk indien de onderzoeker bij de uitvoering van de test onverhoopt toegang tot persoonsgegevens verkrijgt die de opdrachtgever verwerkt.  

Goed om te beseffen, de privacywetgeving hanteert een breed verwerkingsbegrip:  

> ‘een bewerking of een geheel van bewerkingen met betrekking tot persoonsgegevens of een geheel van persoonsgegevens, al dan niet uitgevoerd via geautomatiseerde procedés, zoals het verzamelen, vastleggen, ordenen, structureren, opslaan, bijwerken of wijzigen, opvragen, raadplegen, gebruiken, verstrekken door middel van doorzending, verspreiden of op andere wijze ter beschikking stellen, aligneren of combineren, afschermen, wissen of vernietigen van gegevens’ (art. 4, lid 2 AVG).  

Anders gezegd, zo ongeveer alles wat je met een persoonsgegeven kan doen, valt hieronder. Bij uitbesteding blijft de opdrachtgever (van een beveiligingsonderzoek en meer) te allen tijde zelf verantwoordelijk voor de persoonsgegevens die hij verwerkt. De privacywet verplicht bij uitbesteding van de verwerking van persoonsgegevens het sluiten van een verwerkersovereenkomst. Daarbij geldt in dit kader de opdrachtgever als gegevensverantwoordelijke en de onderzoeker als verwerker (art. 28 AVG). 

Zonder verwerkersovereenkomst ontbreekt een verwerkingsgrond voor de pentester en kan hij in voorkomende gevallen de wet schenden. Op grond van de verwerkersovereenkomst verkrijgt de pentester toestemming om persoonsgegevens te downloaden, aangevuld met de verplichting om de gegevens vervolgens naar keuze van de opdrachtgever onomkeerbaar te vernietigen of desgewenst terug te geven. 

### Auteursrechtelijke invalshoek 
Op digitale technologie rusten doorgaans intellectuele eigendomsrechten. Daarbij spelen computerprogramma’s in soorten en maten en het hierop geldende auteursrecht een overheersende rol, in de zin dat gebruikersorganisaties hiermee intensief worden geconfronteerd. Verreweg de meeste software die een organisatie heeft draaien is in licentie gegeven door een ander, zoals de rechthebbende producent. De rechtsverhouding tussen partijen wordt bepaald door de licentieovereenkomst, andere afspraken, zoals vastgelegd in een onderhoudsovereenkomst, en het wettelijke auteursrecht, dat tevens aanvullende en afwijkende regels kent voor software (hoofdstuk VI, artt. 45h-45n Auteurswet).  

Het uitvoeren van een onderzoek op computercode waarop een ander de eigendomsrechten (het auteursrecht) heeft, leidt tot de vraag of dit een wellicht handeling betreft waarvoor toestemming van de auteursrechthebbende vereist is, omdat de intellectuele eigendomswetgeving de maker sterke beschermingsrechten verleent. Die kan als heer en meester exclusief over zijn een eigen werk beschikken. 

Het auteursrecht betreft het uitsluitend recht van de maker of van diens rechtverkrijgenden, om de code openbaar te maken en te verveelvoudigen, behoudens de beperkingen, bij de wet gesteld (art. 1 Aw). Dat is voor computercode niet anders.  

De wet benoemt en regelt het testen van een computerprogramma. De rechtmatige gebruiker mag de software van de softwareproducent testen, echter deze handelingen moeten zich beperken tot de ‘daaraan ten grondslag liggen ideeën en beginsel te achterhalen’ (art. 5, lid 3 Softwarerichtlijn, omgezet in art. 45l Aw). Daaronder valt een onderzoek naar veiligheidsgebreken niet.  

Maar omdat er bij een beveiligingsonderzoek en in het bijzonder het scannen van de software in beginsel geen nieuwe openbaarmaking of verveelvoudiging plaatsvindt, zijn de handelingen (het zonder toestemming van de softwarefabrikant testen van de software uit oogpunt van digitale veiligheid) auteursrechtelijk toegestaan. 

### Wettelijk recht op foutherstel 
Een onderzoek kan kwetsbaarheden blootleggen, waarbij de bevindingen vervolgens om actie vragen om de veiligheid van digitale technologie en processen te verbeteren. Een van de stappen is het verhelpen van softwarefout. In beginsel is de softwareproducent naar Nederlands contractenrecht verplicht om gebreken in een computerprogramma te verhelpen indien de computercode niet voldoet aan de vastgelegde specificaties, daaronder vallen dus ook veiligheidsgebreken.  

De praktijk toont vaak een ander beeld. Via licentievoorwaarden en algemene voorwaarden proberen softwarefabrikanten hun rol af te zwakken, bijvoorbeeld door de clausule op te nemen dat het geleverde computerprogramma niet foutloos is en niet zonder onderbreking kan werken. En het NCSC hanteert in de Leidraad Coordinated Vulnerability Disclosure (2018) een 60-dagen periode voor het verhelpen van de kwetsbaarheid door de fabrikant. 

> ‘Met een CVD-beleid wordt geprobeerd een balans te vinden tussen het belang om kwetsbaarheden zo snel mogelijk bekend te maken, zodat men maatregelen kan treffen, en het belang van ontwikkelaars en leveranciers om voldoende tijd te hebben de kwetsbaarheid te verhelpen. Het NCSC hanteert voor dit proces een standaardtermijn van 60 dagen tussen melding en publieke bekendmaking. Er kunnen echter omstandigheden zijn waardoor besloten wordt deze termijn te verlengen of in te korten.’ 

Gebruikers daarentegen hebben ook rechten. In het kader van de verbetering van digitale veiligheid, is het onderbelichte Europese recht op foutherstel door de gebruiker / licentienemer vermeldingswaard. Iedere rechtmatige gebruiker beschikt namelijk over het onvervreemdbare, wettelijk verankerde recht een computerprogramma te verveelvoudigen in het kader van het laden, het in beeld brengen of het verbeteren van fouten (art. 5, lid 1 Softwarerichtlijn, omgezet art. 45j AW).  

Hierbij past de kanttekening dat licentienemers doorgaans niet over de broncode van het computerprogramma beschikken, tenzij het bijvoorbeeld open source software betreft. Zonder de software in broncodetaal, wordt foutherstel heel erg moeilijk. Wie over de broncode wil beschikken, moet de machinetaal (nullen en enen) decompileren. De computer-leesbare vorm wordt hiermee omgezet naar een voor de mens leesbare en te wijzigen vorm.  Dit proces heet ‘*reverse engineering*’. 

Echter deze handeling is volgens de wet voor een rechtmatige gebruiker uitsluitend toegestaan voor het maken van interoperabele programmatuur (art. 6 Softwarerichtlijn, omgezet in art. 45m Aw). Anders gezegd, het wettelijke recht op decompilatie van de runcode geldt dus niet voor testdoeleinden (voor de volledigheid: kan wel worden verleend in de licentieovereenkomst) of het herstellen van een veiligheidsfout. Over dat laatstgenoemde verbod denkt de Europese rechter sinds kort anders over.  

Het gaat om - ook in het licht van beveiligingsonderzoek – een belangrijk arrest. Iedere rechtmatige gebruiker van een computerprogramma heeft op grond van de wet volgens de Europese rechter tevens het recht de software te ‘*decompileren teneinde fouten te verbeteren die de werking ervan beïnvloeden, ook wanneer de verbetering erin bestaat een functie te deactiveren die de goede werking verstoort van de toepassing waarvan het programma deel uitmaakt*’. De enige beperking die de rechter aan deze regel stelt, is dat de licentienemer een dergelijke decompilatie slechts mag ‘*verrichten voor zover dit noodzakelijk is voor die verbetering en, in voorkomend geval, met inachtneming van de voorwaarden die bij overeenkomst met de auteursrechthebbende van dit programma zijn vastgelegd.*’ 

### Strafrecht: computervredebreuk 
Een offensieve veiligheidstest die wordt uitgevoerd zonder toestemming van de organisatie die voorwerp van onderzoek is, kan leiden tot een digitale inbraak (‘*hack*’), die de penter pleegt. Laten we beginnen de vraag naar de rechtmatigheid van het bezit van digitale tools in een computersysteem in te breken. Ons Wetboek van Strafrecht stelt strafbaar het vervaardigen, verkopen, verwerven, invoeren, verspreiden of anderszins ter beschikking stellen of voorhanden hebben van een ‘een technisch hulpmiddel dat hoofdzakelijk geschikt is gemaakt of ontworpen is tot het plegen van computervredebreuk (art. 139d lid 2 WvS).   

Een tool die de pentester gebruikt bij zijn onderzoek, kan in beginsel onder een dergelijke ‘*technisch hulpmiddel*’ vallen, maar dan moet er aan twee criteria zijn voldaan. De tool 
1. moet ‘*hoofdzakelijk*’ zijn gemaakt of ontworpen om te hacken en
2. moet gemaakt zijn, in bezit zijn en meer, met het oogmerk om te hacken. De criteria bieden zowel de organisatie die intern penetratietest of ander technisch beveiligingsonderzoek uitvoeren als een professionele dienstverlener die in opdracht test, in de regel voldoende ruimte om tools bij offensieve veiligheidstesten rechtmatig in te zitten. Vooral het ontbreken van een wederrechtelijk oogmerk is effectief. 

Bij delict computervredebreuk (art. 138ab WvS) gaat het om ‘*het opzettelijk wederrechtelijk binnendringen in een geautomatiseerd werk voor de opslag of verwerking van gegevens, of in een deel daarvan*’, dat strafbaar is gesteld als computervredebreuk. Als voorwaarde geldt dat de degene:  
> a. daarbij enige beveiliging doorbreekt of  
> b. de toegang verwerft door een technische ingreep, met behulp van valse signalen of een valse sleutel dan wel door het aannemen van een valse hoedanigheid.’ 

In de praktijk zien we dat rechters met de vraag te maken krijgen of en zo ja wanneer het scannen van een geautomatiseerd werk een voltooid binnendringen oplevert dan wel dat de handeling niet verder komt tot een strafbare poging of zelfs helemaal geen strafbare gedraging betreft. Om een idee te hebben van wat hier kan spelen, wijzen we op de de kern van een arrest van de Hoge Raad van 9 april 2019:

> ‘De enkele omstandigheid dat de verdachte blijkens bewijsmiddel 3 op 12 september 2012 met behulp van een scan-programma de website van de aangever op kwetsbaarheden heeft onderzocht, waarvan een aantal werd geblokkeerd en dat als gevolg daarvan 'niet ondenkbaar is dat er een geslaagde aanval heeft plaatsgevonden' volstaat daartoe niet’
> ‘De vermelding in bewijsmiddel 3 van aanvallen door middel van "cross site scripting" en "directory traversal" waarvan de werking niet nader is toegelicht maakt dat niet anders, in aanmerking genomen dat aldus zonder nadere motivering die ontbreekt in het midden blijft of de verdachte toegang heeft verworven door een technische ingreep of dat het bij een poging daartoe is gebleven.’ 

Voor de volledigheid, sinds de inwerkingtreding van de Wet Computercriminaliteit III op 1 maart 2019 heeft de politie de bevoegdheid om heimelijk een geautomatiseerd werk van een verdachte binnen te dringen (art. 126nba Sv), zoals een laptop of een smartphone. Ook bij deze wettelijke hackbevoegdheid gaat het om een offensief middel, die bovendien aan strikte voorwaarden is verbonden en alleen mag worden ingezet bij verdenking van een ernstig strafbaar feit. 

Coordinated Vulnerability Disclosure 

Uit het bovenstaande volgt dat een ethisch hacker die uit zichzelf, dus zonder opdracht, onderzoek uitvoert naar kwetsbaarheden in ICT-systemen van derden strafrechtelijk in de problemen kan komen. Mede uit oogpunt van algemeen belang vraagt deze omstandigheid om bescherming van personen die te goeder trouw handelen. Daarom hebben een beperkt aantal landen een regeling ingesteld omtrent het melden van een digitaal veiligheidsprobleem dat op deze wijze is ontdekt. In Nederland is inmiddels vigerend de Leidraad Coordinated Vulnerability Disclosure (2018) van het NCSC. 

Het Openbaar Ministerie vindt het naar eigen zeggen belangrijk dat ethische hackers kwetsbaarheden kunnen blijven zoeken en melden zodat ICT-systemen veiliger kunnen worden gemaakt. Daarom stimuleert het OM organisaties beleid over vast te stellen voor het melden van kwetsbaarheden in hun ICT-systemen. Een dergelijke ‘*Coordinated Vulnerability Disclosure*’ of CVD-regeling bindt zowel de organisaties als de melder. Onderzoekers krijgen van het OM het advies om hun stappen in een logbestand bij te houden om te kunnen aantonen dat ze zich aan de regels houden. 

Met een CVD-beleid wordt geprobeerd een balans te vinden tussen het belang om kwetsbaarheden zo snel mogelijk bekend te maken, zodat men maatregelen kan treffen, en het belang van ontwikkelaars en leveranciers om voldoende tijd te hebben de kwetsbaarheid te verhelpen.  

Nederland hanteert een duaal beleid dat zich als volgt laat schetsten. Wie een technische kwetsbaarheid vindt in een systeem van de Rijksoverheid, kan dit melden het NCSC. Gaat het om een kwetsbaarheid in digitale technologie van een andere entiteit, dan moet de ontdekker eerst de eigenaar van het systeem of de productleverancier benaderen. Pas als deze organisatie niet of niet goed reageert, kan er bij het NCSC worden gemeld, die vervolgens als intermediair de kwetsbaarheid bij de desbetreffende organisatie informeert.  

Daarbij past een kanttekening. Het formele CVD-beleid van OM en NCSC staat of valt met een toepasselijke CVD-regeling per organisatie. Voor alle rijksoverheidsorganisaties is deze beschikbaar, zelfs uniform. Organisaties die nog geen CVD-regeling hebben gemaakt en gepubliceerd, doen er goed aan dit aspect van digitaal beveiligingsbeleid alsnog op te pakken. Bij gebreke daarvan, vallen betrokkenen (pentester, onderzochte organisatie en OM) terug op de algemene beleids- en rechtsregels, omdat er niet voldaan is aan de vereisten van ‘*ethisch hacken*’. 

Een tweede opmerking ziet op een aanpalende geheimhoudingskwestie, namelijk de verplichting ter zake die vaak in arbeidsovereenkomsten is opgenomen. Indien werknemers op verzoek van het management hun eigen organisatie onderzoeken en de tot actie nopende bevindingen niet tot tot verbeteringen van de digitale veiligheid leidt, kan een werknemer uiteindelijk door openbaarmaking van de testresultaten een klokkenluider worden. Het Nederlandse recht kent sinds 1 juli 2016 een wettelijke klokkenluidersregeling (Wet huis voor klokkenluiders), die nu wordt herzien op grond van het Europese recht.  

Tot slot, echter zeker niet als laatste: het CVD-beleid van een organisatie vrijwaart een ethisch hacker in beginsel niet van civielrechtelijke aansprakelijkheid. 

### Juridische ontwikkelingen kwetsbaarheden 
Er zijn tientallen technische definities van het begrip '*kwetsbaarheid*' in relatie tot computersystemen, ICT en geautomatiseerde gegevensverwerking in omloop. Deze definities variëren in meer of mindere mate, zelfs binnen één organisatie, zoals het internationaal gezaghebbende National Institute of Standards and Technology (NIST), dat deel uitmaakt van het Amerikaanse ministerie van Handel. In de meeste definities wordt echter verwezen naar een 'flaw' of 'weakness' (fout, zwakte) in het ontwerp, de implementatie, de werking, het beheer of de '*controls*' van systemen of '*assets*'. 

Naast de basisdefinitie blijkt in de praktijk dat er onderscheid wordt gemaakt tussen een '*gewone*' kwetsbaarheid en een kritieke variant. Bovendien worden kwetsbaarheden vaak ingedeeld in 'bekende' en 'zero-day' kwetsbaarheden. De laatstgenoemde categorie kwetsbaarheden wordt ontdekt door derden, waaronder ethische hackers, criminelen of statelijke actoren. De softwareproducent heeft hier geen weet van en krijgt geen tijd ('zero time') om de zwakheid te herstellen voordat er misbruik van wordt gemaakt. 

Het is ook opmerkelijk dat kwetsbaarheden niet altijd uitsluitend met de veiligheid van digitale technologie worden geassocieerd. Gezien de definitie van digitale beveiliging (zie hierboven), valt hier ook het aspect van continuïteit van bedrijfsprocessen en de organisatie onder. Bovendien koppelen veel standaardisatieorganisaties de zwakheid aan de omstandigheid dat er misbruik van kan worden gemaakt. Met andere woorden, als een veiligheidsgebrek niet kan worden aangevallen (meestal met speciaal geschreven software of '*exploit*'), wordt het niet als een kwetsbaarheid beschouwd. 

Sommigen, zoals het NIST (in SP 800-30) en het Europese agentschap ENISA, zien dit echter breder en beschouwen een kwetsbaarheid als een technische zwakheid die in de praktijk tot een veiligheidsprobleem kan leiden, zowel per ongeluk als door opzettelijk misbruik. Deze benadering verdient steun omdat elk digitaal gebrek met een veiligheidsrisico in beginsel actie vereist, ongeacht de intentie (en het is belangrijk op te merken dat fouten juridisch gezien in beginsel reproduceerbaar moeten zijn). 

Op deze lijn zit ook de Europese wetgever. Richtlijn beveiliging netwerk en informatiesystemen (EU/2022/2555, NIS2) definieert ‘*kwetsbaarheid*’ als volgt:  
> ‘een zwakheid, vatbaarheid of gebrek van ICT-producten of ICT-diensten die door een cyberdreiging kan worden uitgebuit’ (art. 6 onder 15 NIS2).  

Onder een ‘*cyberbedreiging*’ moet vervolgens worden Verorderning ENISA en certficering verstaan:  
>‘elke potentiële omstandigheid, gebeurtenis of actie die netwerk- en informatiesystemen, de gebruikers van dergelijke systemen en andere personen kan schaden, verstoren of op andere wijze negatief kan beïnvloeden (art. 2, lid 8 Verordening EU/2019/881). 

Beiden betreffen ruime definities. Belangrijk is verder het ontwerp voor een Europese Cybersecurity Resilence Act (CRA) van 15 september 2022. Hierbij gaat het om veiligheidsmaatregelen voor een ‘*product with digital elements*’, dat wil zeggen ‘*any software or hardware product and its remote data processing solutions, including software or hardware components to be placed on the market separately*’.  

De producten met digitale elementen 
> (i) moeten volgens veiligheidseisen worden ontworpen, ontwikkeld en geproduceerd zodat ze een geschikt cybersecurityniveau waarborgen op basis van de risico’s en
> (ii) moeten worden geleverd zonder bekende kwetsbaarheden waarvan misbruik kan worden gemaakt. Daarbij is uitvoerig testen onvermijdelijk. De conceptverordening onderscheidt in drie productcategorieën met digitale elementen, gerelateerd aan de kritieke status van de toepassing: gewoon, kritiek en hoog-kritiek. 

Zoals gezegd, hanteert het NCSC voor het verhelpen van de kwetsbaarheid een standaardtermijn van 60 dagen tussen CVD-melding en publieke bekendmaking. Meestal gaat het om het schrijven en leveren van een ‘security patch’, nieuwe computercode die de gebrekkige vervangt. Er kunnen echter omstandigheden zijn waardoor besloten wordt deze termijn te verlengen of in te korten. Vervolgens, nadat een herstelcode beschikbaar is gesteld, doen gebruikersorganisaties er doorgaans goed aan deze snel te implementeren.  

Nog een juridische ontwikkeling, maar dan in het consumentenrecht. Om het goede en veilige gebruik te garanderen, zijn aanbieders van een digitaal product of dienst op grond van Richtlijn levering digitale inhoud (EU/2019/770) en de Richtlijn verkoop goederen (EU/ 2019/771) verplicht om software-updates te leveren, daaronder nadrukkelijk begrepen veiligheidsupdates. 

In 2017 wilde toenmalig minister Grapperhaus (Justitie en Veiligheid) digitaal onveilige bedrijven - die verzuimden een security patch voortvarend te installeren – aanpakken, maar dit plan leidde niet tot nieuwe regulering. Twee jaar later overwoog dezelfde minister opnieuw in de markt in te grijpen, nu omdat vitale aanbieders beveiligingsadviezen kennelijk onvoldoende opvolgen. ‘Waar nodig zal gebruik worden gemaakt van de interventiemogelijkheden onder de Wbni als dat nodig is in het kader van nationale veiligheid.  

Het NCSC zal bijvoorbeeld vaker toezichthouders informeren over situaties waarin een vitale aanbieder beveiligingsadviezen onvoldoende opvolgt waardoor risico’s voor de nationale veiligheid blijven bestaan. De VPN-Pulse kwetsbaarheid laat zien dat waarschuwingen en adviezen van het NCSC niet altijd direct worden opgevolgd.  

In het Cyber Security Beeld Nederland (CSBN) 2022 wordt onder andere ‘een toename van het aantal ‘*zero-day kwetsbaarheden*’ geconstateerd. Dat zijn zwakke plekken in software die nog onbekend zijn bij de producent. In 2019 diende D66 een initiatiefwetsvoorstel in. Deze Wet Zeroday’s draagt bestuursorganen op die gebruik maken van onbekende kwetsbaarheden tot het inrichten van een aanvullend afwegingskader voor de bekendmaking van onbekende kwetsbaarheden. Het vorige kabinet constateerde op 9 februari 2021 dat wetsvoorstel een negatief effect op de operationele processen heeft en vergroot daarnaast de administratieve lasten.  

De aansprakelijkheidskwestie in relatie tot een kwetsbaarheid begint met de vraag wie waarvoor verantwoordelijk is. Hierover bestaat in Nederland vandaag in zoverre overeenstemming, dat volgens minister Yesilgöz (Justitie en Veiligheid) organisaties in de eerste plaats zelf verantwoordelijk voor hun eigen cybersecurity zijn, terwijl voor softwarefabrikanten geldt dat zij primair verantwoordelijk zijn voor de digitale veiligheid van de door hen aangeboden producten en diensten. Dat is in lijn met opvattingen van anderen, zoals de Onderzoeksraad voor Veiligheid (OVV) waarop de Kamervragen betrekking hebben. 

Fouten in software, inclusief veiligheidsgebreken, kunnen tot aansprakelijkheid voor schade leiden die hieruit ontstaat, zowel op grond van het leerstuk van de onrechtmatige daad als wanprestatie bij de uitvoering van een overeenkomst. In beide gevallen dient de kwetsbaarheid aan iemand te worden toegerekend. Rechtspraak over kwetsbaarheden naar Nederlands recht ontbreekt vrijwel, hetgeen in schril contrast staat met de hoeveelheid kwetsbaarheden die aan het licht komen en het juridische net in de vorm van beveiligingsverplichtingen, dat telkens wettelijk wordt aangetrokken.  

Om softwareproducenten te stimuleren meer aan digitale veiligheid te doen, wilde het kabinet Rutte III wilde een bijzondere juridische aansprakelijkheid voor onveilige software in het Nederlandse recht introduceren. Dit beleidsvoornemen, vastgelegd in het regeerakkoord van 10 oktober 2017, werd niet uitgevoerd. Daarentegen benadrukt de huidige minister van Justitie het belang om op internationaal en Europees niveau kwaliteits- en aansprakelijkheidsafspraken te maken over digitale veiligheid ‘vanwege het grensoverschrijdende karakter van de markt voor ICT-producten en –diensten’, eveneens in overeenstemming met de OVV.  

De verwachting is dat de Europese Commissie met voorstellen zal komen om de verantwoordelijkheid van fabrikanten voor veilige software wettelijk vast te leggen en hun aansprakelijkheid voor de gevolgen van kwetsbaarheden te definiëren. Ondertussen wordt internationaal sinds 1999 gewerkt met de Common Vulnerabilities and Exposures (CVE)-lijst, waarmee kwetsbaarheden een uniek nummer krijgen om het volgen, uitwisselen van informatie en beoordelen van beveiligingsproducten te vergemakkelijken en te verbeteren. 

### Afsluitende opmerkingen 
Digitale kwaliteitstekortkomingen, waaronder kwetsbaarheden (gedefinieerd als 'zwakke plekken, vatbaarheden of gebreken in ICT-producten of -diensten die kunnen worden misbruikt door cyberdreigingen'), maken individuele gebruikers, organisaties en de samenleving als geheel kwetsbaarder dan noodzakelijk. Dit vergemakkelijkt vaak de uitvoering van digitale criminaliteit op grote schaal. 

Volgens geldende juridische opvattingen zijn organisaties in de eerste plaats zelf verantwoordelijk voor hun eigen digitale veiligheid. Aan de andere kant zijn softwarefabrikanten primair verantwoordelijk voor de digitale veiligheid van de producten en diensten die ze aanbieden. Iedere entiteit, ongeacht sector en omvang, heeft dus de wettelijke verplichting om digitale technologie en processen te beschermen door passende maatregelen te nemen. 

Degene die verplicht is beschermingsmaatregelen te nemen, moet ook controleren en verantwoording afleggen of deze maatregelen zijn geïmplementeerd, worden nageleefd en blijven voldoen aan de geldende normen. Bovendien vereist het controleren van beveiligingsincidenten aandacht en actie, omdat een dergelijk incident verplichtingen met zich meebrengt om schade bij derden te voorkomen of te beperken, en in sommige gevallen is er een wettelijke meldplicht van kracht. 

Bij de controle van digitale veiligheid vormt het structureel uitvoeren van offensieve tests van de eigen organisatie een cruciaal onderdeel om de proactieve aanpak van informatiebeveiliging te verbeteren en te versnellen. Ook binnen het kader van risicomanagement, waarbij het essentieel is om digitale veiligheidsrisico's te identificeren en hiermee om te gaan, kunnen pentests hun waarde bewijzen. 

Op basis van feitelijke gronden zijn pentests in verschillende vormen en mate onvermijdelijke controle-instrumenten en dienen ze integraal deel uit te maken van de digitale veiligheidsmaatregelen. Juridisch gezien is dit niet anders. Zowel geconsolideerde informatiebeveiligingsvoorschriften als beveiligingsnormen impliceren op zijn minst de verplichting tot pentesten. Deze verplichtingen beginnen met preventieve onderzoeken tijdens de ontwikkeling van nieuwe systemen en vóór de ingebruikname van nieuwe applicaties, om kwetsbaarheden in de software te ontdekken die kunnen leiden tot ongewenste incidenten, variërend van systeemuitval tot ransomware-besmettingen. 

Ondertussen scherpt de Nederlandse en Europese wetgeving het beveiligingsrecht voortdurend aan. Zo legt de verordening DORA expliciet de verplichting op voor dreigingsgestuurde penetratietests. 

Ongeacht een impliciet of expliciet wettelijk voorschrift, is een pentest een van de weinige effectieve instrumenten om veiligheidsonderzoeken uit te voeren en tegelijkertijd verantwoording af te leggen over digitale beveiliging. Het is daarbij onvermijdelijk om op zijn minst basiskennis van de verschillende juridische aspecten te hebben. 

Geen enkele organisatie ontkomt aan het uitvoeren van offensieve veiligheidsonderzoeken van zijn computersystemen en bedrijfsprocessen, en dit geldt onverkort voor het toepasselijke rechtskader. Bovendien schrijft komende wetgeving (NIS2 in de vorm van de Wet digitale veiligheid) voor dat ook de toeleveranciers van organisaties onder de reikwijdte vallen. 

Pentesting wordt algemeen beschouwd als een onvermijdelijke maatregel: 
1. die feitelijk noodzakelijk is om kwetsbaarheden in computersystemen en netwerkwerken te ontdekken; 
2. die juridisch noodzakelijk om te kunnen voldoen aan algemeen-wettelijke voorschriften (‘*legal compliance*’), sectorale voorschriften (‘*regulatory compliance*’) en in voorkomende gevallen tevens aan contractuele afspraken (‘*contractual compliance*’). 

Een zorgvuldige juridische uitvoering van het onderzoek beperkt tevens de kans op schade en aansprakelijkheid (risicobeperking). Bovendien is juridische expertise vereist om binnen de geldende wettelijke kaders optimaal te kunnen testen en op basis van de bevindingen, analyses en aanbevelingen de digitale weerbaarheid van een organisatie te vergroten (waardecreatie). 
