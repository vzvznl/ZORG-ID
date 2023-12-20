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

* Compliance met wet- en regelgeving: Een PKI-infrastructuur kan helpen bij het voldoen aan andere relevante wetten en regelgeving, zoals eIDAS (electronic IDentification And trust Services) voor internationale interoperabiliteit.&#x20;
* Het kunnen intrekking van toegangsrechten: PKI maakt het mogelijk om snel en effectief toegangsrechten in te trekken door het intrekken van digitale certificaten, wat bijdraagt aan NEN7512 waar specifieke eisen worden gesteld aan het intrekken van toegangsrechten bij hoog-risico-informatiesystemen.
* Voldoen aan de specifieke eisen van NEN7510, NEN7511 en NEN7512 en tegelijkertijd de vertrouwelijkheid, integriteit en beschikbaarheid van zorginformatie kunnen waarborgen.
  * Uitgifte en Toegangsbeheer: PKI biedt sterke authenticatie, waaronder de uitgifte en het gebruik van digitale identifiers (certificaten), wat bijdraagt aan het waarborgen van passende toegangsrechten tot zorginformatie.
  * Cryptografie: PKI maakt gebruik van sterke crypto grafische technieken, zoals digitale handtekeningen en versleuteling, om de vertrouwelijkheid en integriteit van informatie te waarborgen.
  * Elektronische identificatie en authenticatie met hoog betrouwbaarheidsniveau: PKI zorgt voor een betrouwbaar identificatie- en authenticatiemechanisme, waardoor logging en monitoring nauwkeuriger en traceerbaarder worden.
* Toetsen van attributen: Een sterke identiteit wordt getoetst aan attributen om de organisatie, rol en codering van deze identiteit verder te specificeren.
* NIS2-richtlijnen (Netwerk- en Informatiesystemen) zijn eind 2022 vastgesteld door de Europese Unie en is gericht op een versterking van de digitale en economische weerbaarheid van de Europese lidstaten. Een PKI-infrastructuur (Public Key Infrastructure) voor authenticatie kan hierbij bijdragen aan de naleving van de NIS2-richtlijen door enkele kernprincipes van de richtlijn te ondersteunen, zoals:
  * Beveiliging van netwerk en Informatiesystemen. Zie toegangscontrole (Artikel 7) en maatregelen voor beveiliging (Artikel 14)
  * Incidentenrapportage. Zie traceerbaarheid (Artikel 14 en 15)
  * Samenwerking en informatie uitwisseling. Vertrouwelijkheid en Interoperabiliteit (Artikel 12)
  * Basis beveiligingsverplichtingen (Artikel 19)
  * Certificering van dienstverleners (Artikel 8)
  * Risico beheer (Artikel 13)
  * Preventieve maatregelen (Artikel 14)
  * Herstelmaatregelen (Artikel 15)
* eIDAS richtlijnen, zie de eIDAS uitvoeringsverordening 2015/1502 over betrouwbaarheidsniveaus, de cybersecurity- en ontwerp verordening. Ook dient rekening te worden gehouden met aanpalende kaders zoals de Algemene Verordening Gegevensbescherming (AVG). Hoewel eIDAS niets zegt over de vorm van ZORG-ID, zal dit in de praktijk neerkomen op een mobiele applicatie (Smartphone) die kan worden gebruikt als nationale elektronische identiteit, zowel online als offline, voor allerlei zorg diensten. ZORG-ID ontvangen hun inhoud van gecertificeerde authentieke bronnen en attribuutproviders. Vertrouwende partijen moeten geregistreerd zijn, zodat ZORG-ID de authenticiteit kan verifiëren. Alle actoren in het ZORG-ID ecosysteem moeten voldoen aan de technische architectuur, standaarden, referenties en richtlijnen voor het implementeren van eWallets, zoals gesteld in de eIDAS ontwerpverordening. Hier enkele vertaalde eisen. De Engelstalige teksten zijn echter leidend:

