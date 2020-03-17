---
description: Retourneert een object Collection dat is geïnstantieerd als een type Counting. Voer create_or_update() uit vanaf het object Collection om het constructieproces te voltooien.
seo-description: Retourneert een object Collection dat is geïnstantieerd als een type Counting. Voer create_or_update() uit vanaf het object Collection om het constructieproces te voltooien.
seo-title: buildCountingCollection-sitemethode
title: buildCountingCollection-sitemethode
uuid: e293d66a-0025-4230-997e-295ce4625713
translation-type: tm+mt
source-git-commit: 67aeb3de964473b326c88c3a3f81ff48a6a12652

---


# buildCountingCollection-sitemethode{#buildcountingcollection-site-method}

Retourneert een object Collection dat is geïnstantieerd als een type Counting. Voer create_or_update() uit vanaf het object Collection om het constructieproces te voltooien.

| Variabele | Type | Beschrijving |
|--- |--- |--- |
| titel | String | De titel voor de verzameling. |
| artikelId | String | Een unieke artikel-id die u hebt gekozen om een verzameling binnen uw site te identificeren. |
| url | String | De canonieke absolute URL voor deze verzameling. |

## Java-voorbeeld {#section_nyl_ycs_rz}

```
Collection collection = site.buildCountingCollection(title, articleId, url); 
```

## Voorbeeld van NodeJS {#section_xkd_gds_rz}

```
var collection = site.buildCountingCollection(title, articleId, url); 
```

## PHP-voorbeeld {#section_ghf_gds_rz}

```
$collection = site->buildCountingCollection(title, articleId, url); 
```

## Voorbeeld van Python {#section_dwg_gds_rz}

```
collection = site.build_counting_collection(title, articleId, url) 
```

## Ruby-voorbeeld {#section_enh_gds_rz}

```
collection = site.build_counting_collection(title, articleId, url) 
```
