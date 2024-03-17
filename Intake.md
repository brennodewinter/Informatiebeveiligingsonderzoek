## Het intake proces
Het intakeproces voor een beveiligingsonderzoek is een fase waarin de vereisten, doelstellingen en verwachtingen van een opdrachtgever worden vastgesteld en waarin de scope en aanpak van het onderzoek worden bepaald. 

#### Non-disclosure agreement (NDA)
Voorafgaan aan een een intake voor een informatiebeveiligingsonderzoek, is het noodzakelijk een non-disclosure agreement (NDA) te hebben tussen de partijen welke meewerken aan dit onderzoek.
Een NDA is een juridisch bindend document dat de vertrouwelijkheid van informatie regelt tussen twee of meer partijen. Zonder NDA dient er geen intake te worden uitgevoerd.

Zodra een NDA is opgesteld en ondertekend is door alle relevante partijen, kunnen de beveiligingsonderzoekers de nodige specifieke informatie verzamelen om het onderzeok te plannen en uit te voeren zoals hieronder wordt beschreven.

#### Doelstellingen en scope 
Dit omvat de specifieke doelstellingen van het beveiligingsonderzoek, zoals het testen van specifieke applicaties, netwerken of systemen. Identificeer de systemen, applicaties en technologieën welke dienen te worden getest en
omvat zowel interne als externe systemen.

#### Benaderingen beveilingsonderzoek
De benaderingen beschrijven het niveau van voorkennis en informatie welke de onderzoeker heeft over het te onderzoken systeem, applicatie of omgeving. 

- ##### Whitebox
  Bij deze benadering heeft de onderzoeker volledige kennis van het interne systeem of de applicatie welke onderzocht wordt. Dit kan onder meer toegang omvatten tot broncode, architectuurdocumentatie en inloggegevens voor interne systemen. Met deze volledige transparantie kan de onderzoeker diepgaande analyses uitvoeren en specifieke kwetsbaarheden identificeren.

- ##### Graybox
  Bij deze benadering heeft de onderzoeker gedeeltelijke kennis van een systeem of een applicatie, maar niet alle details zijn beschikbaar. Er is beperkte informatie beschikbaar over de interne werking van een systeem of applicatie.

- ##### Blackbox
  Bij deze benadering is geen voorkennis van een systeem of applicatie en het onderzoek vindt plaats zonder toegang tot interne details of broncode.

Op basis van de bevindingen die voortkomen uit een beveiligingsonderzoek met een whitebox benadering, kan worden vastgesteld welke van deze bevindingen ook zouden worden geconstateerd wanneer er een andere benaderingen zou zijn toegepast.

#### Data classificatie
Dataclassificatie is het proces waarbij gegevens worden geëvalueerd en gecategoriseerd op basis van hun gevoeligheid, waarde en het risico dat ermee gepaard gaat bij ongeoorloofde toegang, openbaarmaking of verlies.
Het ontvangen of vaststellen van een dataclassificatie tijdens een intake van een beveiligingsonderzoek is noodzakelijk omdat dit een weegfactor is bij het bepalen van de ernst van een kwetsbaarheid.

#### Omschrijving van de te onderzoeken omgeving
Het is van groot belang dat een beveiligingsonderzoeker op functioneel niveau begrijpt wat het doel is van de te onderzoeken omgeving. Een omschrijving van de functionaliteiten binnen een omgeving en een proces diagram zijn daarom van groot belang.

#### Omgevingsspecifiek beveiligingsonderzoek
In overleg met de opdrachtgever dient te worden bepaald op welke omgeving het beveiligingsonderzoek wordt uitgevoerd, zoals bijvoorbeeld een acceptatie of productie omgeving.


---------------

#### Braindump

1. Uit hoeveel servers is de omgeving opgebouwd?
2. Wat zijn de IP adressen van deze server(s)
3. Wordt er gebruik gemaakt van zowel IPv4 als IPv6?
4. Uit welke type besturingssystemen bestaat de te onderzoeken omgeving?
5. Hoe wordt data opgeslagen? Database / file system etc.?
6. Indien er gebruik wordt gemaakt van data encryptie, hoe is dit opgezet en geconfigureerd? Is het symetrisch of a-symetrich? Indien van toepassing, waar wordt de sleutel bewaard? 
7. Netwerk tekening / diagram
8. Externe afhankelijkheden (externe services zoals bijv. API's)
9. Gebruikte technologieen netwerk
10. Gebruikte technologieen infrastructuur
11. Gebruikte technologieen applicaties

#### Netwerk technologoieen

1. Aanwezigheid WAF
2. Aanwezigheid content inspectie?
3. ...

##### Infrastructuur technologieen

1. OS
2. Database
3. Koppelingen zoals MQ
4. Zijn er taken die periodiek worden uitgevoerd op specifieke tijdstippen?
5. Versleuteling van data (at rest? in transit? layer 6?)
6. Indicatie hoeveelheid records opgeslagen zijn (indien van toepassing bij verwerking persoonsgegevens)

##### Applicatieve technologieeen e.a.

1. Van welke taal of talen worden gebruikt?
2. Wordt er gebruik gemaakt van een framework? Zo ja, welke?
3. Hoe wordt gebruikersbeheer geregeld?
4. Hoeveel gebruikers maken gebruik van de applicatie?
5. Hoeveel rollen zijn er binnen een applicatie? Overzicht en omschrijving rollen is noodzakelijk.
6. Wat zijn de authenticatie methodes?
7. Documentatie (link)
8. Source code (link)
9. Changelog (link)
10. Happy flow diagram (link)
