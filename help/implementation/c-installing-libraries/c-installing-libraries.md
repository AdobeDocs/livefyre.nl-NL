---
description: Bibliotheken installeren voor taken op de server van LiveCyre
title: Installatie
exl-id: d74f85be-14c0-4f6d-8f16-b688282c0eb0
source-git-commit: 3091db9d7b9611e26ad65c1432856c9465694e92
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Installatie{#installation}


## Java {#section_yd3_3zk_rz}

Om de bibliotheek van Java te installeren, voeg deze gebiedsdeel aan POM van uw project toe:

```
<dependency> 
   <groupId>com.livefyre</groupId> 
   <artifactId>livefyre</artifactId> 
   <version>2.0.3</version> 
</dependency>
```

De Java-bibliotheek is afhankelijk van de volgende modules:

```
<dependency> 
   <groupId>com.sun.jersey</groupId> 
   <artifactId>jersey-client</artifactId> 
   <version>[1.18.1,)</version> 
</dependency> 
<dependency> 
   <groupId>com.google.code.gson</groupId> 
   <artifactId>gson</artifactId> 
   <version>[2.3,)</version> 
</dependency> 
<dependency> 
   <groupId>com.google.guava</groupId> 
   <artifactId>guava</artifactId> 
   <version>[18.0,)</version> 
</dependency> 
<dependency> 
   <groupId>org.apache.commons</groupId> 
   <artifactId>commons-lang3</artifactId> 
   <version>[3.0.1,)</version> 
</dependency> 
<dependency> 
   <groupId>org.bitbucket.b_c</groupId> 
   <artifactId>jose4j</artifactId> 
   <version>[0.4.1,)</version> 
</dependency> 
```

Voor meer informatie, lees de documenten van Java of zie de bron op [GitHub](https://github.com/Livefyre/livefyre-java-utils).

## NodeJS {#section_swj_pwq_rz}

Voer de volgende regel uit om de NodeJS-bibliotheek te installeren:

`$ npm install livefyre`

De bibliotheek NodeJS heeft gebiedsdelen op de volgende modules:

```
"restler":">=3.2.0", 
"validator":"=3.5.0", 
"jsonwebtoken": ">=5.0.0" 
```

Voor meer informatie, lees de documenten NodeJs of zie de bron op [GitHub](https://github.com/Livefyre/livefyre-nodejs-utils).

Koppelingen: [Restler](https://github.com/danwrong/restler), [Validator](https://www.npmjs.org/package/validator), [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken).

## PHP {#section_txj_xwq_rz}

Als u de PHP-bibliotheek met Composer wilt installeren, voegt u dit toe aan uw composer.json:

```
"require": { 
   "livefyre/livefyre-php-utils": "2.0.4" 
}
```

Vervolgens installeren met:

```
composer.phar install 
```

Als u **not** gebruik Composer, verkrijg de recentste versie van de bibliotheek gebruikend:

```
git clone https://github.com/Livefyre/livefyre-php-utils 
```

Als u de bibliotheek wilt gebruiken, voegt u het volgende toe aan uw PHP-script:

```
require_once("/path/to/livefyre-php-utils/src/Livefyre.php"); 
```

De PHP bibliotheek is afhankelijk van de volgende modules:

```
"ext-json": "*", 
"rmccue/requests": ">=1.0" 
"firebase/php-jwt": ">=2.0" 
```

Lees voor meer informatie de PHP docs of zie de bron op [GitHub](https://github.com/Livefyre/livefyre-php-utils).

Koppelingen: [ext-json](https://www.php.net/manual/en/book.json.php), [Requests](https://github.com/rmccue/Requests/), [PHP-JWT](https://github.com/firebase/php-jwt/tree/v2.0.0)

## Python {#section_irk_fxq_rz}

Voer de volgende regel uit om de Python-bibliotheek te installeren:

`$ pip install livefyre`

De Python-bibliotheek is afhankelijk van de volgende modules:

```
PyJWT >= 1.0.1  
requests >= 2.2.1  
python-dateutil >= 2.2  
enum34 == 1.0  
ordereddict == 1.1 if sys.version_info[:2] < 2.7 
```

Voor meer informatie, lees de dokken van Python of zie de bron op [GitHub](https://github.com/Livefyre/livefyre-python-utils).

Koppelingen: [PyJWT](https://github.com/progrium/pyjwt), [Requests](https://github.com/kennethreitz/requests), [Python-Dateutil](https://pypi.python.org/pypi/python-dateutil), [Enum34](https://pypi.python.org/pypi/enum34), [OrderedDict](https://pypi.python.org/pypi/ordereddict)

## Ruby {#section_fv2_tzq_rz}

Als u de Ruby-bibliotheek wilt installeren, voegt u deze regel toe aan het werkbestand van uw toepassing:

```
gem 'livefyre' 
```

Of installeer het zelf:

`$ gem install livefyre`

De Ruby-bibliotheek is afhankelijk van de volgende modules:

```
"jwt", '~> 1.4', ">= 1.4.1"  
"rest-client", '~> 1.8', ">= 1.8.0"  
"addressable", '~> 2.3', ">= 2.3.6" 
```

Voor meer informatie, lees de Ruby dots of zie de bron op [GitHub](https://github.com/Livefyre/livefyre-ruby-utils).

Koppelingen: [Ruby JWT](https://github.com/firebase/php-jwt/tree/v2.0.0), [REST Client](https://github.com/rest-client/rest-client/), [Adressable](https://github.com/sporkmonger/addressable)