<table><thead><tr><th width="138">Bron</th><th>Eis</th></tr></thead><tbody><tr><td>Art. 6a (3)</td><td><p>Met Europese digitale identiteitsportemonnees kan de gebruiker: </p><p>(a) veilig opvragen en verkrijgen, opslaan, selecteren, combineren en delen, op een manier die transparant is voor en herleidbaar is voor de gebruiker, van de noodzakelijke identificatiegegevens van rechtspersonen en elektronische attesteringen van attributen om online en offline te authentiseren om online te gebruiken openbare en particuliere diensten;</p><p>(b) ondertekenen door middel van gekwalificeerde elektronische handtekeningen.</p></td></tr><tr><td>Art 6a (4a)</td><td><p>Digitale identiteitsportemonnees bieden een generieke interface: </p><p>(1) aan gekwalificeerde en niet-gekwalificeerde vertrouwens-diensten die gekwalificeerde en niet-gekwalificeerde elektronische attesteringen van attributen of andere gekwalificeerde en niet-gekwalificeerde certificaten afgeven met het oog op de afgifte van dergelijke attesteringen en certificaten aan de European Digital Identity Wallet </p><p>(2) voor vertrouwende partijen om persoonsidentificatiegegevens en elektronische attesteringen van attributen op te vragen en te valideren </p><p>(3) voor de presentatie aan vertrouwende partijen van persoonsidentificatiegegevens, elektronische attestering van attributen of andere gegevens zoals inloggegevens, in lokale modus zonder internettoegang voor de portemonnee</p><p> (4) voor de gebruiker om interactie met de European Digital Identity Wallet mogelijk te maken en een "EU Digital Identity Wallet Trust Mark" te tonen</p></td></tr><tr><td>Art. 6a (4b)</td><td>Zekerstellen dat vertrouwensdiensten van gekwalificeerde attesteringen van attributen geen informatie kunnen ontvangen over het gebruik van deze attributen.</td></tr><tr><td>Art. 6a (4c)</td><td>Voldoen aan de vereisten van Artikel8 met betrekking tot het betrouwbaarheidsniveau "hoog", met name zoals toegepast op de vereisten voor identiteitsbewijs en -verificatie, en beheer en authenticatie van elektronische identificatiemiddelen.</td></tr><tr><td>Art. 6a (4d)</td><td>Zorgen voor een mechanisme om ervoor te zorgen dat de vertrouwende partij de gebruiker kan authentiseren en elektronische attesteringen van attributen kan ontvangen.</td></tr><tr><td>Art. 6a (4e)</td><td>Ervoor zorgen dat bedoelde persoonsidentificatiegegevens op unieke en duurzame wijze de natuurlijke of rechtspersoon vertegenwoordigen die ermee in verband wordt gebracht.</td></tr><tr><td>Art. 6a (7)</td><td>Persoonsgegevens met betrekking tot de levering van Europese digitale identiteitsportemonnees worden fysiek en logisch gescheiden van alle andere gegevens bewaard.</td></tr></tbody></table>

## Scenario's

ZORG-ID SMART (ZORG-ID met Smartphone) biedt verschillende functionaliteiten aan, dat gebruikers in staat stelt om identiteitsgegevens, inloggegevens en attributen uit te kunnen lezen en op te slaan, die aan een identiteit zijn gekoppeld en deze op verzoek aan vertrouwde partijen te verstrekken en te gebruiken voor authenticatie en om (gekwalificeerde) elektronische handtekeningen te creëren.

* Een WID (Wet Identificatie bij Dienstverlening) scan kunnen uitvoeren (om de identiteit van een patiënt vast te stellen a.d.h.v. een wettelijk identiteitsbewijs)&#x20;
* Lokaal inloggen door (zorg) medewerkers met UZI-pas of Smartphone
* Lokale autorisatie vastleggen a.d.h.v. (uitgegeven en vastgelegde) attributen
* Ondertekenen met lokale identiteit met UZI-pas of Smartphone
* Ondertekenen van inschrijftoken voor landelijke gegevensuitwisseling&#x20;

## Use-cases

#### Eindgebruikers

| Use-case   | Omschrijving              | Betrokken actoren                                          |
| ---------- | ------------------------- | ---------------------------------------------------------- |
| ZID-UC-001 | Open sessie/authenticatie | <ul><li>ZORG applicatie</li><li>(Zorg)medewerker</li></ul> |
| ZID-UC-002 | Scan WID                  |                                                            |
| ZID-UC-003 | Ondertekenen van token    |                                                            |

#### Backoffice administratie



#### Backoffice administratie voor personeelsbeheer van zorgorganisaties

####





## Bedrijfsobjecten



## Kwaliteitseisen
