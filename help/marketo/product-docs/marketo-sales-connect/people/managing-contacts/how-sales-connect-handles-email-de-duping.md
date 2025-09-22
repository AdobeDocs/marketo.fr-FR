---
unique-page-id: 14352514
description: Comment Sales Connect Gère Le Duping Des E-Mails - Documents Marketo - Documentation Du Produit
title: Gestion de la suppression des doublons d’e-mails dans Sales Connect
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 6%

---

# Gestion du dédoublonnage [!DNL Sales Connect] e-mails {#how-sales-connect-handles-email-de-duping}

Lorsque vous [téléchargez un fichier CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) dans [!DNL Sales Connect], nous fusionnons tous les contacts comme dans le CSV avant que l’importation ne se produise.

Nous faisons cela en fonction d’une adresse e-mail similaire. Ainsi, s’il existe deux adresses e-mail identiques, nous les fusionnons en un seul contact.

Si vous essayez par la suite d’ajouter/de charger manuellement le même contact, nous ne le fusionnerons pas.

Si vous essayez d&#39;ajouter un contact qui est déjà dans votre base de données, nous vous empêcherons de l&#39;ajouter.
