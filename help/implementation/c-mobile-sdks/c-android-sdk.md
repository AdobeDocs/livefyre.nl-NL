---
description: Maak Android-apps met Livefyre.
title: Android-SDK
exl-id: 54ea6537-5f27-4174-af25-d17257f23e48
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Android-SDK{#android-sdk}

Maak Android-apps met Livefyre.

Gebruik deze bibliotheek om LiveCycle-services te integreren in uw systeemeigen Android-app. De [Livefyre StreamHub Android SDK](https://github.com/Livefyre/StreamHub-Android-SDK) verstrekt een dunne laag rond onze gemeenschappelijke API mechanismen, die op de Gradle/Android de ontwikkelomgeving wordt gebaseerd.

Livefyre verstrekt ook een [Beoordelingen](https://github.com/Livefyre/StreamHub-iOS-Reviews-App) steekproefapp, die op deze SDK wordt gebaseerd.

Deze Livefyre Android-SDK kan zowel in Eclipse als in Android Studio worden gebruikt.

>[!NOTE]
>
>Voordat u de Livefyre Android SDK installeert, moet de [Android SDK](https://developer.android.com/sdk/index.html) op uw omgeving zijn geïnstalleerd. U moet ook enkele extra Android SDK-pakketten opnemen, zoals beschreven in de documentatie voor Android-ontwikkelaars > .
>[SDK-pakketten toevoegen](https://developer.android.com/sdk/installing/adding-packages.html)

Gebruik Android SDK Manager (beschikbaar op de werkbalk Android Studio of Eclipse) om alle aanbevolen pakketten te installeren. Zorg ervoor dat u ook de Android Support Repository opneemt.

## {#section_dtm_slv_zz} uitknippen

U kunt als volgt de Livefyre Android-SDK toevoegen aan uw project in Eclipse:

1. Krijg recentste [StreamHub-Android-SDK](https://github.com/Livefyre/StreamHub-Android-SDK) van GitHub.
1. Begin met een bestaand project of maak een nieuw project.
1. Ga naar **[!UICONTROL File > Import > General > Existing Project into Workspace]** om de StreamHub-Android-SDK in uw werkruimte te importeren.
1. Blader en selecteer StreamHub-Android-SDK; het moet nu in de pakketverkenner worden getoond .
1. Klik met de rechtermuisknop op uw project en selecteer **[!UICONTROL Properties,]** en vervolgens het tabblad Android.
1. Onder de sectie van de Bibliotheek, selecteer **[!UICONTROL Add button,]** dan StreamHub-Android-SDK van de lijst van bibliotheken.
1. Klik op **[!UICONTROL Apply]** en **[!UICONTROL OK]**.

## Android Studio {#section_vpw_klv_zz}

U voegt als volgt de Livefyre Android SDK toe aan uw project in Android Studio:

1. Krijg recentste [StreamHub-Android-SDK](https://github.com/Livefyre/StreamHub-Android-SDK) van GitHub.
1. Begin met een bestaand project of maak een nieuw project.
1. Klik met de rechtermuisknop op uw project en selecteer **[!UICONTROL Open Module Settings]**.
1. Selecteer de **[!UICONTROL +]** knoop in de hoogste linkerhoek van het venster.
1. Selecteer **[!UICONTROL Import Existing Project.]** (In nieuwe versie van Android-studio vindt u **[!UICONTROL Import Existing Project]** onder **[!UICONTROL More Modules]**.)

1. Blader en selecteer StreamHub-Android-SDK.

Android Studio kan u vragen de SDK om te zetten in een grijze versie. Als dit voorkomt, selecteer **[!UICONTROL next]** dan **[!UICONTROL finish]**.

Ga naar **projectmap > toepassingsmap > build.gradle** bestand onder afhankelijkheden om de volgende afhankelijkheid toe te voegen:

```
dependencies {   compile project(':streamHubAndroidSDK') } 
```

Zorg ervoor dat de volgende lijn in uw **projectomslag > settings.gradle** dossier is:

```
include ':streamHubAndroidSDK' 
```

>[!NOTE]
>
>U kunt configuraties aanpassen vanuit Config.java.

## Clients {#section_yfq_blv_zz}

De StreamHub Android SDK stelt verscheidene cliëntklassen bloot die kunnen worden gebruikt om levende API eindpunten aan te vragen:

* **** AdminClientExchange een token voor gebruikersverificatie, sleutels en andere metagegevens.

* **** BootstrapClientGet recente inhoud en meta-gegevens over een bepaalde Inzameling.

* **** StreamClientPoll een stroom voor een Inzameling om nieuwe, bijgewerkte, en geschrapte inhoud terug te winnen.

* **** WriteClientPost, vlag, en als inhoud in een Inzameling.
