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
