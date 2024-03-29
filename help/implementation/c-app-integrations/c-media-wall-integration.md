---
description: Maak een mediamuur met inhoud die in real-time wordt gestreamd.
title: Mediumwand
exl-id: 597af7e1-9ada-4893-9071-e17c21ef0d04
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# Media Wall{#media-wall}

Maak een mediamuur met inhoud die in real-time wordt gestreamd.

Met Media Wall kunt u een real-time sociale muur voor uw site maken. Met het stroomnet-wallpakket van de Livefyre JavaScript SDK kunt u Livefyre sociale feeds weergeven als een visueel aantrekkelijke, volledig-schermvullende, naast elkaar geplaatste inhoud die ideaal is voor het behandelen van live gebeurtenissen, het ontvangen van fotowedstrijden en het aansturen van sociale gedeelten van uw website.

## Integratie {#section_jfm_bwb_c1b}

De snelste manier om een Muur van Media toe te voegen is de ingebouwde versie te gebruiken die op CDN van Livefyre wordt ontvangen.

Voeg eerst [Livefyre.js](https://github.com/Livefyre/Livefyre.js) toe aan uw site.

```
<script src="//cdn.livefyre.com/Livefyre.js"></script> 
```

Plaats vervolgens het element waarin de mediamuur wordt weergegeven.

```
<div id="wall"></div>
```

Tot slot gebruik `Livefyre.require` om de component te construeren.

```
<script> 
Livefyre.require([ 
    'streamhub-wall#5' 
], function(MediaWall) {     
    var wall = window.wall = new MediaWall({ 
        el: document.getElementById("wall"), 
        collection: { 
            "network": "client-solutions.fyre.co", 
            "siteId": "364309", 
            "articleId": "answers-mediawall" 
        } 
    }); 
}); 
</script>
```

U hebt nu een muur! Zie dit alles in actie in [dit voorbeeld](https://codepen.io/gobengo/pen/dFwDL).

**Is er een fout opgetreden?** Controleer of u de juiste omgevingsparameter doorgeeft. U kunt kiezen uit `livefyre.com` (productie) of `t402.livefyre.com` (UAT).

>[!NOTE]
>
>Om het even welke het stileren aanpassing van Tweets die door uw Muur App van Media worden teruggegeven moet worden gedaan in overeenstemming met de [Vereisten van de Vertoning ](https://dev.twitter.com/terms/display-requirements) van Twitter.

## Configuratieopties {#section_ucv_qvb_c1b}

`columns`

Staat u toe om het aantal kolommen voor uw Muur van Media te bepalen wanneer het construeren van uw muur. Als deze optie wordt geplaatst, zal de breedte van elke kolom automatisch aan de de containergrootte van de Muur van Media aanpassen, terwijl het handhaven van het gespecificeerde aantal kolommen.

```
var wallView = new MediaWall({ 
    el: document.getElementById('wall'), 
    columns: 5 
});
```

`initial`

Het aantal inhoudsitems dat moet worden gerenderd bij het laden van de pagina. De standaardwaarde is 50.

```
var wallView = new MediaWall({ 
   el: document.getElementById('wall'), 
   initial: 10 
});
```

`minContentWidth`

Staat u toe om de minimumbreedte (pixel) voor elke kolom binnen het de containerelement van de Muur van Media te plaatsen. (Uw Muur van Media zal automatisch een aangewezen aantal kolommen, afhankelijk van de breedte van zijn containerelement selecteren. Standaard bepaalt de breedte van de mediamuur gedeeld door de minimale breedte van de inhoud (300 px, indien ongedefinieerd) het aantal kolommen.)

>[!NOTE]
>
>Gebruik deze optie niet in combinatie met de optie Kolommen.

```
var wallView = new MediaWall({ 
    el: document.getElementById('wall'), 
    minContentWidth: 300 
});
```

`modal`

Als er bijlagen voor een stuk inhoud zijn, wordt standaard een klikbare miniatuur weergegeven in de mediaschalen. Wanneer op de app wordt geklikt, wordt een modaal met de volledige foto-/videobijlage geopend. Als u deze optie wilt uitschakelen, stelt u modal in op false.

```
var wallView = new MediaWall({ 
    el: document.getElementById('wall'), 
    columns: 5, 
    modal: false 
});
```

`postButton`

Bepaalt [!UICONTROL Post Content] knoop om op uw Muur te verschijnen. Deze optie vereist dat u `opts.collection` doorgeeft, en een integratie Livefyre.js Auth aan de pagina toevoegt.

`postButton` parameters:

* `false` (standaard): Geen knop Inhoud plaatsen tonen. (Hiermee maakt u een alleen-lezen mediamuur.)
* `true` (of  `LiveMediaWall.postButtons.contentWithPhotos`): Neem een knop op waarmee gebruikers tekstinhoud kunnen toevoegen aan gekoppelde foto&#39;s.

* `LiveMediaWall.postButtons.content`: Neem een knop op waarmee gebruikers tekstinhoud kunnen toevoegen, maar geen foto&#39;s kunnen bijvoegen.
* `LiveMediaWall.postButtons.photo`: Neem een knop op waarmee gebruikers een foto kunnen toevoegen, maar geen tekst.

```
var wallView = new MediaWall({ 
    el: document.getElementById('wall'), 
    collection: collection, 
    postButton: true, 
    minContentWidth: 300 
});
```

`showMore`

Bepaalt het aantal punten van de Inhoud om aan de muur toe te voegen wanneer uw [!UICONTROL Show More] knoop wordt geklikt.

```
var wallView = new LiveMediaWall({ 
    el: document.getElementById('wall'), 
    showMore: 10 
});
```

## Opties voor opmaakconfiguratie {#section_ztv_dvb_c1b}

De Muur van media biedt ook verscheidene configuratieopties aan die u toestaan om tekstkleur, stijl, en grootte aan te passen. Gebruik de volgende syntaxis om deze opties te implementeren:

```
var wall2 = window.wall2 = new MediaWall({ 
   el: document.getElementById("listView1"), 
   collection: collection, 
   cardBackgroundColor: '#333', 
   textColor: 'magenta', 
   linkColor: 'orange', 
   footerTextColor: 'lime', 
   displayNameColor: 'cyan', 
   usernameColor: 'red', 
   fontFamily: 'Helvetica, Arial', 
   linkAttachmentBackgroundColor: '#555', 
   linkAttachmentBorderColor: '#888' 
}); 
```

Voor geldige invoer raadpleegt u de W3C-standaarden voor CSS [Fontfamilie](https://www.w3.org/TR/CSS2/fonts.html#propdef-font-family), [Fontgrootte](https://www.w3.org/TR/CSS2/fonts.html#font-size-props), [Lijnhoogte,](https://www.w3.org/TR/CSS2/visudet.html#propdef-line-height) en [Kleur](https://www.w3.org/TR/css3-color/#colorunits) eigenschappen.

* **bodyFontSize** *(CSS Font Size String)* De tekengrootte voor de hoofdtekst van de inhoud.

* **bodyLineHeight** *(CSS Line Height String)* De regelhoogte voor hoofdtekst van inhoud.

* **buttonActiveBackgroundColor** *(CSS Color String)** The color for the button background on active.

* **buttonBorderColor** *(CSS Color String)** De kleur voor knopranden.

* **buttonHoverBackgroundColor** *(CSS Color String)* De kleur voor de knopachtergrond bij aanwijzen.

* **buttonTextColor** *(CSS Color String)* De kleur voor de knoplabels.

* **cardBackgroundColor** *(CSS Color String)* De achtergrondkleur voor inhoudskaarten in de mediamuur.

* **displayNameColor** *(CSS Color String)* De kleur voor weergavenamen in de byline.

* **fontFamily** *(CSS Font Family String)* De lettertypefamilie voor platte tekst.

* **footerTextColor** *(CSS het Koord van de Kleur)* De kleur voor secundaire teksten (zoals de footer tekst, en de gebruikersbenaming in de byline).

* **linkAttachmentBackgroundColor** *(CSS Color String)* De achtergrondkleur voor koppelingsbijlagen (gestapelde bijlagen).

* **linkAttachmentBorderColor** *(CSS Color String)* De randkleur voor koppelingsbijlagen (gestapelde bijlagen).

* **linkAttachmentTextColor** *(CSS Color String)* De kleur voor koppelingstekst.

* **linkColor** *(CSS Color String)* De kleur voor hyperlinks (zoals koppelingen in hoofdtekst en koppelingen voor weergavenamen).

* **textColor** *(CSS Color String)* De kleur voor platte tekst.

* **titleFontSize** *(CSS Font Size String)* The font size for content titles.

* **titleLineHeight** *(CSS Line Height String)* De regelhoogte voor titels van inhoud.

* **sourceLogoColor** *(CSS Color String)* De kleur voor het bronlogo.

* **usernameColor** *(CSS Color String)* The color for the usernames in the byline.
