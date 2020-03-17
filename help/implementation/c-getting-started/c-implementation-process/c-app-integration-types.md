---
description: Wanneer u LiveCycle Apps implementeert, hangt de implementatiestijl af van uw gebruiksscenario. Op deze pagina worden de functies uitgelegd voor de drie manieren waarop u een app kunt maken.
seo-description: Wanneer u LiveCycle Apps implementeert, hangt de implementatiestijl af van uw gebruiksscenario. Op deze pagina worden de functies uitgelegd voor de drie manieren waarop u een app kunt maken.
seo-title: Integratie van CMS-toepassingen
solution: Experience Manager
title: Integratie van CMS-toepassingen
uuid: 14fd7e36-0e50-4ae3-97f0-2de731c184f5
translation-type: tm+mt
source-git-commit: 67aeb3de964473b326c88c3a3f81ff48a6a12652

---


# Integratie van CMS-toepassingen{#cms-app-integrations}

Wanneer u LiveCycle Apps implementeert, hangt de implementatiestijl af van uw gebruiksscenario. Op deze pagina worden de functies uitgelegd voor de drie manieren waarop u een app kunt maken.

Integratie van Livefy is niet bekend met CMS en gebruikersprofiel en Auth-platform. Voer Livefyre op één of meerdere manieren uit, afhankelijk van uw gebruiks-geval en vereisten.

Met traditionele integratie kunt u aangepaste AEM-componenten maken.

## Overzicht van CMS App Integration Type

| Type | Ontwikkelingsvereiste | Functies | Pros | Beperkingen |
|--- |--- |--- |--- |--- |
| App Designer | Zeer laag | Maak JS-insluitingen in Studio en voeg deze toe aan pagina&#39;s zonder dat er een <br>beperkt aantal stijlen en configuraties beschikbaar is </br>Gebruiksscenario: Pagina&#39;s voor één gebruik (gebeurtenisdekking, campagnes, hubs) | Kan een app binnen een korte tijd aan de slag krijgen. <br>Configuraties kunnen worden uitgevoerd door een niet-technisch lid. <br>Eenvoudig en eenvoudig te wijzigen in configuraties | Moet eerst een app maken met LiveCyre Studio <br>niet geautomatiseerd |
| Livefyre.js | Normaal | Apps integreren in het JavaScript van uw pagina&#39;s <br>Gebruik hoofdlettergebruik: Herbruikbare sjablonen (redactionele inhoud, productreeksen) | Gebruik de volledige reeks van de aanpassingen en configuraties van de Toepassing <br>Automatiseert het proces om toepassingen van binnen uw CMS op uw pagina&#39;s dynamisch te concretiseren | Ik heb een ontwikkelaar nodig. |
| SDK API&#39;s | Geavanceerd | Haal uw inhoud van Livefy op om te gebruiken voor aangepaste toepassingen <br>Pas de front-end-out aan, maar niet-ondersteunde <br>gebruiksscenario&#39;s: Integratie van gegevens/analyses en aangepaste front-end apps | Volledige macht over de blik en het gevoel van App | Vereist ontwikkeling op voorhand. <br>Hoger ontwikkelingsniveau om te implementeren. |