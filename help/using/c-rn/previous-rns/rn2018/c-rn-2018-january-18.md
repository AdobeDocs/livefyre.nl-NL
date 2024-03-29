---
description: Opmerkingen bij de release van 18 januari 2018.
title: 18 januari 2018
exl-id: aaf49dc9-64eb-4354-8bcb-04039fa25f10
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# 18 januari 2018{#january}

Opmerkingen bij de release van 18 januari 2018.

## Productievrijgave

| **Type probleem** | **Component** | **Opmerking vrijgeven** |
|---|---|---|
| Bug | Apps | Het probleem waarbij Avatars niet correct werden gerenderd tijdens het gebruik van een JPEG-bestand, is opgelost. |
| Bug | ModQ | Oplossing voor een bug voor klanten van S1 om het filtreren door Inzamelingen in ModQ toe te staan. |
| Bug | Streams | Het probleem waarbij een streamregel werd verbroken toen het taalfilter werd ingesteld op Geen, is opgelost. |
| Bug | Streams | Het probleem waarbij de YouTube-stroomregels niet werden opgeslagen, is opgelost. |
| Bug | Streams | Hiermee wordt een fout verholpen waarbij gebruikers onjuist opgemaakte geo-items in streaming regels kunnen maken en opslaan, waardoor de stream zou mislukken. Gebruikers kunnen nu niet meer slecht opgemaakte geo-tags opslaan. |
| Bug | Studio | Probleem verholpen waardoor sommige gebruikers zich niet konden aanmelden bij LiveCycle. |

## UAT Release

| **Type probleem** | **Component** | **Opmerking vrijgeven** |
|---|---|---|
| Bug | Bibliotheek | Beveiligingsfout verhelpen. Alle verificatieaanroepen worden nu uitgevoerd met het HTTPS-protocol in plaats van met HTTP. |
| Verbetering | Slimme tags | Gestroomde inhoud wordt nu automatisch slim gecodeerd door Adobe Sensei als deze wordt opgeslagen in een map of gepubliceerd naar een app. |
| Bug | Streams | Probleem verholpen waarbij Japanse tekens niet werden herkend door Instagram-streamregels. |
| Verbetering | Streams | Klanten kunnen nu de logische operatoren (ANY, ALL, NOT) gebruiken om gedetailleerde filters voor slimme tags te maken in streams die nauwkeuriger inhoud beheren. Als ik bijvoorbeeld de hashtag #himalyas gebruik, kan ik alleen afbeeldingen weergeven die &#39;sneeuwgordijnen&#39; bevatten. |
| Bug | Studio | Los dit probleem op door speciale tekens in namen als HTML weer te geven. |
