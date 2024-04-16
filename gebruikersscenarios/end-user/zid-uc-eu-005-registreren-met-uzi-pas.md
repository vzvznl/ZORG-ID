---
description: Een gebruiker met UZI-pas kan zichzelf registreren bij ZORG-ID.
---

# ZID-UC-EU-005 Registreren met UZI-pas

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption><p>Registratie proces met UZI-pas</p></figcaption></figure>

## Step-up registratieproces met UZI-pas

### Pre-conditie

* Gebruiker heeft een “Zorgverlener” of “Medewerker op naam” UZI-pas type.
* Gebruiker heef ZORG-ID Mobile App geïnstalleerd op een smartphone (Android of iPhone) en een PIN code ingevoerd.
* URA en naam van zorgaanbieder is geregistreerd in ZORG-ID.

### Post-conditie

* De gebruiker kan zijn ZORG-ID Mobile App gebruiken om zich te authentiseren met zijn ZORG-ID identiteit bij die systemen die gebruik maken van ZORG-ID.



### Proces flow

1. Gebruiker navigeert naar ZORG-ID Registratie UZI-Portaal voor identificatie met UZI-pas. Zie volgende URL's:&#x20;
   * productie omgeving: https://productie.zorg-id.nl/uzi-portaal of&#x20;
   * acceptatie omgeving: https://acceptatie.zorg-id.nl/uzi-portaal
2. Gebruiker voert de pincode van zijn UZI-pas in.
3. Indien pincode of UZI-pas ongeldig is, meldt dit en toon aan gebruiker dat het registratie proces stopt.
4. UZI-pas gegevens worden uitgelezen.&#x20;
   * URA
   * Voornaam en achternaam
   * Rolcode
   * UZI-nummer
5. URA wordt gecontroleerd of deze bij ZORG-ID is geregistreerd.
   * Indien URA onbekend is, stopt het registratie proces en meldt dat URA onbekend is in ZORG-ID.
6. De geboortedatum wordt van de gebruiker in een dialoog opgevraagd.
7. ZORG-ID controleert of de identiteit van de gebruiker a.d.h.v. URA, voornaam, achternaam en geboortedatum geregistreerd is bij ZORG-ID.
   1. Bij een nieuwe identiteit van een gebruiker,
      1. Registreert ZORG-ID een nieuwe ZORG-ID gebruikersnaam. De ZORG-ID gebruikersnaam is samengesteld uit voornaam, achternaam en UZI-nummer.
      2. Koppelt de ZORG-ID gebruikersnaam aan een ZORG-ID organisatie via de URA van de UZI-pas.
      3. Gebruiker bevestigd door het ondertekenen van de acties 7.1.1. en 7.1.2. met zijn UZI-pas.
      4. De gebruiker ziet zijn ZORG-ID gebruikersnaam en zijn attributen ‘UZI-nummer’ en ‘rolcode’ van de UZI-pas verschijnen.
      5. ZORG-ID genereert een QR-code voor het personaliseren van de ZORG-ID Mobiele App.
   2. Bij een bestaande identiteit, die bevestigd wordt door de gebruiker:
      1. Worden de attributen ‘UZI-nummer’ en ‘rolcode’ van de UZI-pas overgenomen.
      2. De gebruiker bevestigd door het ondertekenen van de acties 7.2.1.met zijn UZI-pas
      3. ZORG-ID genereert een QR-code voor het personaliseren van de ZORG-ID Mobiele App.
8. Gebruiker wordt gevraagd zijn ZORG-ID Mobile App te openen en de QR-code te scannen en te bevestigen.
9. Gebruiker is nu m.b.v. zijn UZI-pas geregistreerd, en alle gegevens van de UZI-pas zijn als attributen overgenomen en gekoppeld aan zijn ZORG-ID gebruikersnaam.&#x20;
10. De gebruiker kan nu ZORG-ID Mobile App gebruiken om in te loggen op die zorgapplicaties die gebruik maken van ZORG-ID.
11. Gebruiken kan het registratie proces nu afsluiten door het ZORG-ID Registratie UZI-portaal te verlaten met een afsluitknop.
