---
description: >-
  Deze pagina beschrijft de bedrijfsarchitectuur waarin beschreven staat welke
  processen onder welke condities ondersteund worden door ZORG-ID.
---

# Bedrijfsarchitectuur

## ZORG-ID

ZORG-ID is een generiek, centraal, veilig en vertrouwd platform voor identificatie en authenticatie in de zorg. ZORG-ID kent een veelheid aan toepassingen in de zorg, voldoet aan alle relevante standaarden van wet- en regelgeving en maakt een snelle en eenvoudige integratie mogelijk in zorgapplicaties ook met het oog op toekomstige ontwikkelingen en/of veranderingen op dit gebied.

## Positie van ZORG-ID

## Kaders

* Compliance met wet- en regelgeving: Een PKI-infrastructuur kan helpen bij het voldoen aan andere relevante wetten en regelgeving, zoals de WDO (Wet Digitale Overheid) voor het veilig en betrouwbaar kunnen inloggen en eIDAS (electronic IDentification And trust Services) voor internationale interoperabiliteit.&#x20;
* Het kunnen intrekking van toegangsrechten: PKI maakt het mogelijk om snel en effectief toegangsrechten in te trekken door het intrekken van digitale certificaten, wat bijdraagt aan NEN7512 waar specifieke eisen worden gesteld aan het intrekken van toegangsrechten bij hoog-risico-informatiesystemen.
* Voldoen aan de specifieke eisen van NEN7510, NEN7511 en NEN7512 en tegelijkertijd de vertrouwelijkheid, integriteit en beschikbaarheid van zorginformatie kunnen waarborgen.
  * Uitgifte en Toegangsbeheer: PKI biedt sterke authenticatie, waaronder de uitgifte en het gebruik van digitale identifiers (certificaten), wat bijdraagt aan het waarborgen van passende toegangsrechten tot zorginformatie.
  * Cryptografie: PKI maakt gebruik van sterke crypto grafische technieken, zoals digitale handtekeningen en versleuteling, om de vertrouwelijkheid en integriteit van informatie te waarborgen.
  * Elektronische identificatie en authenticatie met hoog betrouwbaarheidsniveau: PKI zorgt voor een betrouwbaar identificatie- en authenticatiemechanisme, waardoor logging en monitoring nauwkeuriger en traceerbaarder worden.
* Toetsen van attributen: Een sterke identiteit wordt getoetst aan attributen om de organisatie, rol en codering van deze identiteit verder te specificeren. Zie ook eIDAS richtlijnen (Art. 6a).
* NIS2-richtlijnen (Netwerk- en Informatiesystemen) zijn eind 2022 vastgesteld door de Europese Unie en is gericht op een versterking van de digitale en economische weerbaarheid van de Europese lidstaten. Een PKI-infrastructuur (Public Key Infrastructure) voor authenticatie kan hierbij bijdragen aan de naleving van de NIS2-richtlijen door enkele kernprincipes van de richtlijn te ondersteunen, zoals:
  * Beveiliging van netwerk en Informatiesystemen. Zie toegangscontrole (Art. 7) en maatregelen voor beveiliging (Artikel 14)
  * Incidentenrapportage. Zie traceerbaarheid (Art. 14 en 15)
  * Samenwerking en informatie uitwisseling. Vertrouwelijkheid en Interoperabiliteit (Art. 12)
  * Basis beveiligingsverplichtingen (Art. 19)
  * Certificering van dienstverleners (Art. 8)
  * Risico beheer (Art. 13)
  * Preventieve maatregelen (Art. 14)
  * Herstelmaatregelen (Art. 15)
