---
title: LiveCycle gebruiken met Ander Analyseprogramma
description: LiveCycle gebruiken met Ander Analyseprogramma
exl-id: da29e281-5095-4e99-a248-19390f2059a2
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# LiveCycle gebruiken met Ander Analytics Tool{#use-livefyre-with-other-analytics-tool}

U kunt hulpprogramma&#39;s voor analyse gebruiken om gegevens te verzamelen over gebruikersinteracties met LiveCycle Apps. U kunt naar keuze Adobe Analytics of een ander gereedschap gebruiken.

Als u LiveCycle wilt gebruiken met een gereedschap van uw keuze (niet Adobe Analytics), volgt u de procedure die op deze pagina wordt beschreven.

## Stap 1: Gebeurtenishandler {#section_ngm_gzl_pdb} instellen

Stel een gebeurtenishandler in op pagina&#39;s waarop u Live Apps gebruikt. Op deze manier kunt u gegevens verzamelen van de toepassingen op die pagina die u kunt gebruiken voor analyses.

Voeg Livefyre.js aan een pagina toe aan opstelling de gebeurtenismanager. Livefyre.js wordt asynchroon geladen. Om de bestandsgrootte te verkleinen en de laadprestaties te verbeteren, zijn analyses niet direct beschikbaar. U moet het analyseobject opiniepeilen totdat er gegevens beschikbaar zijn. Plaats dit script ergens op de pagina of bundel het in uw eigen gecompileerde scripts.

```
/** 
 * Handler for Livefyre analytics batch events. 
 * @param {Array.<string>} events Array of events that have been fired since 
 * the last batch send. 
 */ 
function analyticsHandler(events) { 
  // Send to analytics 
  console.log(events); 
} 
 
var attempts = 0; 
 
function pollForAnalytics() { 
  if (Livefyre && Livefyre.analytics) { 
    Livefyre.analytics.addHandler(analyticsHandler); 
    return; 
  } 
  if (attempts === 10) { 
    return; 
  } 
  attempts++; 
  setTimeout(pollForAnalytics, 500); 
} 
 
pollForAnalytics(); 
```

## Stap 2: Handlerfunctie implementeren

Zodra de functionaliteit Livefyre.analytics op de pagina beschikbaar is, voer de analyticsHandler functie uit om de ontvangen gebeurtenissen naar de analytische leverancier van uw keus te verzenden.

1. De handler analytics ontvangt een array met gebeurtenissen die moeten worden doorlopen en afzonderlijk of als batch moeten worden verzonden, als uw provider dit ondersteunt.
1. Wijs de gebeurtenisgegevens toe die door de manager aan een formaat worden ontvangen dat uw analyseleverancier vereist.
1. Verzend de gegevens naar het analysebureau.
