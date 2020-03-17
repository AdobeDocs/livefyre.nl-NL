---
description: Bouw Ping voor Pull reactie om bijgewerkte gebruikersinformatie naar Livefyre over te brengen.
seo-description: Bouw Ping voor Pull reactie om bijgewerkte gebruikersinformatie naar Livefyre over te brengen.
seo-title: De pingelen voor volledige reactie samenstellen
solution: Experience Manager
title: De pingelen voor volledige reactie samenstellen
uuid: f90871d5-601f-40dc-b3d2-ab78635e4a88
translation-type: tm+mt
source-git-commit: 74a63daa264014af9a8afb6639fa1561a7b83241

---


# De pingelen voor volledige reactie samenstellen{#build-the-ping-for-pull-response}

Bouw Ping voor Pull reactie om bijgewerkte gebruikersinformatie naar Livefyre over te brengen.

| Type | Eigenschap | Beschrijving |
|--- |--- |--- |
| Tekenreeks *vereist* | id | De gebruikersnaam van de gebruiker in uw profielsysteem. Dit moet uniek over alle gebruikers in uw Netwerk zijn, en moet nooit veranderen. |
| Tekenreeks *vereist* | display_name | De weergavenaam van de gebruiker. Dit wordt weergegeven met Livefyre-inhoud die door de gebruiker is gepost. |
| Object *optioneel, maar aanbevolen* | name | Tekenreeksen om de opgemaakte, eerste, middelste en achternaam van de gebruiker te definiëren. |
| Tekenreeks *optioneel, maar aanbevolen* | email | E-mailadres van gebruiker. Wordt gebruikt om e-mailmeldingen te verzenden. |
| Tekenreeks *optioneel, maar aanbevolen* | image_url | URL naar een avatar om voor de gebruiker te tonen. Met LiveCycle worden geüploade afbeeldingen geschaald naar 100×100, 75×75 of 50×50 pixels, al naargelang het geval. Voor de beste resultaten moeten gebruikers een vierkante afbeelding uploaden van 100×100 pixels. Om ervoor te zorgen dat de avatar-afbeelding wordt bijgewerkt in LiveCycle, wijzigt u de image_url voor elke afbeeldingsupdate, zodat Ping for Pull detecteert dat de afbeelding is gewijzigd. Voeg bijvoorbeeld een tijdstempel toe aan de bestandsnaam of vergroot de wijzigingen in de afbeelding. Opmerking:  Alle URL&#39;s moeten volledig zijn gekwalificeerd en toegankelijk zijn. |
| Tekenreeks *optioneel, maar aanbevolen* | profile_url | URL aan de de profielpagina van de gebruiker op uw plaats. |
| Tekenreeks *optioneel, maar aanbevolen* | settings_url | URL naar een pagina waarop gebruikers de profielinstellingen van de gebruiker voor uw site kunnen configureren. |
| Array *optioneel, maar aanbevolen* | tags | Wordt gebruikt om gebruikers toe te wijzen aan gebruikersgroepen. Tags kunnen 1-63 alfanumerieke tekens en onderstrepingstekens bevatten. |
| Boolean *optioneel, maar aanbevolen* | autofollow_conversations | Bepaalt of een gebruiker een Inzameling na het posten aan het automatisch wil volgen. Wanneer gebruikers een verzameling volgen, ontvangen ze e-mailmeldingen wanneer andere gebruikers deelnemen. Kan waar of onwaar zijn. Heeft als standaardwaarde true. |
| Object *optioneel, maar aanbevolen* | email_notifications | Definieert de frequentie van beschikbare e-mailmeldingen voor LiveCycle. Voor elk meldingstype kunnen verschillende frequenties worden ingesteld. Standaard worden geen meldingen verzonden. <br><ul><li> geeft onmiddellijk meldingen uit op de vermelde gebeurtenis. </li><li>geeft vaak meldingen in batches uit. </li><li> geen e-mailmelding voor de activiteit verzenden. </li><li>*opmerkingen*: Hiermee definieert u wanneer meldingen worden verzonden wanneer andere gebruikers inhoud plaatsen in verzamelingen die deze gebruiker volgt. </li><li>*antwoorden*: Definieert wanneer meldingen worden verzonden wanneer een andere gebruiker op de inhoud van deze gebruiker reageert.</li><li>*leuk*: Definieert wanneer meldingen worden verzonden wanneer een andere gebruiker de inhoud van deze gebruiker leuk vindt.</li><li>*moderator_comments*: Bepaalt wanneer de berichten worden verzonden naar moderators wanneer de gebruikers inhoud aan om het even welke Inzameling in het Netwerk posten.</li><li>*moderator_flags*: Bepaalt wanneer de berichten worden verzonden naar moderators wanneer andere gebruikers inhoud in om het even welke Inzameling in het Netwerk markeren.</li></ul> |
| Tekenreeks *optioneel* | locatie | Een door de gebruiker verzonden locatie. |
| Tekenreeks *optioneel* | bio | Een door de gebruiker ingediende autobiografie. |
| Array *optioneel* | websites | Een array van door de gebruiker ingediende sites. Max = 2. |
| Object *optioneel* | display_rules | Bepaalt welke profieleigenschappen openbaar zichtbaar aan andere gebruikers zijn. Elke beschikbare parameter neemt Booleaanse invoer waar of onwaar. Beschikbare parameters:  <br><ul><li>bio </li><li> locatie</li><li>  sekse </li><li>naamplaatje </li><li> remote_profile_url</li></ul> |
| Boolean *optioneel* | moderator | Bepaalt of de gebruiker moderatorvoorrechten over het netwerk heeft. |
| Boolean *optioneel* | gravatar_disabled | Bepaalt of om het gebruik van een gravatar van Livefyre onbruikbaar te maken als geen image_url wordt verstrekt. |

## Voorbeeld-reactie {#section_uxt_3dd_mz}

```
{
 "id": "1234567890",
 "display_name": "Bob Dole",
 "name": {
   "formatted": "Bob Joseph Dole",
   "first": "Bob",
   "middle": "Joseph",
   "last": "Dole"
 },
   "email": "bob@dole.com",
   "image_url": "https://dole.com/images/bob.jpg",
   "profile_url": "https://site.com/bobdole",
   "settings_url":"https://site.com/settings",
   "tags": ["bob", "dole"],
   "autofollow_conversations": "true",
   "email_notifications": {
      "comments": "never",
      "replies": "immediately",
      "likes": "often",
      "moderator_comments": "immediately",
      "moderator_flags": "immediately" 
 },
  "location": "Washington D.C., USA",
  "bio": "Bob Dole speaks in the third person",
  "websites": ["https://dole.com/blog/", "https://bobdolerocks.com"],
  "display_rules": {
      "bio": "false",
      "location": "false",
      "gender": "false",
      "name": "false",
      "image": "false",
      "remote_profile_url": "false"
  },
  "moderator": "true",
  "gravatar_disabled": "false"
}
```