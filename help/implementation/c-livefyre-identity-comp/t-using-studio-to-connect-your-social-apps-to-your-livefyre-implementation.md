---
description: Als u aanmelden via een sociaal netwerk wilt inschakelen, gebruikt u Studio om de referenties van uw sociale apps toe te voegen aan uw LiveCycle-integratie en past u de aanmeldingsmodus aan.
title: Studio gebruiken om uw sociale toepassingen te verbinden met uw LiveCycle-implementatie
exl-id: 2ccb9737-8c59-4c1d-93d3-61f913b3cdd6
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Studio gebruiken om uw sociale toepassingen te verbinden met uw LiveCycle-implementatie{#using-studio-to-connect-your-social-apps-to-your-livefyre-implementation}

Als u aanmelden via een sociaal netwerk wilt inschakelen, gebruikt u Studio om de referenties van uw sociale apps toe te voegen aan uw LiveCycle-integratie en past u de aanmeldingsmodus aan.

## Aanpassen van de Login Modal {#section_v4c_hv2_3z}

Met de aanmeldingsmodus kunt u de gegevens aanpassen die uw gebruikers zien wanneer ze zich aanmelden bij uw apps. U kunt het modale venster aanpassen.

* **Logo:** Upload een logo voor gebruik in uw aanmeldingsmodi.
* **Lettertypefamilie:** selecteer een lettertype dat overeenkomt met uw branding.
* **Brand Color:** Voer een hexadecimale kleur in die moet worden gebruikt voor specifieke tekst in het modaal.
* **Voorwaarden en bepalingen URL:** Voer de URL in voor de pagina Voorwaarden en bepalingen van uw bedrijf. Dit veld is vereist voor gebruik met LiveCycle Identity.

## Livefyre-id {#section_xxt_z52_3z} omzetten

U kunt vertaalsets voor tekstreeksen maken en wijzigen in LiveCycle Identity.

Zie Vertaalsets voor meer informatie over het gebruik van vertaalsets met LiveCycle Identity.

Zie Livefyre Identity voor meer informatie over de specifieke tekenreeksen die u kunt aanpassen voor LiveY Identity.

## Aanmelding inschakelen met e-mail {#section_dlv_wzt_bbb}

Gebruikers toestaan hun e-mailadressen te gebruiken om zich aan te melden bij en te communiceren met Apps op uw site.

Aanmelden met een native Livefyre-account inschakelen:

1. Navigeer naar **[!UICONTROL Integration Settings]** in LiveCyre Studio.
1. Schakel de schakeloptie **[!UICONTROL Enable Login with Email]** in op **[!UICONTROL On]**.

## Aanmelding inschakelen met een Facebook-account {#section_ph3_515_bbb}

Sluit uw Facebook-account aan op Livefyre zodat gebruikers hun Facebook-aanmeldingen kunnen gebruiken om te communiceren met Apps op uw site.

Aanmelden met een Facebook-account inschakelen:

1. Schakel de schakeloptie **[!UICONTROL Enable Login with Facebook]** in op **[!UICONTROL ON]**.

1. Voeg de **[!UICONTROL App ID]** en **[!UICONTROL App Secret]** van uw Facebook-app toe.

   Deze waarden worden vermeld in het dashboard voor Facebook-ontwikkelaars voor de app, beschikbaar op [https://developers.facebook.com/apps/](https://developers.facebook.com/apps/675503539257343/dashboard/).

## Aanmelden met Google {#section_fq3_kb5_bbb} inschakelen

Sluit uw Google+-account aan op Livefyre zodat gebruikers hun Google+-aanmeldingen kunnen gebruiken om te communiceren met Apps op uw site.

Aanmelden met een Google+-account inschakelen:

1. Schakel de schakeloptie **[!UICONTROL Enable Login with Google]** in op **[!UICONTROL ON]**.

1. Voeg de **[!UICONTROL Client ID]** en **[!UICONTROL Client secret]** van uw Google-app toe.

   Deze waarden worden vermeld in uw projectinterface van het Platform van Google Cloud, beschikbaar bij [https://console.cloud.google.com/](https://console.cloud.google.com/apis/library). Om deze informatie terug te winnen, ga naar **[!UICONTROL API Manager > Credentials]**, en klik de projectnaam.

## Aanmelden met een Twitter-account {#section_iyz_wb5_bbb} inschakelen

Sluit uw Twitter-account aan op Livefyre zodat gebruikers hun Twitter-aanmeldingen kunnen gebruiken om te communiceren met Apps op uw site.

Aanmelden met een Twitter-account inschakelen:

1. Schakel de schakeloptie **[!UICONTROL Enable Login with Twitter]** in op **[!UICONTROL ON]**.

1. Voeg de **[!UICONTROL Consumer Key (API Key)]** en **[!UICONTROL Consumer Secret (API Secret)]** van uw Twitter-app toe.

   Deze waarden worden vermeld op de pagina **[!UICONTROL Keys and Access Tokens]** van uw Twitter-app, beschikbaar op [https://apps.twitter.com/](https://apps.twitter.com/).

## Aanmelding inschakelen met een Yahoo! Account {#section_s1q_3c5_bbb}

Verbind uw Yahoo! account aan Livefyre om gebruikers toe te staan hun Yahoo te gebruiken! meldt zich aan om te communiceren met Apps op uw site.

Aanmelden met een Yahoo inschakelen! account:

1. Schakel de schakeloptie **[!UICONTROL Enable Login with Yahoo!]** in op **[!UICONTROL ON]**.

1. Voeg je Yahoo toe! **[!UICONTROL Client ID]** en **[!UICONTROL Client Secret]**.

   Deze waarden staan in Yahoo! pagina met toepassingsdetails, beschikbaar via [developer.yahoo.com/apps](https://developer.yahoo.com/apps).

## Aanmelding inschakelen met een Microsoft Live-account {#section_z42_4c5_bbb}

Sluit uw Microsoft Live-id-account aan op LiveCycle zodat gebruikers hun Microsoft Live-id-aanmeldingen kunnen gebruiken voor interactie met Apps op uw site.

Aanmelden met een Microsoft Live ID-account inschakelen:

1. Schakel in **[!UICONTROL Livefyre > Integration Settings > Livefyre Identity > Microsoft Live]** de schakeloptie **[!UICONTROL Enable Microsoft Live Login]** in op **[!UICONTROL On]**.

1. Voer de **[!UICONTROL Microsoft Live Client ID (Private Key)]** en **[!UICONTROL Microsoft Live Client Secret (Password)]** in.

1. Klik op **[!UICONTROL Save Settings]**.

   De waarden **[!UICONTROL Microsoft Live Client ID (Private Key)]** en **[!UICONTROL Microsoft Live Client Secret (Password)]** worden weergegeven op de pagina met details voor de Microsoft Live-id-toepassing.

## Sluit uw sociale toepassingen aan Levensmiddelenidentiteit {#section_on2_vc5_bbb} aan

Laat uw gebruikers toe om uw implementatie van de Identiteit van het Leven voor apps op uw plaats te gebruiken.

1. Maak een app.
1. Ga naar **[!UICONTROL Studio]** > **[!UICONTROL Settings]** > **[!UICONTROL Integration Settings]**> **[!UICONTROL Livefyre Identity]**.

1. Voer de vereiste App-referenties in voor de app die u hebt gemaakt.
