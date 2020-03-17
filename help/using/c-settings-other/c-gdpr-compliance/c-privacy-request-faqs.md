---
description: Antwoorden op Veelgestelde vragen (FAQs) over GDPR-Klaar de Verzoeken van de Privacy.
seo-description: Antwoorden op Veelgestelde vragen (FAQs) over GDPR-Klaar de Verzoeken van de Privacy.
seo-title: Veelgestelde vragen over privacyverzoeken
solution: Experience Manager
title: Veelgestelde vragen over privacyverzoeken
uuid: 0cd6f0d2-504d-46e9-ac46-070536cda086
translation-type: tm+mt
source-git-commit: 67aeb3de964473b326c88c3a3f81ff48a6a12652

---


# Veelgestelde vragen over privacyverzoeken{#privacy-request-faqs}

Antwoorden op Veelgestelde vragen (FAQs) over GDPR-Klaar de Verzoeken van de Privacy.

* **Hoe kunnen bezoekers van de site ervoor kiezen niet te worden bijgehouden op een site die gebruikmaakt van LiveCycle Apps?** Wanneer een sitebezoeker het programma uitschakelt, moet de implementatie van de klant bij LiveCycle aangeven dat de gebruiker het programma heeft uitgeschakeld voordat een app wordt gemaakt. Livefyre heeft een manier gecreeerd om dit met de optie te doen JavaScript, `userPrivacyOptOut`. Zie `userPrivacyOptOut`userPrivacyOptOut voor meer informatie over het gebruik [ervan](/help/using/c-settings-other/c-gdpr-compliance/c-userprivacyoptout.md).

   Als de `userPrivacyOptOut` markering is ingesteld op true, verzendt Apps op de pagina geen gegevens naar LiveCycle-servers met behulp van cookies of een andere methode. De lokale opslag wordt dan niet bijgewerkt met gegevens die kunnen worden gebruikt om bezoekers van de site bij te houden. Als een bron geen volmacht steunt, dan toont Livefyre een masker op de inhoud tenzij een gebruiker op de video klikt en het potentiële volgen van die bron goedkeurt.

   Als u LiveCycle Identity gebruikt, kunnen gebruikers ervoor kiezen om hun profiel te verwijderen of een rapport te maken met gegevens die voor hun gebruikersaccount worden bijgehouden.

* **Hoe kan ik voorkomen dat ik toekomstige inhoud verzamel van een bezoeker van de site die ervoor gekozen heeft?** Gebruik deze optie `userPrivacyOptOut` met `livefyre.js` op een webpagina die LiveCycle Apps gebruikt. Zie `userPrivacyOptOut`userPrivacyOptOut voor meer informatie [](/help/using/c-settings-other/c-gdpr-compliance/c-userprivacyoptout.md).

* **Hoe kan ik een rapport genereren en de gegevens voor App-gebruikers of eigenaars van sociale accounts verwijderen?** Met [privacyverzoeken](../../c-settings-other/c-gdpr-compliance/c-privacy-requests.md#c_privacy_requests) kunt u een rapport genereren en gebruikersgegevens verwijderen uit Apps.

* **Hoe verwijder ik alle inhoud voor een bezoeker?** Livefyre houdt geen permanente informatie bij over sitebezoekers, behalve in de vorm van cookies om deze op unieke wijze te identificeren voor Livecount-functies. Livecount is een tijdelijk en realtime aantal bezoekers op de site. Er blijft geen geschiedenis behouden nadat de bezoeker cookies verlaat of wist.

   Maak een [privacyverzoek](../../c-settings-other/c-gdpr-compliance/c-privacy-requests.md#c_privacy_requests) om het account te verwijderen. LiveCycle verwijdert of maakt het gebruikersprofiel en de bijbehorende records anoniem.

* **Hoe verwijder ik inhoud voor een geregistreerde gebruiker?** Maak een [privacyverzoek](../../c-settings-other/c-gdpr-compliance/c-privacy-requests.md#c_privacy_requests) om het account te verwijderen. Het gebruikersprofiel en de bijbehorende records worden volledig vernietigd.

   >[!NOTE]
   >
   >Deze handeling kan niet ongedaan worden gemaakt.

* **Hoe kan ik een rapport opstellen met gegevens die worden bijgehouden van een huidige of voormalige werknemer?** Een privacyrapport [](../../c-settings-other/c-gdpr-compliance/c-view-a-privacy-report.md#c_view_a_privacy_report) weergeven om een rapport te genereren met gegevens die voor een gebruikersaccount zijn bijgehouden.

* **Voldoet Livefyre social stream?** Wanneer een gebruiker een bericht of tweet verwijdert uit het sociale netwerk, wordt de inhoud binnen 24 uur ook verwijderd uit alle bronnen in LiveCycle. Dit geldt voor Twitter en Facebook.
