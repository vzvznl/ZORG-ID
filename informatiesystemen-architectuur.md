---
description: >-
  Deze pagina beschrijft de informatiesystemen architectuur en de samenwerking
  tussen de deelnemende systemen van ZORG-ID.
---

# Informatiesystemen architectuur

## ZORG-ID Informatiesystemen beschrijving

### Doel en overwegingen

Deze documentatie heeft als doel het ZORG-ID platform te beschrijven, een dienst voor de Nederlandse gezondheidszorg die voldoet aan de eIDAS-normen. Het ZORG-ID platform faciliteert authenticatie, op attributen gebaseerde autorisatie en ondertekening. Het dient als hulpmiddel voor het mogelijk maken van toegang tot medische toepassingen, evenals voor het raadplegen en wijzigen van centraal opgeslagen medische gegevens.

Deze architectuur richt zich specifiek op centraal opgeslagen digitale identiteiten en daarbij behorende attributen. Door deze benadering wordt een minder kostbare en flexibelere oplossing geboden, vooral in situaties waarin smartcards (UZI-pas) minder praktisch zijn. Het stelt medische toepassingen in staat om snel en effectief gebruik te maken van de attributen en autorisaties die gekoppeld zijn aan de centraal opgeslagen digitale identiteiten.

### Logisch model

Het logisch model dat hieronder wordt weergegeven geeft een beschrijving van de betrokken ZORG-ID componenten en de aangeboden diensten.&#x20;

<figure><img src=".gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

### Componenten en interfaces

| Component/Interface | Omschrijving                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Agent (Browser)     | Een op een gebruikersagent gebaseerde toepassing waarbij de clientcode wordt uitgevoerd binnen een gebruikersagent (bijvoorbeeld een webbrowser) op het apparaat dat wordt gebruikt door de eigenaar van de bron (dat wil zeggen, de eindgebruiker).                                       |
| ZID Desktop App     | De ZID Desktop App is een eindgebruikerstoepassing die geïnstalleerd is op een Windows-desktopcomputer of een Apple OSX-desktopcomputer. De ZID Desktop App biedt het systeem de mogelijkheid om indirect met een smartcard te communiceren via de SDK en de ZID Server.                   |
| UZI Card Reader     | De UZI Card Reader ontsluit de beveiliging van de certificaten op de UZI pas en de software op een desktop. Het ontsluiten van de beveiliging komt tot uiting in het vragen van een PIN code. Hierbij zijn er diverse afhankelijkheden van het operating systeem van de desktop of server. |
| QR-code             | De QR-code wordt gebruikt om met een mobiele App in te loggen op een netwerk, dat wil zeggen zonder dat verdere inloggegevens ingevoerd hoeven te worden.                                                                                                                                  |

### Token gebaseerd Authenticatie en Autorisatie

Voor token-gebaseerde authenticatie/autorisatie biedt het systeem identiteiten met:

#### Signing functionaliteit

* Volgt de 'NEN-EN 419241 Trustworthy Systems Supporting Server Signing'
* Maakt gebruik van identiteitsattribuut certificaten voor het ondertekenen van transacties.





