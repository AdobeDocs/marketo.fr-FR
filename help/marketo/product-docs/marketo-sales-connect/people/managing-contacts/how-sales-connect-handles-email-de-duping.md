---
unique-page-id: 14352514
description: Comment Sales Connect gère le nettoyage des emails - Documents Marketo - Documentation du produit
title: Comment Sales Connect gère la déduplication des emails
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Comment Sales Connect gère la déduplication des emails {#how-sales-connect-handles-email-de-duping}

Quand tu es [chargement d’un fichier CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) dans Sales Connect, nous fusionnons tous les contacts similaires dans le fichier CSV avant l’importation.

Nous le faisons en fonction d&#39;adresses email similaires. Ainsi, s&#39;il existe deux adresses email identiques, nous les fusionnons en un seul contact.

Si vous essayez ultérieurement d&#39;ajouter/télécharger manuellement le même contact, nous ne le fusionnerons pas.

Si vous essayez d&#39;ajouter un contact déjà présent dans votre base de données, nous vous empêcherons de l&#39;ajouter.
