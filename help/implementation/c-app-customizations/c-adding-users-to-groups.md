---
description: Voeg een gebruikerstag toe aan een account om een gebruiker aan een groep toe te voegen.
seo-description: Voeg een gebruikerstag toe aan een account om een gebruiker aan een groep toe te voegen.
seo-title: Gebruikers toevoegen aan groepen
solution: Experience Manager
title: Gebruikers toevoegen aan groepen
uuid: 3633f2df-8d60-4cdd-b9a2-3807218c74a0
translation-type: tm+mt
source-git-commit: 67aeb3de964473b326c88c3a3f81ff48a6a12652

---


# Gebruikers toevoegen aan groepen{#adding-users-to-groups}

Voeg een gebruikerstag toe aan een account om een gebruiker aan een groep toe te voegen.

De tags van de gebruiker kunnen voor zowel merkgebonden als ondernemingsprofielsystemen worden uitgevoerd, en kunnen aan rekeningen op verscheidene manieren worden toegevoegd:

* Als u eigenaars en moderatoren via Studio maakt, wordt de gebruikerstag Moderator aan de account toegewezen.
* Wanneer u gebruikersgroepen maakt en gebruikers aan deze groepen toevoegt via Studio, worden automatisch gebruikerstags met de naam van de groep toegepast op de geselecteerde gebruikers.
* De Markeringen van de gebruiker kunnen ook rechtstreeks op rekeningen worden toegepast gebruikend de [Add vraag van HTTP](https://api.livefyre.com/docs#add-user-tag) van de Markering van de Gebruiker, of Pingel voor Trek.

>[!NOTE]
>
>Beide API-methoden, de HTTP Add User Tag-aanroep en de Ping for Pull-methode, overschrijven alle tags die eerder aan de Account zijn toegewezen via andere methoden. Selecteer daarom één methode en gebruik deze consistent gedurende het hele proces.

## Voeg een gebruiker aan een Groep van de pagina van Gebruikers in Studio toe {#section_qgq_nbw_xz}

* Klik op **[!UICONTROL Add Group]** of het groeplabel onder een gebruikersnaam om het menu Groepen te openen.
* Blader door de lijst en zoek de groep waaraan u de gebruiker wilt toevoegen. U kunt een groepsnaam invoeren in het **[!UICONTROL Search]** vak boven aan het vervolgkeuzemenu.
* Klik op het selectievakje naast de groep(en) waaraan de gebruiker moet worden toegevoegd en klik op Enter.

In het gebruikersprofiel wordt de naam van de groep (als de gebruiker slechts in één groep is) of het aantal groepen weergegeven waartoe de gebruiker behoort.

## Een gebruiker toevoegen aan een groep met de aanroep Gebruikerstag toevoegen {#section_kn3_gbw_xz}

Geef de LFToken en de naam van de geselecteerde tag door aan de POST-aanvraag

Bijvoorbeeld:

```
curl -XPOST -d 'tag_name=tag&lftoken=eyJhbGciOiAiA_TOKENcGlyZXMiOiAxMzU3OTY3NTAxLjIzn0.KoyXUVCavt-rdvkVXm2qzQTyMAOSp-crQA1uL1ht9WU' 'https://labs.quill.fyre.co/api/v3.0/author/system@`labs.fyre.co`/tag/'
```


Zie API-naslaggids > [Gebruikerstag](https://api.livefyre.com/docs/apis/by-category/user-management#operation=urn:livefyre:apis:quill:operations:api:v3.0:author:tags:method=post)toevoegen voor meer informatie.

## Een gebruiker toevoegen aan een groep met Ping for Pull {#section_kyj_11w_xz}

Gebruik de array met tags om gebruikers toe te wijzen aan gebruikersgroepen. (Tags kunnen 1-63 alfanumerieke tekens en onderstrepingstekens bevatten.)

Bijvoorbeeld:

```
"tags": ["moderator", "brand_advocate"],
```

## Een gebruiker aan een groep toevoegen met externe profielen {#section_uyn_scv_xz}

Voeg gebruikerstags toe aan het externe profiel, waarmee gebruikersgegevens voor specifieke gebruikers worden gesynchroniseerd tussen het aangepaste profielsysteem en het LiveCycle.