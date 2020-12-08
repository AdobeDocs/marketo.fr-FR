---
unique-page-id: 14352514
description: Comment Sales Connect gère le décodage des e-mails - Docs marketing - Documentation sur les produits
title: Comment Sales Connect gère le déclassement des e-mails
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# Comment Sales Connect gère le déclassement des e-mails {#how-sales-connect-handles-email-de-duping}

Lorsque vous [téléchargez un fichier CSV](http://docs.marketo.com/x/VADb) dans Sales Connect, nous fusionnons tous les contacts similaires dans le fichier CSV avant l&#39;importation.

Nous le faisons en fonction de l&#39;adresse électronique de type &quot;courriel&quot;. Donc, s&#39;il y a deux adresses électroniques identiques, nous les fusionnons en un seul contact.

Si vous essayez plus tard d&#39;ajouter ou de transférer manuellement le même contact, nous ne le fusionnerons pas.

Si vous essayez d&#39;ajouter un contact qui se trouve déjà dans votre base de données, nous vous empêcherons de l&#39;ajouter.

