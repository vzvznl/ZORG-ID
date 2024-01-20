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

<figure><img src=".gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

### Token gebaseerd Authenticatie en Autorisatie

Voor token-gebaseerde authenticatie/autorisatie biedt het systeem identiteiten met:

#### Signing functionaliteit

* Volgt de 'NEN-EN 419241 Trustworthy Systems Supporting Server Signing'
* Maakt gebruik van identiteitsattribuut certificaten voor het ondertekenen van transacties.





