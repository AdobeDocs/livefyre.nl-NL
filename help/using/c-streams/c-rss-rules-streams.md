---
description: U kunt stroomregels maken die inhoud ophalen uit RSS-feeds.
title: RSS-regels
exl-id: bfb3bbad-ab26-451e-b540-d6c41f54dc31
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# RSS-regels{#rss-rules}

U kunt stroomregels maken die inhoud ophalen uit RSS-feeds.

RSS-streams worden elke 5 minuten bijgewerkt, waarbij wordt gezocht naar inhoud die nog niet bestaat in LiveCycle uit de eerste 50 items in de feed. Livefyre negeert alles voorbij de eerste 50 voorwerpen in het voer.

Als u RSS-regels wilt maken om inhoud van RSS-feeds naar uw app of map te halen, kunt u filteren op:

* **[!UICONTROL URL]** van de RSS Feed.
* **[!UICONTROL Include recent items.]** Als deze is ingesteld op:

   * **[!UICONTROL Enabled]**, voegt Livefyre de eerste 50 inhoudselementen in uw voer aan de stroom toe, ongeacht de publicatiedatum.
   * **[!UICONTROL Disabled]**, voegt Livefyre de eerste 50 inhoudselementen in uw voer aan de stroom met een publicatiedatum toe die het zelfde als de de aanmaakdatum van de stroomregel of later is.

* **[!UICONTROL Extract post information from item link (when disabled, post information is extracted from XML).]** Trek informatie van de punthandeling of van XML.

**RSS-regels**

Livefyre parseert RSS-feeds op basis van de volgende RSS-specs:

* [RSS 2.0](https://en.wikipedia.org/wiki/RSS)
* [Media RSS](https://en.wikipedia.org/wiki/Media_RSS)
* [Atom-feed](https://validator.w3.org/feed/docs/atom.html)

Livefyre leest geen feeds die zich niet aan deze specs houden, en de inhoud ervan zal niet in uw stroom worden getrokken. Gebruik de Dienst van de Bevestiging van het Veed WC3 om de syntaxis van uw voer van RSS te controleren, en ervoor te zorgen dat het geldig is.

Voor extra de regelopties van de Stroom voor alle regels van de Stroom, zie [de Opties van de Regel van de Stroom voor Alle Regels van de Stroom](../c-streams/c-stream-rule-options-for-all-stream-rules.md#c_stream_rule_options_for_all_stream_rules).
