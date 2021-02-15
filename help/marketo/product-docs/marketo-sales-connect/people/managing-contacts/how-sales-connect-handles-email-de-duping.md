---
unique-page-id: 14352514
description: Comment Sales Connect gère le décodage des e-mails - Docs marketing - Documentation sur les produits
title: Comment Sales Connect gère le déclassement des e-mails
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Comment Sales Connect gère le déclassement des e-mails {#how-sales-connect-handles-email-de-duping}

Lorsque vous téléchargez [un fichier CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) dans Sales Connect, nous fusionnons tous les contacts similaires dans le CSV avant que l&#39;importation ne se produise.

Nous le faisons en fonction de l&#39;adresse électronique de type &quot;courriel&quot;. Donc, s&#39;il y a deux adresses électroniques identiques, nous les fusionnons en un seul contact.

Si vous essayez plus tard d&#39;ajouter ou de transférer manuellement le même contact, nous ne le fusionnerons pas.

Si vous essayez d&#39;ajouter un contact qui se trouve déjà dans votre base de données, nous vous empêcherons de l&#39;ajouter.