* De WDO (Wet Digitale Overheid) is een zogeheten kaderwet en regelt algemene principes, verantwoordelijkheden en procedures, maar geen gedetailleerde regels.&#x20;
* Verplichtingen standaarden voor veiligheid (Art3. WDO) . Grondslag voor het gebruik van beveiligde verbinding met overheids websites en -webapplicaties.  HTTPS-configuraties moeten voldoen aan de TLS-richtlijnen en web applicatie richtlijnen van het Nationaal Cyber Security Centrum (NCSC).
* eIDAS richtlijnen, zie de eIDAS uitvoeringsverordening 2015/1502 over betrouwbaarheidsniveaus, de cybersecurity- en ontwerp verordening. Ook dient rekening te worden gehouden met aanpalende kaders zoals de Algemene Verordening Gegevensbescherming (AVG). Hoewel eIDAS niets zegt over de vorm van ZORG-ID, zal dit in de praktijk neerkomen op een mobiele applicatie (Smartphone) die kan worden gebruikt als nationale elektronische identiteit, zowel online als offline, voor allerlei zorg diensten. ZORG-ID ontvangen hun inhoud van gecertificeerde authentieke bronnen en attribuutproviders. Vertrouwende partijen moeten geregistreerd zijn, zodat ZORG-ID de authenticiteit kan verifiëren. Alle actoren in het ZORG-ID ecosysteem moeten voldoen aan de technische architectuur, standaarden, referenties en richtlijnen voor het implementeren van eWallets, zoals gesteld in de eIDAS ontwerpverordening. Hier enkele vertaalde eisen. De Engelstalige teksten zijn echter leidend:

<table><thead><tr><th width="138">Bron</th><th>Eis</th></tr></thead><tbody><tr><td>Art. 6a (3)</td><td><p>Met Europese digitale identiteitsportemonnees kan de gebruiker: </p><p>(a) veilig opvragen en verkrijgen, opslaan, selecteren, combineren en delen, op een manier die transparant is voor en herleidbaar is voor de gebruiker, van de noodzakelijke identificatiegegevens van rechtspersonen en elektronische attesteringen van attributen om online en offline te authentiseren om online te gebruiken openbare en particuliere diensten;</p><p>(b) ondertekenen door middel van gekwalificeerde elektronische handtekeningen.</p></td></tr><tr><td>Art. 6a (4a)</td><td><p>Digitale identiteitsportemonnees bieden een generieke interface: </p><p>(1) aan gekwalificeerde en niet-gekwalificeerde vertrouwens-diensten die gekwalificeerde en niet-gekwalificeerde elektronische attesteringen van attributen of andere gekwalificeerde en niet-gekwalificeerde certificaten afgeven met het oog op de afgifte van dergelijke attesteringen en certificaten aan de European Digital Identity Wallet </p><p>(2) voor vertrouwende partijen om persoonsidentificatiegegevens en elektronische attesteringen van attributen op te vragen en te valideren </p><p>(3) voor de presentatie aan vertrouwende partijen van persoonsidentificatiegegevens, elektronische attestering van attributen of andere gegevens zoals inloggegevens, in lokale modus zonder internettoegang voor de portemonnee</p><p> (4) voor de gebruiker om interactie met de European Digital Identity Wallet mogelijk te maken en een "EU Digital Identity Wallet Trust Mark" te tonen</p></td></tr><tr><td>Art. 6a (4b)</td><td>Zekerstellen dat vertrouwensdiensten van gekwalificeerde attesteringen van attributen geen informatie kunnen ontvangen over het gebruik van deze attributen.</td></tr><tr><td>Art. 6a (4c)</td><td>Voldoen aan de vereisten van Artikel8 met betrekking tot het betrouwbaarheidsniveau "hoog", met name zoals toegepast op de vereisten voor identiteitsbewijs en -verificatie, en beheer en authenticatie van elektronische identificatiemiddelen.</td></tr><tr><td>Art. 6a (4d)</td><td>Zorgen voor een mechanisme om ervoor te zorgen dat de vertrouwende partij de gebruiker kan authentiseren en elektronische attesteringen van attributen kan ontvangen.</td></tr><tr><td>Art. 6a (4e)</td><td>Ervoor zorgen dat bedoelde persoonsidentificatiegegevens op unieke en duurzame wijze de natuurlijke of rechtspersoon vertegenwoordigen die ermee in verband wordt gebracht.</td></tr><tr><td>Art. 6a (7)</td><td>Persoonsgegevens met betrekking tot de levering van Europese digitale identiteitsportemonnees worden fysiek en logisch gescheiden van alle andere gegevens bewaard.</td></tr></tbody></table>

