---
unique-page-id: 14352514
description: Comment Sales Connect gère le nettoyage des emails - Documents Marketo - Documentation du produit
title: Comment Sales Connect gère la déduplication des emails
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Comment Sales Connect gère la déduplication des emails {#how-sales-connect-handles-email-de-duping}

Lorsque vous [ téléchargez un fichier CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) dans Sales Connect, nous fusionnons tous les contacts similaires dans le CSV avant l’importation.

Nous le faisons en fonction d&#39;adresses email similaires. Ainsi, s&#39;il existe deux adresses email identiques, nous les fusionnons en un seul contact.

Si vous essayez ultérieurement d&#39;ajouter/télécharger manuellement le même contact, nous ne le fusionnerons pas.

Si vous essayez d&#39;ajouter un contact déjà présent dans votre base de données, nous vous empêcherons de l&#39;ajouter.
