---
unique-page-id: 2359467
description: Rapport Performances des emails - Documents Marketo - Documentation du produit
title: Rapport des performances des e-mails
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 3%

---

# Rapport des performances des e-mails {#email-performance-report}

Pour vérifier les performances de vos emails avec des statistiques telles que la diffusion, l’ouverture, le clic, etc., créez un rapport Performance des emails .

1. [Création d’un rapport dans un programme](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) et sélectionnez la variable **Performances des emails** [Type de rapport](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Modification de la période de rapport](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) et cliquez sur le bouton **Rapport** .
1. Vous êtes là ! Maintenant, explorez le rapport pour voir comment vos emails se sont comportés.

   >[!NOTE]
   >
   >Le filtre Date d’envoi repose sur la première date d’envoi de l’e-mail.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Cliquez sur le nom d’un email pour l’ouvrir dans le prévisualiseur d’email.

   >[!NOTE]
   >
   >Un rapport de performances des emails comprend des activités pour toutes les personnes, y compris celles qui ont été supprimées depuis l’envoi du message. Parfois, vous souhaitez afficher les activités uniquement pour les personnes principales. Dans ce cas, vous devez filtrer les personnes supprimées de votre rapport. Utilisez la variable **Liste dynamique** à [création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) pour le rapport. Si vous ne filtrez aucun champ spécifique, définissez le filtre Adresse électronique sur : **n’est pas vide**.

   [Sélectionner les colonnes du rapport](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) pour un rapport de performances des emails, procédez comme suit :

   | Colonne | Description |
   |---|---|
   | Renvoi définitif | Le courrier électronique a été rejeté en raison d’une condition permanente, telle qu’une adresse électronique inexistante. |
   | Retour en erreur temporaire | Le courrier électronique a été rejeté en raison d’une condition temporaire, telle qu’un serveur en panne ou une boîte de réception pleine. |
   | en attente | Ce nombre est calculé en soustrayant du nombre total d’envois le nombre d’emails délivrés, de messages rebonds et de messages soft rebonds. |
   | Lien cliqué | Nombre de destinataires de courrier électronique ayant cliqué sur un lien dans le courrier électronique. |
   | Désabonné | Nombre de destinataires du courrier électronique ayant cliqué sur la variable **Désabonner** dans le courrier électronique et remplissez le formulaire. |

   >[!NOTE]
   >
   >Les liens de désabonnement et les adresses électroniques sur lesquels l’utilisateur clique dans un email ne sont pas enregistrés sous Liens cliqués dans le rapport.

En général, nous essayons d&#39;utiliser le bon sens pour enregistrer ces statistiques. Par exemple, si quelqu’un a cliqué sur un lien dans un email, il est évident qu’il a ouvert l’email en premier. Nous suivons ces règles spécifiques pour le rapport Performance des emails :

* **Règle 1**: Chaque enregistrement d’activité de courrier électronique est défini sur une seule des valeurs suivantes : _Délivrés_, _Hard Bounce_, _Soft Bounce_ ou _En attente_.

* **Règle 2**: Si l’enregistrement du courrier électronique s’affiche *Ayant ouvert*, il est comptabilisé comme *Délivrés*.

* **Règle 3**: Si l’enregistrement du courrier électronique s’affiche _Courrier électronique cliqué_ ou _Désabonné_, il est comptabilisé comme _Délivrés_ et _Ayant ouvert_.

* **Règle 4**: Si l’adresse électronique est _Ayant ouvert_, les rebonds sont ignorés. Si l&#39;email n&#39;a pas été ouvert, _Hard Bounce_ a priorité sur _Soft Bounce_ et _Délivrés_.

>[!NOTE]
>
>Les envois multiples d’une même campagne vers la même personne ne sont comptabilisés qu’une seule fois.

>[!MORELIKETHIS]
>
>* [Filtrage des ressources dans les rapports de messagerie de Campaign](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Rapport Performance des liens de courriel](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

