---
description: >-
  Deze pagina beschrijft de informatiesystemen architectuur en de samenwerking
  tussen de deelnemende systemen van ZORG-ID.
---

# Informatiesystemen architectuur

## ZORG-ID Informatiesystemen beschrijving

### Doel en overwegingen

Deze documentatie heeft als doel het ZORG-ID platform te beschrijven, een dienst voor de Nederlandse gezondheidszorg die voldoet aan de eIDAS 2.0 verordening. Het ZORG-ID platform faciliteert authenticatie, op attributen gebaseerde autorisatie en elektronische ondertekening. Het dient als hulpmiddel voor het mogelijk maken van toegang tot medische toepassingen, evenals voor het raadplegen en wijzigen van centraal opgeslagen medische gegevens.

Deze architectuur richt zich specifiek op centraal opgeslagen digitale identiteiten en daarbij behorende attributen. Door deze benadering wordt een minder kostbare en flexibelere oplossing geboden, vooral in situaties waarin smartcards (UZI-pas) minder praktisch zijn. Het stelt medische toepassingen in staat om snel en effectief gebruik te maken van de attributen en autorisaties die gekoppeld zijn aan de centraal opgeslagen digitale identiteiten.

### Logisch model

Het logisch model dat hieronder wordt weergegeven geeft een beschrijving van de betrokken ZORG-ID componenten en de aangeboden diensten.&#x20;

<figure><img src=".gitbook/assets/image (16).png" alt=""><figcaption><p>De componenten van ZORG-ID</p></figcaption></figure>

### Componenten en interfaces

<table><thead><tr><th width="271">Component/Interface</th><th>Omschrijving</th></tr></thead><tbody><tr><td>Agent (Browser)</td><td>Een op een gebruikersagent gebaseerde toepassing waarbij de clientcode wordt uitgevoerd binnen een gebruikersagent (bijvoorbeeld een webbrowser) op het apparaat dat wordt gebruikt door de eigenaar van de bron (dat wil zeggen, de eindgebruiker).</td></tr><tr><td>ZID Desktop App</td><td>De ZID Desktop App is een eindgebruikerstoepassing die geïnstalleerd is op een Windows-desktopcomputer of een Apple OS-desktopcomputer. De ZID Desktop App biedt het systeem de mogelijkheid om indirect met een smartcard te communiceren via de SDK en de ZID Server.</td></tr><tr><td>UZI Card Reader</td><td>De UZI Card Reader ontsluit de beveiliging van de certificaten op de UZI pas en de software op een desktop. Het ontsluiten van de beveiliging komt tot uiting in het vragen van een PIN code. Hierbij zijn er diverse afhankelijkheden van het operating systeem van de desktop of server.</td></tr><tr><td>QR-code</td><td>De QR-code wordt gebruikt om met een mobiele App te kunnen  authentiseren en in te loggen op een netwerk, dat wil zeggen zonder dat verdere inloggegevens ingevoerd hoeven te worden.</td></tr><tr><td>ZID Mobiele App</td><td>De ZID Mobiele App is een eindgebruikers applicatie, geïnstalleerd op een iOS- of Android smartphone. De ZID Mobiele App biedt het systeem een faciliteit om indirect te communiceren met een lokale ZID-identiteit via de SDK Web - en ZID Service.</td></tr><tr><td>ZID Façade (SDK Web Service)</td><td>De SDK Web Service is een Software Development Kid (zichtbare buitenkant van de ZID Service) die de zorgaanbieder kan gebruiken om toegang te krijgen tot de functionaliteit van de ZID service. De SDK biedt data, sessie en transactie beheer functionaliteit.</td></tr><tr><td>Secure Element Store</td><td>Hier wordt de X509-certificaat objecten beheerd met bijgevoegde verwijzingen naar een privésleutel, Via deze weg kunnen SAML-tokens en hash resultaten ondertekening transacties uitgevoerd en gevalideerd worden a.d.h.v. een aangeleverde X509-certificaat.</td></tr><tr><td>data manager</td><td>De datamanager is verantwoordelijk voor het ophalen van WID-gegevens, nadat er een WID-scan is uitgevoerd m.b.v. de ZID Mobiele App</td></tr><tr><td>session manager</td><td>De session manager is verantwoordelijk voor het initialiseren van een nieuwe sessie. Wanneer een sessie wordt geopend, kan de SDK Web Service via de transaction manager toegang krijgen tot de (digitale) identiteit (UZI-pas of ZID-lokaal) voor ondertekening verwerkingen.</td></tr><tr><td>transaction manager</td><td>De transaction manager is verantwoordelijk voor het indienen en controleren van ingediende ondertekenings-transacties. Voordat men de transaction manager kan gebruiken, moet een sessie geopend zijn.</td></tr></tbody></table>

### Token gebaseerd Authenticatie en Autorisatie

Voor token-gebaseerde authenticatie/autorisatie biedt het systeem identiteiten met:

#### Signing functionaliteit

* Volgt de 'NEN-EN 419241 Trustworthy Systems Supporting Server Signing'
* Maakt gebruik van identiteitsattribuut certificaten voor het ondertekenen van transacties.





