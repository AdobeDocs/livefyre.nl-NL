---
description: De kernbibliotheek van Livefyre die wordt gebruikt om Livefyre op uw plaats aan te drijven.
seo-description: De kernbibliotheek van Livefyre die wordt gebruikt om Livefyre op uw plaats aan te drijven.
seo-title: Livefyre.js
solution: Experience Manager
title: Livefyre.js
uuid: 7b3eca57-d5e8-416d-badf-a9c51d10dadd
translation-type: tm+mt
source-git-commit: 67aeb3de964473b326c88c3a3f81ff48a6a12652

---


# Livefyre.js {#livefyre-js}

De kernbibliotheek van Livefyre die wordt gebruikt om Livefyre op uw plaats aan te drijven.

`Livefyre.js` Dit is de kernbibliotheek die u op elke LiveCycle-webpagina kunt installeren. Het definieert het algemene `window.Livefyre` object en één openbare methode, `Livefyre.require`die kan worden gebruikt om andere LiveCycle JavaScript-bibliotheken te laden die u helpen bij het [insluiten van LiveCycle Apps](/help/implementation/c-getting-started/c-implementation-process/c-using-livefyre.js-to-create-customize-and-use-apps-on-your-site.md), door uw verificatieprovider te [integreren met LiveCycle](/help/implementation/t-about-identity-integration/t-about-identity-integration.md) en meer.

## Toevoegen aan uw site {#section_cst_twg_xz}

Voeg de volgende `<script>` tag toe aan uw webpagina of websitesjabloon. Voeg het indien mogelijk toe aan de `<head>` sectie van uw HTML-document, zodat het snel wordt geladen.

```
<script src="//cdn.livefyre.com/Livefyre.js"></script>
```

>[!NOTE]
>
>Met dit script wordt een zeer klein bestand (~1 kB), genaamd Livefyre.js-scout, ingesloten dat vervolgens de nieuwste versie van Livefyre.js laadt via het protocol waarmee uw webpagina is geopend (HTTP of HTTPS).

## Livefyre.require {#section_ipq_hwg_xz}

`Livefyre.require` is een aangepaste JavaScript-modulelader, zoals [curl.js](https://github.com/cujojs/curl) of [RequireJS](https://requirejs.org/). Het kan worden gebruikt om de meeste pakketten te laden die door Livefyre worden gepubliceerd en biedt een handig en intuïtief integratiepad.

Pakketten die toegankelijk zijn via `Livefyre.require` een versienummer, zijn [semantische versiering](https://semver.org/). Pakketten kunnen in een specifieke versie of in een reeks versies worden vereist, zodat uw webpagina automatisch kan profiteren van de nieuwe functies voor foutopsporing. Dit biedt u flexibiliteit bij het integreren van Livefyre op uw site. Er zijn drie niveaus van versie die u kunt gebruiken met `Livefyre.require`.

* **package-name#1:** Vastzetten op hoofdversie v1. U ontvangt alle nieuwe updates die een achterwaarts compatibele API onderhouden. Vastzetten aan een belangrijke versie om insectenmoeilijke situaties en minder belangrijke eigenschapverhogingen voor die versie te ontvangen.
* **package-name#1.1:** Vastzetten op secundaire versie v1.1. Alle problemen worden in deze kleine versie opgelost. Met LiveCycle Engineering wordt altijd een kleine versie van een pakket geplaatst als het standaardgedrag of het functionele bereik zodanig verandert dat er nieuw, onverwacht gedrag op de webpagina kan optreden. Als u geautomatiseerde foutoplossingen wilt ontvangen, maar geen aanvullende functionaliteit of wijzigingen in standaardgedrag wilt toepassen, moet u deze vastzetten in een lagere versie.
* **package-name#1.1.1:** Vastzetten op patchversie v1.1.1. Het gedrag van deze insluiten verandert nooit, zelfs niet als er fouten zijn. Zet aan een flardversie als u uitgebreide CSS aanpassingen voor uw plaats hebt die van de de prijsverhogingsstructuur van een pakket afhangen die kan veranderen, of als u andere redenen hebt om te verkiezen dat de versie van de Levensstijl u loopt op geen enkele manier zal veranderen.

Een voorbeeldintegratie met behulp van `Livefyre.require` kan er als volgt uitzien:

```
<!-- First add Livefyre.js to the page --> 
<script src="https://cdn.livefyre.com/Livefyre.js"></script> 
  
<!-- Then load up all the desired Livefyre packages and Do Stuff in the callback --> 
<script> 
Livefyre.require([ 
    'lfawesome#1', 
    'lfsuperawesome#2.1.2' 
], function (LFAwesome, LFSuperAwesome) { 
    var greatness = new LFAwesome(); 
    // etc.. 
}); 
</script>
```

## Beschikbare pakketten {#section_ygd_dwg_xz}

Welke LiveCycle JavaScript-pakketten zijn beschikbaar via `Livefyre.require`? Hier vindt u altijd een bijgewerkte lijst met ondersteunde pakketten en de meest recente versies: [packages.html](https://cdn.livefyre.com/packages.html).

## Versies van pakketten die vooraf zijn uitgebracht testen {#section_pgm_dpg_xz}

Soms wilt u een volgende versie van een LiveCycle-pakket testen om ervoor te zorgen dat het op uw website werkt of om een functie die op uw verzoek wordt ontwikkeld, te accepteren. Naast het opnemen van een Semantische waaier van de Versie, kan het preUAT milieu worden gespecificeerd.

Hieronder vindt u bijvoorbeeld de UAT-release van `fyre.conv`, de toepassingen Opmerkingen, Live Blog en Chat.

```
Livefyre.require(['fyre.conv#uat'], callback); 
```