## Scenario's

ZORG-ID SMART (ZORG-ID met Smartphone) biedt verschillende functionaliteiten aan, dat gebruikers in staat stelt om identiteitsgegevens, inloggegevens en attributen uit te kunnen lezen en op te slaan, die aan een identiteit zijn gekoppeld en deze op verzoek aan vertrouwde partijen te verstrekken en te gebruiken voor authenticatie en om (gekwalificeerde) elektronische handtekeningen te creëren.

De volgende ZORG-ID Smart scenario's zijn uitgewerkt:

* Een WID (Wet Identificatie bij Dienstverlening) scan kunnen uitvoeren (om de identiteit van een persoon vast te stellen a.d.h.v. een wettelijk identiteitsbewijs).&#x20;
* Lokaal inloggen door (zorg) medewerkers met UZI-pas of Smartphone.
* Lokale autorisatie vastleggen a.d.h.v. (uitgegeven en vastgelegde) attributen.
* Ondertekenen met lokale identiteit met UZI-pas of Smartphone.
* Ondertekenen van inschrijftoken voor landelijke gegevensuitwisseling via het Landelijk Schakelpunt (LSP).

## Use-cases

De volgende Use cases zijn op ZORG-ID Smart gericht.



#### Eindgebruikers (End User)

De use cases voor eindgebruikers tonen de gebruiksscenario's die verband houden met eindgebruikers. De aanvrager-actor is in het use-case model een gezondheidszorgtoepassing.&#x20;

Het gebruiksscenario 'patiënt aanmelden', waarin een ' inschrijftoken' wordt gecreëerd, wordt niet beschouwd als een gebruiksscenario vanuit ZORG-ID Smart. Deze use-case wordt geïmplementeerd door de aanvrager via een combinatie van de volgende use-case: 'Open sessie', 'Token ophalen' en 'Token ondertekenen'.&#x20;

<table><thead><tr><th width="202">Use-case</th><th>Omschrijving</th><th>Betrokken actoren</th></tr></thead><tbody><tr><td>ZID-UC-EU-001</td><td>Open Sessie (authenticatie)</td><td><ul><li>Gezondheidszorgtoepassing</li><li>(Zorg)medewerker</li></ul></td></tr><tr><td>ZID-UC-EU-002</td><td>Scan WID</td><td><ul><li>Gezondheidszorgtoepassing</li><li>(Zorg)medewerker</li></ul></td></tr><tr><td>ZID-UC-EU-003</td><td>Ophalen Token</td><td><ul><li>Gezondheidszorgtoepassing</li></ul></td></tr><tr><td>ZID-UC-EU-004</td><td>Ondertekenen Token</td><td><ul><li>Gezondheidszorgtoepassing</li></ul></td></tr></tbody></table>

#### Backoffice administratie (Backoffice Administration)

De use-cases voor backoffice-administratie betreffen de registratie en het beheer van attributen, type-invoer, administratieve gebruikers van organisaties en systeemvermeldingen voor gezondheidsorganisaties.

Het volgende tabel geeft een overzicht van de use-cases voor backoffice-administratie.



