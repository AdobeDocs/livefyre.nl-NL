---
description: Opmerkingen bij de release van 5 oktober 2017.
title: 5 oktober 2017
exl-id: 6e39a86e-82dd-47ff-ad68-2b483f8b1921
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 5 oktober 2017{#october}

Opmerkingen bij de release van 5 oktober 2017.

## Productievrijgave

| **Type probleem** | **Component** | **Opmerking vrijgeven** |
|---|---|---|
| Bug | Livefyre-id | Klanten die de Livefyre-identiteit gebruikten om zich aan te melden, ondervonden problemen bij het zien of bijwerken van hun avatars tijdens het posten naar apps met opmerkingen. Dit is nu opgelost, omdat avatars nu zichtbaar zijn en kunnen worden bijgewerkt. |
| Bug | Rights Management | Oplossing voor een probleem met het weergeven van lange gebruikersnamen op het tabblad Rights Modal. |
| Verbetering | Streams | De mogelijkheid toegevoegd om op de Tab-toets te drukken in een tekstveld Streams om een zoekterm te voltooien. |

## UAT Release

| **Type probleem** | **Component** | **Opmerking vrijgeven** |
|---|---|---|
| Verbetering | Filmstrip | Wanneer een klant een filmstrip-app implementeert, heeft de nieuwe gestreamde UGC een &quot;nieuw&quot; label om deze snel te kunnen identificeren. |
| Verbetering | Filmstrip | Filmstrip is een gloednieuwe visualisatie-app die speciaal is ontworpen om UGC in e-commercescenario&#39;s te laten zien, zoals productpagina&#39;s of transactiewebsites. Met Filmstrip wordt de UGC horizontaal uitgelijnd en weergegeven als een camerarol, één stuk tegelijk. Eindgebruikers kunnen door Filmstrip navigeren door op de zijpijlen te klikken om door de beschikbare inhoud te bladeren. |
| Verbetering | Bibliotheek | Bestanden die door een klant naar de bibliotheek zijn geüpload, worden automatisch toegewezen. Dit is een handige functie wanneer gebruikers het filter &#39;Rechten vereisen verleend&#39; hebben ingeschakeld in hun apps. |
| Verbetering | Livefyre-id | Klanten kunnen nu hun Github-gegevens gebruiken om zich aan te melden bij LIvefyre Identity en deel te nemen aan onze apps voor opmerkingen. |
| Bug | Rights Management | Het probleem waarbij Unicode-tekens konden worden ingevoegd in Rights Request-berichten om validatie te omzeilen, is opgelost. |
| Verbetering | VEILIG | Kleine verbeteringen toegevoegd aan SAFE Spam-detectie. |
| Bug | Service | Gebruikers zonder geldige e-mails hebben e-mails voor hen geconstrueerd. Probleem verholpen met productielogboeken waarbij het systeem geen e-mails naar deze gebruikers heeft verzonden. |
| Verbetering | Studio | De koppeling Help bij LiveCycle is bijgewerkt in de bovenste navigatiebalk. |
| Verbetering | UGC-handel | Als klant kan ik nu één LiveCycle-app (mozaïek, filmstrip of mediamuur) maken en deze insluiten in meerdere productpagina&#39;s, die dynamisch de juiste UGC voor elke productpagina filtert (bijvoorbeeld UGC met schoenen voor een schoenproductpagina). |
| Verbetering | UGC-handel | Klanten kunnen nu handmatig een Google-productcatalogus uploaden naar Livefyre-studio met behulp van een JSON-bestandsuitvoer. Dit laat de klant toe om UGC met producten van die catalogus te combineren en hen in onze handel toegelaten apps te visualiseren. |
| Verbetering | UGC-handel | Klanten kunnen selecteren welke productmappen ze willen gebruiken wanneer ze hun e-commercetoepassing filteren op product-id. Ik wil bijvoorbeeld dat mijn nieuwe filmstrip op de productpagina&#39;s van schoenen en dameszakken komt en daarom zal ik alleen de productmappen &quot;Women&#39;s schoenen collection&quot; en &quot;Women&#39;s bags&quot; selecteren. |
| Verbetering | UGC-handel | Livefyre-klanten kunnen de gepubliceerde UGC nu alleen naar hun apps filteren als ze rechten hebben gekregen. Een klant kan bijvoorbeeld een selectie van items beheren en publiceren, maar deze items worden pas in de app weergegeven nadat de auteur aan deze items machtigingen heeft verleend. Dit is met name van belang voor gevallen waarin de UGC voor commerciële doeleinden wordt gebruikt. |
