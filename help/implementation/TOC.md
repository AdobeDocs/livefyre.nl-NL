---
product: livefyre
audience: end-user
user-guide-title: Implementatiehandleiding voor Livefyre
translation-type: tm+mt
source-git-commit: 3664bc1c51d2b372c358385127a1ca9c2f0cfef8
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---


# Handleiding voor implementatie van Livefy {#implementation}

+ [Implementatiehandleiding voor Livefyre](home.md)
+ Aan de slag {#getting-started}
   + [Aan de slag met Livefyre-integratie](c-getting-started/c-getting-started.md)
   + Implementatieproces {#implementation-process}
      + [Implementatieproces](c-getting-started/c-implementation-process/c-implementation-process.md)
      + [Toepassingsintegratietypen](c-getting-started/c-implementation-process/c-app-integration-types.md)
      + [Toepassingsimplementatie](c-getting-started/designer-app-implementation.md)
      + [Livefyre implementeren met integratie van derden](c-app-integrations/implement-livefyre-3rd-party.md)
      + [Architectuur](c-getting-started/c-implementation-process/c-architecture.md)
      + [Een app insluiten](c-getting-started/c-implementation-process/c-using-livefyre.js-to-create-customize-and-use-apps-on-your-site.md)
      + [Verificatie toevoegen aan een app met Livefyre.js](c-getting-started/c-implementation-process/c-add-authetication-to-an-app-using-livefyre.js.md)
      + [Server-zijtokens maken](c-getting-started/c-implementation-process/c-build-server-side-tokens.md)
      + [CollectionMeta-token](c-getting-started/c-implementation-process/c-collectionmeta-tokent.md)
      + [Token van auteur](c-getting-started/c-implementation-process/c-user-auth-token.md)
      + [Creeer een Inzameling gebruikend de Token CollectionMeta](t-create-a-collectionmeta-token.md)
      + [Checksum maken](c-creating-a-checksum.md)
+ Identiteitsintegratie {#identity-integration}
   + [Identiteitsintegratie](t-about-identity-integration/t-about-identity-integration.md)
   + [Verificatiepakket](t-about-identity-integration/c-authorization-package.md)
   + [Object AuthDelegate](t-about-identity-integration/c-building-an-auth-delegate.md)
   + [Gebruikersmachtigingen naar externe systemen posten (optioneel)](t-about-identity-integration/c-posting-user-permissions-to-external-systems.md)
   + SSO {#implementing-sso} implementeren
      + [Implementatie van SSO](t-about-identity-integration/c-implementing-sso/c-implementing-sso.md)
      + [Foutopsporing Auth Delegate](t-about-identity-integration/c-implementing-sso/c-debugging-auth.md)
   + Synchroniseren met LiveCycle {#sync-ping-for-pull}
      + [Synchroniseren met Livefyre Ping for Pull gebruiken](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/t-sync-with-livefyre-using-ping-for-pull.md)
      + [Het eindpunt van de trek opbouwen](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/t-build-the-pull-endpoint.md)
      + [Registreer het Eindpunt met Studio](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/c-register-the-endpoint-with-studio.md)
      + [Pingelen samenstellen](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/t-build-the-ping.md)
      + [Pull Request Structure](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/t-pull-request-structure.md)
      + [De pingelen voor volledige reactie samenstellen](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/c-build-the-ping-for-pull-response.md)
+ Livefyre-id {#livefyre-identity}
   + [Livefyre-id](c-livefyre-identity-comp/c-livefyre-identity-comp.md)
   + [LiveCycle-identiteit inschakelen](c-livefyre-identity-comp/t-enable-livefyre-identity.md)
   + Sociale toepassingen gebruiken met levende identiteit {#use-social-apps-with-livefyre-identity}
      + [Uw sociale apps maken](c-livefyre-identity-comp/t-create-your-social-apps.md)
      + [Een Facebook-app maken voor gebruik met LiveCyre-id](c-livefyre-identity-comp/t-create-a-facebook-app-for-use-with-livefyre-identity.md)
      + [Een Twitter-app maken voor gebruik met LiveCyre-identiteit](c-livefyre-identity-comp/t-create-a-twitter-app-for-use-with-livefyre-identity.md)
      + [Maak een Yahoo! App voor gebruik met LiveCyre-identiteit](c-livefyre-identity-comp/t-create-a-yahoo-app-for-use-with-livefyre-identity.md)
      + [Een Microsoft Live Identity-app maken voor gebruik met LiveCyre-identiteit](c-livefyre-identity-comp/t-create-a-microsoft-live-id-app-for-use-with-livefyre-identity.md)
      + [Een LinkedIn-toepassing maken voor gebruik met LiveCycle-identiteit](c-livefyre-identity-comp/t-create-a-linkedin-app-for-use-with-livefyre-identity.md)
      + [Een GitHub Identity-app maken voor gebruik met LiveCyre-identiteit](c-livefyre-identity-comp/c-create-a-github-identity.md)
      + [Studio gebruiken om uw sociale toepassingen te verbinden met uw LiveCycle-implementatie](c-livefyre-identity-comp/t-using-studio-to-connect-your-social-apps-to-your-livefyre-implementation.md)
   + [Livefyre.js toevoegen aan de pagina](c-livefyre-identity-comp/t-add-livefyre.js-to-the-page.md)
   + [Livefyre-identiteit initialiseren](c-livefyre-identity-comp/t-initialize-livefyre-identity.md)
   + [E-mails voor identiteit LiveCycle](c-livefyre-identity-comp/c-emails-for-livefyre-identity.md)
   + [Janrain Capture/Backplane](c-livefyre-identity-comp/c-janrain-capture-backplane-comp.md)
   + Installatie {#installation}
      + [Bibliotheken installeren](c-installing-libraries/c-installing-libraries.md)
      + [Klassen en methoden](c-installing-libraries/c-methods-livefyre.md)
      + [Netwerkmethoden](c-installing-libraries/c-network-methods.md)
      + [setSSL-netwerkmethode](c-installing-libraries/r-setssl-method.md)
      + [buildLivefyreToken, netwerkmethode](c-installing-libraries/r-buildlivefyretoken-method.md)
      + [buildUserAuthToken Netwerkmethode](c-installing-libraries/r-builduserauthtoken-method.md)
      + [validateLivefyreToken Netwerkmethode](c-installing-libraries/c-validatelivefyretoken-network-method.md)
      + [setUserSyncUrl Netwerkmethode](c-installing-libraries/r-setusersyncurl-method.md)
      + [syncUser-netwerkmethode](c-installing-libraries/r-syncuser-method.md)
      + [getUrn-netwerkmethode](c-installing-libraries/r-geturn-method.md)
      + [getUrnForUser Netwerkmethode](c-installing-libraries/r-geturnforuser-method.md)
      + [getNetworkName Netwerkmethode](c-installing-libraries/r-getnetworkname-method.md)
      + [getSite-netwerkmethode](c-installing-libraries/r-getsite-method.md)
      + [Methoden van de netwerkklasse](c-installing-libraries/c-network-class-methods.md)
      + [Methoden van de klasse Collection](c-installing-libraries/c-collection-methods.md)
      + [createOrUpdate Collection Method](c-installing-libraries/r-createorupdate-collection-method.md)
      + [buildCollectionMetaToken Collection Method](c-installing-libraries/r-buildcollectionmetatoken-collection-method.md)
      + [buildChecksum-verzamelingsmethode](c-installing-libraries/r-buildchecksum-collection-method.md)
      + [getCollectionContent Collection, methode](c-installing-libraries/t-getcollectioncontent-collection-method.md)
      + [getUrn, verzamelingsmethode](c-installing-libraries/r-geturn-collection-method.md)
      + [Methoden van de klasse Site](c-installing-libraries/c-site-methods.md)
      + [Site-methode buildBlogCollection](c-installing-libraries/r-buildblogcollection-site-method.md)
      + [Site-methode buildChatCollection](c-installing-libraries/r-buildchatcollection-site-method.md)
      + [buildCommentsCollection-sitemethode](c-installing-libraries/r-buildcommentscollection-site-method.md)
      + [buildCountingCollection-sitemethode](c-installing-libraries/r-buildcountingcollection-site-method.md)
      + [buildRatingsCollection-sitemethode](c-installing-libraries/r-buildratingscollection-site-method.md)
      + [Site-methode buildReviewsCollection](c-installing-libraries/r-buildreviewscollection-site-method.md)
      + [Site-methode buildSitenotesCollection](c-installing-libraries/r-buildsitenotescollection-site-method.md)
      + [Site-methode buildCollection](c-installing-libraries/r-buildcollection-site-method.md)
      + [getUrn-sitemethode](c-installing-libraries/r-geturn-site-method.md)
      + [Voorbeelden](c-installing-libraries/c-libraries-examples.md)
   + Mobiele SDK&#39;s {#mobile-sdks}
      + [Mobiele SDK&#39;s](c-mobile-sdks/c-mobile-sdks.md)
      + [Livefyre iOS SDK](c-mobile-sdks/c-livefyre-ios-sdk.md)
      + [Android-SDK](c-mobile-sdks/c-android-sdk.md)
+ [Livefyre.js](c-livefyre.js.md)
+ [Livefyre Tokens maken C#](c-creating-livefyre-tokens-c-.md)
+ Toepassingsintegratie {#app-integrations}
   + [Chat](c-app-integrations/c-app-integratios-chat.md)
   + Opmerkingen {#comments}
      + [Opmerkingen](c-app-integrations/c-comments-integration/c-comments-integration.md)
   + [Live blog](c-app-integrations/c-live-blog-integration.md)
   + [Revisies](c-app-integrations/c-reviews-integration.md)
   + Sidenotes {#sidenotes}
      + [Sidenotes-integratie](c-app-integrations/c-sidenotes-integration/r-sidenotes-integration.md)
      + [Symbolen toevoegen aan een pagina](c-app-integrations/c-sidenotes-integration/r-adding-sidenotes-to-a-page.md)
      + [Sidenotes App Events](c-app-integrations/c-sidenotes-integration/r-app-events.md)
      + [Opties voor Sidenotes-configuratie](c-app-integrations/c-sidenotes-integration/r-configuration-options.md)
      + [Aangepaste stijlen voor markeringen](c-app-integrations/c-sidenotes-integration/r-custom-styles.md)
      + [Aangepaste strings](c-app-integrations/c-sidenotes-integration/r-custom-strings.md)
      + [Sidenotes-implementatie](c-app-integrations/c-sidenotes-integration/r-sidenotes-implementation.md)
      + [Methode updateAnchors](c-app-integrations/c-sidenotes-integration/update-anchors-method.md)
   + [Kaart](c-app-integrations/c-map-integration.md)
   + [Mediumwand](c-app-integrations/c-media-wall-integration.md)
   + [Trend](c-app-integrations/c-trending-integration.md)
+ Toepassingsaanpassingen {#app-customizations}
   + [Toepassingsaanpassingen](c-app-customizations/c-app-customizations.md)
   + [Weergaveopties wijzigen](c-app-customizations/c-change-display-options.md)
   + [CSS-klassen](c-app-customizations/c-css-classes.md)
   + [CSS-klassen stabiliseren](c-app-customizations/c-storify-css-classes.md)
   + [Vertaalsets](c-app-customizations/c-translation-sets.md)
   + [Het Livefyre-logo verplaatsen](c-app-customizations/c-move-the-livefyre-logo.md)
   + [Media beperken](c-app-customizations/c-restrict-media.md)
   + [App Elements verbergen](c-app-customizations/c-hide-app-elements.md)
   + [Pictogram @mention wijzigen](c-app-customizations/c-change-mention-icon.md)
   + [Inhoud markeren](c-app-customizations/c-highlight-content.md)
   + [De datum- en tijdstempel aanpassen](c-app-customizations/c-date-time-stamp.md)
   + Inhoud element {#feature-content}
      + [Inhoud onderdeel](c-app-customizations/t-feature-content.md)
      + [Functie-inhoud in Studio inschakelen](c-app-customizations/t-enable-featuring-content-in-studio.md)
      + [Selecteer inhoud die u wilt gebruiken in een app](c-app-customizations/t-select-content-to-feature.md)
      + [Inhoud uit Studio selecteren voor functionaliteit](c-app-customizations/t-select-content-to-feature-from-studio.md)
      + [CSS gebruiken om aanbevolen inhoud op te maken](c-app-customizations/c-use-css-to-style-featured-content.md)
      + [Functie-API&#39;s](c-app-customizations/c-feature-apis.md)
   + [Janrain verbinden met Livefyre met gebruik van AuthDelegate](c-app-customizations/c-connecting-janrain-to-livefyre-using-authdelegate.md)
   + [Geaggregeerde aanbevolen inhoud met de aanbevolen API&#39;s](c-app-customizations/c-aggregated-featured-content-using-the-featured-apis.md)
   + Stijlinhoud {#style-content}
      + [Inhoud gebruikersgroep opmaken](c-app-customizations/c-style-user-group-content.md)
      + [Gebruikers toevoegen aan groepen](c-app-customizations/c-adding-users-to-groups.md)
   + Aangepaste stijlen toepassen {#apply-custom-styles}
      + [Aangepaste stijlen toepassen](c-app-customizations/c-applying-custom-styles-.md)
      + [Aangepaste knoppen toevoegen](c-app-customizations/t-add-custom-buttons.md)
   + JavaScript-gebeurtenissen {#javascript-events}
      + [Definities en voorbeelden van JavaScript-gebeurtenissen](c-app-customizations/c-javascript-events.md)
      + [Javascript-gebeurtenissen voor visualisatie-apps](c-app-customizations/c-javascript-events-for-visualization-apps.md)
      + [Javascript-gebeurtenissen voor mediamuur](c-app-customizations/c-javascript-events-media-wall.md)
      + [Javascript-gebeurtenissen voor conversie-apps](c-app-customizations/c-javascript-events-for-conversation-apps.md)
   + [Een app voor opmerkingen insluiten](c-app-customizations/c-embed-a-comments-app.md)
   + [Verwijzing bijhouden](c-app-customizations/c-referral-tracking.md)
   + [Apparaat- en browserondersteuning](c-app-customizations/c-device-and-browser-support.md)
   + [Vereisten voor Twitter-weergave](c-app-customizations/c-twitter-display-requirements.md)
+ [Testbeleid voor stress](c-stress-test-policy.md)
+ Analyse {#analytics}
   + [Analyse](livefyre-analytics/livefyre-analytics.md)
   + [LiveCycle gebruiken met Adobe Analytics en Dynamic Tag Manager (DTM)](livefyre-analytics/c-use-livefyre-with-adobe-analytics.md)
   + [LiveCycle gebruiken met Ander Analyseprogramma](livefyre-analytics/c-livefyre-analytics.md)
   + [Gebeurtenissen van Livefyre Analytics](livefyre-analytics/c-livefyre-analytics-events.md)
+ [LiveCycle integreren met AEM](c-livefyre-aem-integration.md)
+ Geavanceerde onderwerpen {#advanced-topics}
   + [Aantal opmerkingen weergeven](c-advanced-topics/t-display-comment-count.md)
   + [Sociaal delen inschakelen](c-advanced-topics/c-enabling-social-sharing.md)
   + [Activiteitenstroom](c-advanced-topics/c-activity-stream.md)
   + [Bootstrap HTML](c-advanced-topics/c-bootstrap-html.md)
   + [Verzameling wijzigen](c-advanced-topics/c-change-collection.md)
   + [Meerdere verzamelingen](c-advanced-topics/c-multiple-collections.md)
   + [Switch Core App-typen](c-advanced-topics/c-switch-core-app-types.md)
   + [Sociale teller](c-advanced-topics/c-social-counter.md)
   + [Bootsrap en stroom API met de Apps van het Leven gebruiken](c-advanced-topics/bootstrap-stream-api.md)
