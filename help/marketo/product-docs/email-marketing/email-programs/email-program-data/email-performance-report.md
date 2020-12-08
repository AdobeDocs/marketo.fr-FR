---
unique-page-id: 2359467
description: Rapport de performances des courriels - Documents marketing - Documentation du produit
title: Rapport Performance des courriers électroniques
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Rapport Performance des courriers électroniques {#email-performance-report}

Pour déterminer les performances de vos courriels avec des statistiques telles que la diffusion, l’ouverture, les clics, etc., créez un rapport sur les performances des courriels.

1. [Créez un rapport dans un Programme](../../../../product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) et sélectionnez le type **de** rapport Performances [du](../../../../product-docs/reporting/basic-reporting/report-types/report-type-overview.md)courriel.
1. [Modifiez la période](../../../../product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) du rapport et cliquez sur l’onglet **Rapport** .
1. Vous êtes là ! Examinez maintenant le rapport pour voir comment vos courriels se sont comportés.

   >[!NOTE]
   >
   >Le filtre Date d’envoi est basé sur la première date d’envoi du courrier électronique.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Cliquez sur le nom d’un courrier électronique pour l’ouvrir dans l’outil de prévisualisation du courrier électronique.

   >[!NOTE]
   >
   >
   >Un rapport sur les performances des courriels comprend des activités pour toutes les personnes, y compris celles qui ont été supprimées depuis l’envoi du courrier électronique. Parfois, vous voulez voir des activités uniquement pour les principaux. Dans ce cas, vous devez filtrer les personnes supprimées de votre rapport. Utilisez l&#39;onglet Liste **** intelligente pour [créer une liste](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) intelligente pour le rapport. Si vous ne filtrez aucun champ spécifique, définissez le filtre Adresse électronique sur : **n’est pas vide**.

   [Sélectionnez les colonnes](../../../../product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) du rapport pour un rapport Performance de courriel :

   | Colonne | Description |
   |---|---|
   | Bruyant | Le courrier électronique a été rejeté en raison d’une condition permanente, telle qu’une adresse électronique inexistante. |
   | Rebond léger | Le courrier électronique a été rejeté en raison d’une condition temporaire, telle qu’un serveur en panne ou une boîte de réception complète. |
   | En attente | Ce nombre est calculé en soustrayant du nombre total d’envois le nombre d’e-mails distribués, rebondis et rebonds. |
   | Lien cliqué | Nombre de destinataires de messagerie qui ont cliqué sur un lien dans le courrier électronique. |
   | Non abonné | Nombre de destinataires de messagerie qui ont cliqué sur le lien **Se désabonner** dans le courrier électronique et rempli le formulaire. |

   >[!NOTE]
   >
   >La désinscription des liens et des adresses électroniques sur lesquels l’utilisateur clique dans un courriel ne s’inscrit pas sous Liens cliqués dans le rapport.

En général, nous essayons d&#39;utiliser le bon sens pour enregistrer ces statistiques. Par exemple, si une personne a cliqué sur un lien dans un courriel, elle a manifestement ouvert le courriel en premier. Nous suivons les règles spécifiques suivantes pour le rapport Performance de courriel :

* **Article 1**: Chaque enregistrement d’activité par courrier électronique est défini sur l’un des éléments suivants, et sur un seul : *Livré*, *Différé*, Rebond *modéré ou* En attente **.

* **Article 2**: Si l’enregistrement de courrier électronique affiche *Ouvert*, il est comptabilisé comme *Livré*.

* **Article 3**: Si l’enregistrement de courrier électronique affiche le message électronique ** cliqué ou le *désabonnement*, il est comptabilisé comme *Livré* et *Ouvert.*

* **Article 4**: Si le courrier électronique est *ouvert*, les rebonds sont ignorés. Si le courrier électronique n’a pas été ouvert, les rebonds ** nets ont la priorité sur les rebonds ** doux et les *remises*.

>[!NOTE]
>
>Plusieurs envois de la même campagne à la même personne ne sont comptabilisés qu’une seule fois.

>[!NOTE]
>
>**Articles connexes**
>
>* [Filtrage des ressources dans les rapports de messagerie Campaign](../../../../product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Rapport Performance des liens de courriel](email-link-performance-report.md)

>



>[!NOTE]
>
>**Plongée profonde**
>
>En savoir plus sur le Rapports [](http://docs.marketo.com/display/docs/basic+reporting)de base.

