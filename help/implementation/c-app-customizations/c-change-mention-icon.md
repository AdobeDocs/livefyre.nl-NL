---
description: Wijzig het pictogram dat voor Livefyre-gebruikers wordt weergegeven in het vervolgkeuzemenu @mention.
title: Pictogram @mention wijzigen
exl-id: e078ef7f-7f16-4f5d-9152-95ae7fe7e4bd
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '83'
ht-degree: 18%

---

# Pictogram `@mention` wijzigen {#change-mention-icon}

Wijzig het pictogram dat wordt weergegeven voor Live-gebruikers in het keuzemenu `@mention`.

Wijzig het pictogram LiveCycle dat in het vervolgkeuzemenu `@mention` wordt gebruikt in een pictogram van uw keuze, zodat u de leden van de gebruikersgemeenschap kunt aangeven met uw eigen pictogram.

## Voorbeeld

Als u dit pictogram wilt wijzigen, voegt u de volgende CSS toe aan uw stijlpagina. Vervang &lt;*uw resource*> URL door de URL van de afbeelding die u hebt geselecteerd om de standaardbadge van de bibliotheek te vervangen.

```
.fyre-editor-container .fyre-editor-toolbar > .fyre-mention-menu .fyre-mention-item .fyre-mention-item-livefyre { 
    background: url(<your resource url>) no-repeat center; 
    background-position: 0px 0px; 
    background-size: 22px 22px; 
}
```
