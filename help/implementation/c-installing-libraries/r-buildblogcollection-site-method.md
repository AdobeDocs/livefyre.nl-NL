---
description: Retourneert een object Collection dat is geïnstantieerd als een blogtype. Voer create_or_update() uit vanaf het object Collection om het constructieproces te voltooien.
title: Site-methode buildBlogCollection
exl-id: 93565eff-dc4e-4868-9d75-50f16ddb4fa4
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

---

# buildBlogCollection Site Method{#buildblogcollection-site-method}

Retourneert een object Collection dat is geïnstantieerd als een blogtype. Voer create_or_update() uit vanaf het object Collection om het constructieproces te voltooien.

| Variabele | Type | Beschrijving |
|--- |--- |--- |
| titel | String | De titel voor de verzameling. |
| artikelId | String | Een unieke artikel-id die u hebt gekozen om een verzameling binnen uw site te identificeren. |
| url | String | De canonieke absolute URL voor deze verzameling. |

## Java-voorbeeld {#section_nyl_ycs_rz}

```
Collection collection = site.buildBlogCollection(title, articleId, url); 
```

## NodeJS-voorbeeld {#section_xkd_gds_rz}

```
var collection = site.buildBlogCollection(title, articleId, url); 
```

## PHP-voorbeeld {#section_ghf_gds_rz}

```
$collection = site->buildBlogCollection(title, articleId, url); 
```

## Python-voorbeeld {#section_dwg_gds_rz}

```
collection = site.build_blog_collection(title, articleId, url) 
```

## Ruby-voorbeeld {#section_enh_gds_rz}

```
collection = site.build_blog_collection(title, articleId, url) 
```
