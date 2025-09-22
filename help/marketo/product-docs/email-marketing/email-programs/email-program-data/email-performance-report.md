---
unique-page-id: 2359467
description: Rapport sur les performances des e-mails - Documents Marketo - Documentation du produit
title: Rapport des performances des e-mails
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 3%

---

# Rapport des performances des e-mails {#email-performance-report}

Pour évaluer les performances de vos e-mails par rapport à des statistiques telles que la diffusion, l’ouverture, le clic, etc., créez un rapport sur les performances des e-mails.

1. [Créer un rapport dans un programme](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) puis sélectionnez le **[!UICONTROL Performance des emails]** [Type de rapport](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Modifiez la période du rapport](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) puis cliquez sur l’onglet **[!UICONTROL Rapport]**.
1. Vous êtes là ! Explorez maintenant le rapport pour voir comment s’est comporté votre ou vos e-mails.

   >[!NOTE]
   >
   >Le filtre Date d’envoi est basé sur la première date d’envoi de l’e-mail.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Cliquez sur le nom d’un e-mail pour l’ouvrir dans la Prévisualisation d’e-mail.

   >[!NOTE]
   >
   >Un rapport sur les performances des emails inclut des activités pour toutes les personnes, y compris celles qui ont été supprimées depuis l&#39;envoi de l&#39;email. Parfois, vous souhaitez afficher les activités uniquement pour les personnes actives. Dans ce cas, vous devez filtrer les personnes supprimées de votre rapport. Utilisez l’onglet **[!UICONTROL Liste dynamique]** pour [créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) pour le rapport. Si vous ne filtrez aucun champ spécifique, définissez le filtre Adresse e-mail sur : **[!UICONTROL n’est pas vide]**.

   [Sélectionner les colonnes du rapport](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) pour un rapport Performance des e-mails, procédez comme suit :

   <table><thead>

<tr>
    <th>Colonne</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Renvoi définitif</td>
    <td>L'e-mail a été rejeté en raison d'une condition permanente, telle qu'une adresse e-mail inexistante.</td>
  </tr>
  <tr>
    <td>Renvoi temporaire</td>
    <td>L’e-mail a été rejeté en raison d’une condition temporaire, telle qu’une panne de serveur ou une boîte de réception pleine.</td>
  </tr>
  <tr>
    <td>En attente</td>
    <td>Ce nombre est calculé en soustrayant le nombre d'e-mails diffusés, rejetés et soft rebonds du nombre total d'envois.</td>
  </tr>
  <tr>
    <td>Lien cliqué</td>
    <td>Nombre de destinataires d’e-mails qui ont cliqué sur un lien dans l’e-mail.</td>
  </tr>
  <tr>
    <td>Désabonné ou désabonnée</td>
    <td>Nombre de destinataires d’e-mails qui ont cliqué sur le lien de désabonnement dans l’e-mail et rempli le formulaire.</td>
  </tr>
  <tr>
    <td>Interrompu</td>
    <td>Nombre d’e-mails n’ayant pas pu être délivrés et aucun événement de rebond n’ayant été reçu. Un e-mail est automatiquement qualifié d’Abandonné si aucune réponse n’est reçue dans les trois jours suivant l’envoi de l’e-mail.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Les liens de désabonnement et les adresses e-mail sur lesquelles l’utilisateur clique dans un e-mail ne s’enregistrent pas sous Liens cliqués dans le rapport.

En général, nous essayons d&#39;utiliser le bon sens pour consigner ces statistiques. Par exemple, si une personne cliquait sur un lien dans un e-mail, elle ouvrait évidemment l’e-mail en premier. Nous suivons les règles suivantes pour le rapport sur les performances des e-mails :

* **Règle 1** : chaque enregistrement d’activité d’e-mail est défini sur un seul des éléments suivants : _Diffusé_, _Hard bounce_, _Soft bounce_ ou _En attente_.

* **Règle 2** : si l’enregistrement de l’e-mail indique _[!UICONTROL Ouvert]_, il est comptabilisé comme _Diffusé_.

* **Règle 3** : si l’enregistrement d’e-mail affiche _[!UICONTROL E-mail cliqué]_ ou _[!UICONTROL Désabonné]_, il est comptabilisé comme _Diffusé_ et _Ouvert_.

* **Règle 4** : si l&#39;email est _[!UICONTROL Ouvert]_, les rebonds sont ignorés. Si l’e-mail n’a pas été ouvert, _hard bounce_ est prioritaire sur _soft bounce_ et _diffusé_.

* **Règle 5** : si aucune activité d’e-mail n’est reçue trois jours après son envoi, elle est considérée _Abandonnée_.

>[!NOTE]
>
>* Les envois multiples de la même campagne à la même personne sont comptabilisés une seule fois.
>
>* Les envois multiples de différentes campagnes à la même personne sont comptabilisés séparément.

>[!MORELIKETHIS]
>
>* [Filtrer Assets dans les rapports de campagne par e-mail](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtrer les enregistrements supprimés/fusionnés dans un rapport sur les performances des e-mails](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [ Rapport sur les performances des liens d’e-mail ](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