<table><thead><tr><th>Use-case</th><th width="173">Omschrijving</th><th>Betrokken actoren</th></tr></thead><tbody><tr><td>ZID-UC-BA-001</td><td>Inschrijven Attribuuttype</td><td><ul><li>ZORG-ID beheerder (AET)</li></ul></td></tr><tr><td>ZID-UC-BA-002</td><td>Uitschrijven Attribuuttype</td><td><ul><li>ZORG-ID beheerder (AET)</li></ul></td></tr><tr><td>ZID-UC-BA-003</td><td>Authenticatie</td><td><ul><li>ZORG-ID beheerder (AET)</li><li>ZORG-ID beheerder (VZVZ)</li></ul></td></tr><tr><td>ZID-UC-BA-004</td><td>Inschrijven Zorgaanbieder</td><td><ul><li>ZORG-ID beheerder (VZVZ)</li></ul></td></tr><tr><td>ZID-UC-BA-005</td><td>Uitschrijven Zorgaanbieder</td><td><ul><li>ZORG-ID beheerder (VZVZ)</li></ul></td></tr><tr><td>ZID-UC-BA-006</td><td>Inschrijven ZORG-ID beheerder </td><td><ul><li>ZORG-ID beheerder (VZVZ)</li></ul></td></tr><tr><td>ZID-UC-BA-007</td><td>Inschrijven Organisatie beheerder</td><td><ul><li>ZORG-ID beheerder (VZVZ)</li></ul></td></tr><tr><td>ZID-UC-BA-008</td><td>Uitschrijven Organisatie beheerder</td><td><ul><li>ZORG-ID beheerder (VZVZ)</li></ul></td></tr></tbody></table>

#### Backoffice administratie voor personeelsbeheer van zorgorganisaties (Healthcare Administration)

De use-cases voor backoffice-administratie van zorgorganisaties betreffende het inschrijven van personen en het verlenen van rechten (via attributen) en het intrekken van rechten aan personen.



<table><thead><tr><th>Use-case</th><th width="213">Omschrijving</th><th>Betrokken actoren</th></tr></thead><tbody><tr><td>ZID-UC-HA-001</td><td>Authenticatie</td><td><ul><li>Organisatie beheerder</li><li>Organisatie operator</li></ul></td></tr><tr><td>ZID-UC-HA-002</td><td>Inschrijven Organisatie beheerder</td><td><ul><li>Organisatie beheerder</li></ul></td></tr><tr><td>ZID-UC-HA-003</td><td>Uitschrijven Organisatie beheerder</td><td><ul><li>Organisatie beheerder</li></ul></td></tr><tr><td>ZID-UC-HA-004</td><td>Inschrijven Organisatie aanvraag</td><td><ul><li>Organisatie beheerder</li></ul></td></tr><tr><td>ZID-UC-HA-005</td><td>Uitschrijven Organisatie aanvraag</td><td><ul><li>Organisatie beheerder</li></ul></td></tr><tr><td>ZID-UC-HA-006</td><td>Inschrijven Organisatie operator</td><td><ul><li>Organisatie beheerder</li></ul></td></tr><tr><td>ZID-UC-HA-007</td><td>Uitschrijven Organisatie operator</td><td><ul><li>Organisatie beheerder</li></ul></td></tr><tr><td>ZID-UC-HA-008</td><td>Inschrijven gebruiker</td><td><ul><li>Organisatie operator</li><li>Zorgmedewerker</li></ul></td></tr><tr><td>ZID-UC-HA-009</td><td>Uitschrijven gebruiker</td><td><ul><li>Organisatie operator</li></ul></td></tr><tr><td>ZID-UC-HA-010</td><td>Koppel gebruiker aan organisatie</td><td><ul><li>Organisatie operator</li></ul></td></tr><tr><td>ZID-UC-HA-011</td><td>Ontkoppel gebruiker van organisatie</td><td><ul><li>Organisatie operator</li></ul></td></tr><tr><td>ZID-UC-HA-012</td><td>Ken attribuut toe aan gebruiker</td><td><ul><li>Organisatie operator</li></ul></td></tr><tr><td>ZID-UC-HA-013</td><td>Trek attribuut in van gebruiker</td><td><ul><li>Organisatie operator</li></ul></td></tr></tbody></table>





## Bedrijfsobjecten



## Kwaliteitseisen
