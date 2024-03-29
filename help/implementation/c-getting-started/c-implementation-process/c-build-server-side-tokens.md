---
description: Een gids voor het bouwen van collectionMeta en auth tokens.
title: Server-zijtokens maken
exl-id: f709b79e-9236-443e-b862-c7d281815d91
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---

# Server-zijtokens maken{#build-server-side-tokens}

Een gids voor het bouwen van collectionMeta en auth tokens.

De bouw van de tokens die Livefyre gebruikt om verzoeken te bevestigen zorgt ervoor dat slechts u updates aan uw netwerk van de Levensstijl kunt maken.

## CollectionMeta-token

Leer hoe u een token maakt om nieuwe en bestaande gesprekken te maken.

## Auth Token

Leer hoe u een token maakt voor het verifiëren van gebruikers. Dit is een noodzakelijke stap in het integratieproces als u Janrain Capture niet gebruikt voor gebruikersbeheer.

## Token van auteur {#section_l5l_hwt_bbb}

In deze sectie wordt beschreven hoe u het JSON-object UserAuth genereert dat het token User Authentication (Gebruikersverificatie) maakt dat nodig is om gebruikers aan te melden bij uw apps.

Als u het token wilt maken, gebruikt u de voorkeurstaalbibliotheek om de volgende parameters door te geven:

| Parameter | Type | Beschrijving |
|---|---|---|
| networkName | Tekenreeks *required* | De naam van het Livefyre-netwerk (verstrekt door Livefyre). |
| networkKey | Tekenreeks *required* | De geheime sleutel voor dit specifieke netwerk (verstrekt door Livefyre). |
| userId | Tekenreeks *required* | De id van de gebruiker die zich aanmeldt als opgeslagen in uw gebruikersbeheersysteem (alleen alfanumerieke tekens, streepjes, onderstrepingstekens en punttekens zijn toegestaan: `[a-zA-Z0-9_-.]`). **Opmerking:** de gebruikersnaam moet uniek zijn. |
| verloopt | Geheel *vereist* | Wanneer het token vanaf nu (in seconden) moet verlopen. **Opmerking:** deze waarde kan ook als een zwevende waarde worden doorgegeven. Deze waarde wordt opgeslagen in de JSON-webtoken die wordt gemaakt in de tijdperk UNIX. |
| displayName | Tekenreeks *required* | Tekst om deze gebruiker te identificeren in de gebruikersinterface en in opmerkingen. (Maximum aantal tekens: 50.) |
