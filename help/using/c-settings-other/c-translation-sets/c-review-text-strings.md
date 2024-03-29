---
description: De tekstreeksen aanpassen voor LiveRevisies.
title: Tekstreeksen controleren
exl-id: 82ced091-d573-4514-9b91-3451a94ed5d3
source-git-commit: 1d9088eecf797e1af881cb6be55b3c96284f75e5
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Tekstreeksen controleren{#review-text-strings}

De tekstreeksen aanpassen voor LiveRevisies.

Deze pagina bevat een overzicht en beschrijving van de tekenreeksen die beschikbaar zijn voor aanpassing in revisie-apps. De hier vermelde tekenreeksen komen bovenop en overschrijven voor de standaardtekenreeksen voor LiveCycle-kerntoepassingen, die worden vermeld in String Customizations. Waar duplicaten worden vermeld, zijn de tekenreeksen in deze tabellen de standaardinstelling voor revisieapps.

Implementatie
Revisie-/beoordelingsinterface
Stream-info
Informatie auteur/inhoud
Handelingen van gebruikers
Functies
Fouten

## Implementatie {#section-vsy-1k4-xz}

Als u deze functie wilt implementeren, geeft u een 1-1-objecttoewijzing van de tekenreeksen die u wilt overschrijven, door aan het Javascript-configuratieobject. Als u geen veld opgeeft, wordt de standaardtekst gebruikt.

Voorbeeld:

```
var customStrings = {
   postAsButton: "New Post As Text",
   postEditButton: "New Post Edit Text" };
networkConfig["strings"] = customStrings; fyre.conv.load(
   networkConfig,
   [convConfig],
   function(){}
);
```

## Revisie-/beoordelingsinterface {#section_iyv_zj4_xz}

Tekenreeksen beschikbaar voor de gebruikersinterface voor revisie en beoordeling.

| Element | Sleutel | Standaardtekst |
|--- |--- |--- |
| Knoppen | editReviewBtn | Revisie bewerken |
|  | reviewBtn | Revisie schrijven |
|  | beoordelingenGesloten | Revisies gesloten |
|  | showReviewBtn | Revisie tonen |
|  | volgen | Ik ben geïnteresseerd |
|  | shareText | Ik schreef net een revisie. Kijk eens! |
| Knopinfo voor classificaties | ratingValues | Een array. Standaard = `[‘Poor’, ‘Poor’, ‘Fair’, ‘Fair’, ‘Average’, ‘Average’, ‘Good’, ‘Good’, ‘Excellent’, ‘Excellent’]`; <br>Opmerking: Waarden in de array moeten worden gedupliceerd om aan de linker- en rechterhelft van elke ster dezelfde naam toe te wijzen. |
| Onderdelen van classificaties | ratingSubpartPlaceholders | Een array. Standaard = `[]` |
|  | ratingSubpartTitles | Een array. Standaard = `[]` |
|  | reviewStreamTitle | Standaard leeg. Titel van de samenvatting van de evaluatie. |
| Dic | averageRating | Gemiddelde beoordeling door gebruiker |
|  | breakHeader | Classificatie-indeling |
|  | nuttig | %s van %s is nuttig gevonden |
|  | NuttigePlural | %s van %s is nuttig gevonden |
|  | outOf | / |
|  | ratingType | ster |

## Stream-info {#section_wmv_yj4_xz}

Tekenreeksen beschikbaar voor informatie en weergave van de inhoudsstroom.

| Element | Sleutel | Standaardtekst |
|---|---|---|
| Sorteren | sortBy | Standaard leeg. |
|  | sortHighestRated | Hoogste beoordeling |
|  | sortLowestRated | Laagste classificatie |
|  | sortMostHelpful | Meeste handigheid |
| Stream misc. | showMore | Meer weergeven |
| Hoge snelheid streamen | newComment | Nieuwe revisie |
|  | newComments | Nieuwe revisies |
| Aantal listeners | listenerCount | persoon die luistert |
|  | listenerCountPlural | mensen luisteren |
| Aantal opmerkingen | commentCountLabel | LiveRevisies<strong> | </strong>%s |
|  | commentCountLabelPlural | LiveRevisies<strong> | </strong>%s |
| Telling van opmerkingenkennisgever | commentNotifier | Nieuwe revisie |
|  | commentNotifierPlural | Nieuwe revisies |

## Informatie auteur/inhoud {#section_osx_xj4_xz}

Stings beschikbaar voor auteur en individuele inhoudsinformatie.

| Element | Sleutel | Standaardtekst |
|---|---|---|
| Doorbraak van thread | reviewsContentNotFoundMsg | Deze revisie is niet meer zichtbaar |
|  | backToComments | Terug naar Revisies |

## Handelingen van gebruikers {#section_tlx_wj4_xz}

Tekenreeksen beschikbaar voor gebruikersacties: bestaande inhoud toewijzen, delen en markeren als handig.

| Element | Sleutel | Standaardtekst |
|---|---|---|
| Voettekst voor opmerkingen | wasReviewHelpful | Nuttig? |
|  | wasReviewHelpfulMobile | Nuttig? |
|  | ownIsReviewHelpful | Gevonden nuttig. |
|  | reviewIsHelpful | Ja |
|  | NuttigeScheider | &amp;vert; |
|  | reviewIsNotHelpful | Nee |
| Stemmen over modaal | voiceTitle | Was deze herziening nuttig? |
|  | stemmenDownloaden | Nee |
|  | voiceReplyTitle | Was dit antwoord nuttig? |
|  | voiceTitle | Was deze opmerking nuttig? |
|  | stemonthouding | Ja |
| Markering — modaal | flagTitle | Revisie van %s markeren |
|  | flagSuccessMsg | Revisie is gemarkeerd. |
| Markering mobiel | flagConfirmationMessage | Revisie van %s markeren als %s? |
| Meningmodaal | notifyDefaultText | Ik heb u in een Livefyre-revisie genoemd! |
| Delen, modaal | shareTitle | Revisie delen |

## Functies {#section_yl1_wj4_xz}

Tekenreeksen beschikbaar voor gebruikers die revisies plaatsen.

| Element | Sleutel | Standaardtekst |
|---|---|---|
| Editor | bodyPlaceholder | Revisie schrijven... |
|  | postEditButton | Bewerken |
|  | postEditCancelButton | Annuleren |
|  | postAsButton | Herziening achteraf als... |
|  | postButton | Na revisie |
|  | postReplyAsButton | Plaatsen als... |
|  | postReplyButton | Post |
|  | shareButton | Delen |
|  | titlePlaceholder | Titel... |

## Fouten {#section_jbc_vj4_xz}

Tekenreeksen beschikbaar voor algemene foutberichten.

| Element | Sleutel | Standaardtekst |
|---|---|---|
| Fouten | errorAlreadyPosted | Je kunt slechts één revisie plaatsen. |
|  | errorAuthError | U bent niet bevoegd om een revisie op dit gesprek te plaatsen |
|  | errorCommentsNotAllowed | Revisies kunnen op dit moment niet worden gepost |
|  | errorDislikeOwnComment | Je kunt je eigen beoordeling niet opheffen |
|  | errorDuplicate | U mag de revisie niet tweemaal plaatsen, wat u ook leuk vindt. |
|  | errorEditDuplicate | U moet de hoofdtekst van de revisie wijzigen wanneer u de revisie bewerkt. |
|  | errorEditNotAllowed | U bent niet gemachtigd revisies op dit gesprek te bewerken. |
|  | errorEditTimeExceeded | De revisiebewerkingsperiode is verlopen. |
|  | errorEmpty | Het lijkt erop dat u een lege revisie wilt plaatsen. |
|  | errorEmptyTitle | Het lijkt erop dat u een lege titel wilt plaatsen |
|  | errorFieldRating | sterrenwaardering |
|  | errorFieldReview | revisie |
|  | errorFieldTitle | titel |
|  | errorMaxChars | Je beoordeling is te lang. Bewerk het bestand en probeer het opnieuw. |
|  | errorMissingFields | Voer een |
|  | errorRatingEmpty | Je kunt geen lege beoordeling verzenden |
|  | errorRatingNotSet | Alle classificaties moeten worden ingesteld |
|  | errorRatingNotValid | De classificatie moet een object zijn |
|  | errorShowMore | Er is een fout opgetreden bij het laden van meer revisies. |
|  | errorTitleMaxChars | Je titel is te lang. Bewerk het bestand en probeer het opnieuw. |
|  | errorStemOwnComment | Je kunt niet op je eigen beoordeling stemmen |
