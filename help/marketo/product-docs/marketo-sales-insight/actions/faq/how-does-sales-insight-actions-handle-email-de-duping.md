---
description: Comment les actions Sales Insight gèrent-elles le dédoublonnage des emails - Documents Marketo - Documentation du produit
title: Comment les actions Sales Insight gèrent-elles le dédoublonnage des emails
hide: true
hidefromtoc: true
source-git-commit: 47b0f31b410f0bf4b41740aa6440c2a0484ab835
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Comment Les Actions Sales Insight Gèrent-Elles Le Déduplication Des Emails ? {#how-does-sales-insight-actions-handle-email-de-duping}

Quand tu es [chargement d’un fichier CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) dans les actions Sales Insight, nous fusionnons tous les contacts similaires dans le fichier CSV avant l’importation.

Nous le faisons en fonction d&#39;adresses email similaires. Ainsi, s&#39;il existe deux adresses email identiques, nous les fusionnons en un seul contact.

Si vous essayez ultérieurement d&#39;ajouter/télécharger manuellement le même contact, nous ne le fusionnerons pas.

Si vous essayez d&#39;ajouter un contact déjà présent dans votre base de données, nous vous empêcherons de l&#39;ajouter.
