---
unique-page-id: 2359467
description: Découvrez comment créer et utiliser le rapport Performance des e-mails. Suivre les ouvertures, les clics, les bounces et d’autres mesures relatives aux e-mails.
title: Rapport des performances des e-mails
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 96%

---

# Rapport des performances des e-mails {#email-performance-report}

Pour évaluer les performances de vos e-mails par rapport à des statistiques telles que la diffusion, l’ouverture, les clics, etc., créez un rapport sur les performances des e-mails.

1. [Créez un rapport dans un programme](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md), puis sélectionnez le [type de rapport](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md) **[!UICONTROL Performances des e-mails]**.
1. [Modifiez la période du rapport](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md), puis cliquez sur l’onglet **[!UICONTROL Rapport]**.
1. Le tour est joué. Parcourez maintenant le rapport pour voir les performances de votre ou vos e-mails.

   >[!NOTE]
   >
   >Le filtre Date d’envoi est basé sur la première date d’envoi de l’e-mail.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Cliquez sur le nom d’un e-mail pour l’ouvrir dans le Prévisualiseur d’e-mail.

   >[!NOTE]
   >
   >Un rapport sur les performances des e-mails inclut des activités pour toutes les personnes, y compris celles qui ont été supprimées depuis l’envoi de l’e-mail. Parfois, vous souhaitez afficher les activités uniquement pour les personnes actives. Dans ce cas, vous devez filtrer pour retirer les personnes supprimées de votre rapport. Utilisez l’onglet **[!UICONTROL Liste intelligente]** pour [créer une liste intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) pour le rapport. Si vous ne filtrez aucun champ spécifique, définissez le filtre Adresse e-mail sur : **[!UICONTROL n’est pas vide]**.

   Pour un rapport Performances des e-mails, [sélectionnez les colonnes du rapport](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) comme suit :

   <table><thead>

<tr>
    <th>Colonne</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Renvoi définitif</td>
    <td>L’e-mail a été rejeté en raison d’une condition permanente, telle qu’une adresse e-mail inexistante.</td>
  </tr>
  <tr>
    <td>Renvoi temporaire</td>
    <td>L’e-mail a été rejeté en raison d’une condition temporaire, telle qu’une panne de serveur ou une boîte de réception pleine.</td>
  </tr>
  <tr>
    <td>En attente</td>
    <td>Ce nombre est calculé en soustrayant le nombre d’e-mails diffusés et renvoyés définitivement ou temporairement du nombre total d’envois.</td>
  </tr>
  <tr>
    <td>Lien cliqué</td>
    <td>Nombre de personnes destinataires de l’e-mail qui ont cliqué sur un lien dans l’e-mail.</td>
  </tr>
  <tr>
    <td>Désabonnement</td>
    <td>Nombre de personnes destinataires de l’e-mail qui ont cliqué sur le lien de désabonnement dans l’e-mail et rempli le formulaire.</td>
  </tr>
  <tr>
    <td>Abandonné</td>
    <td>Nombre d’e-mails n’ayant pas pu être diffusés sans événement de renvoi. Un e-mail est automatiquement qualifié d’Abandonné si aucune réponse n’est reçue dans les trois jours suivant l’envoi de l’e-mail.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Les liens de désabonnement et les adresses e-mail sur lesquelles la personne clique dans un e-mail ne s’enregistrent pas sous Liens cliqués dans le rapport.

En général, nous essayons d’utiliser le bon sens pour consigner ces statistiques. Par exemple, si une personne clique sur un lien dans un e-mail, cela implique qu’elle a ouvert l’e-mail en premier lieu. Nous suivons ces règles spécifiques pour le rapport sur les performances des e-mails :

* **Règle 1 :** chaque activité de l’e-mail enregistrée prend une et une seule des valeurs suivantes : _Diffusé_, _Renvoi définitif_, _Renvoi temporaire_ ou _En attente_.

* **Règle 2** : si l’e-mail est enregistré comme _[!UICONTROL Ouvert]_, il est compté comme _Diffusé_.

* **Règle 3** : si l’enregistrement de l’e-mail affiche _[!UICONTROL E-mail cliqué]_ ou _[!UICONTROL Désabonnement]_, il est comptabilisé comme _Diffusé_ et _Ouvert_.

* **Règle 4** : si l’e-mail est _[!UICONTROL Ouvert]_, les renvois sont ignorés. Si l’e-mail n’a pas été ouvert, _Renvoi définitif_ est prioritaire sur _Renvoi temporaire_ et _Diffusé_.

* **Règle 5** : si aucune activité d’e-mail n’est reçue trois jours après son envoi, il est considéré _Abandonné_.

>[!NOTE]
>
>* Les envois multiples de la même campagne à la même personne sont comptabilisés une seule fois.
>
>* Les envois multiples de différentes campagnes à la même personne sont comptabilisés séparément.

>[!MORELIKETHIS]
>
>* [Filtrer les ressources dans des rapports des e-mails de campagne](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtrer les enregistrements supprimés/fusionnés dans un rapport des performances des e-mails](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Rapport sur les performances des liens dans les e-mails](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
