---
unique-page-id: 11377395
description: Ajout d’un domaine de marque supplémentaire - Documents Marketo - Documentation du produit
title: Ajouter un domaine de branding supplémentaire
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: de2f73f932fd38211dba96d8697ef4bb4fd0f0da
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 3%

---

# Ajouter un domaine de branding supplémentaire {#add-an-additional-branding-domain}

Ajoutez un domaine de branding supplémentaire lorsque vous exécutez plusieurs marques à partir d’une seule instance Marketo et souhaitez que chacune d’elles ait ses propres liens de suivi de branding.

>[!PREREQUISITES]
>
>Vous devez [remplacer le lien de suivi générique](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} par un domaine de marque avant d’ajouter d’autres domaines de marque.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Cliquez sur **[!UICONTROL Ajouter]** pour ajouter un domaine de marque supplémentaire.

   ![](assets/add-an-additional-branding-domain-3.png){width="600"}

1. Saisissez le nom de votre nouveau domaine de marque, sélectionnez _Créer un domaine de Principal_ et/ou _Générer un certificat SSL_ (tous deux facultatifs), puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Définir comme domaine de Principal_ : définissez ce domaine comme votre domaine principal et tous les e-mails non envoyés existants définis sur « Par défaut » ainsi que tous les nouveaux e-mails seront définis par défaut sur le domaine principal. Vous pouvez [remplacer ce paramètre par e-mail](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _Générer un certificat SSL_ : vous pouvez créer un protocole SSL (Secure Sockets Layer) avec la création du domaine. Le premier domaine de suivi lance une configuration unique de l’infrastructure qui peut prendre quelques heures. Vous recevrez une notification à la fin de l’opération, puis vous pourrez configurer le premier domaine. Pour ajouter SSL à vos domaines existants, contactez l’assistance technique de [Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Modifier les SSL pour les domaines existants

Pour activer SSL pour vos domaines existants, procédez comme suit.

1. Dans la zone _[!UICONTROL Admin]_, sélectionnez **[!UICONTROL Email]**.

1. Dans l’onglet _[!UICONTROL Domaine]_, sélectionnez la ligne de domaine et cliquez sur **[!UICONTROL Ajouter SSL]**.

   ![Admin - Email - Domain - Add SSL](./assets/admin-email-branding-domain-add-ssl.png){width="600"}

1. Dans la boîte de dialogue, cliquez sur **[!UICONTROL Confirmer]**.

   ![Ajouter SSL - Confirmer](./assets/generate-ssl-cert-confirm.png){width="400"}

## Message d&#39;erreur {#error-messages}

<table><thead>
  <tr>
    <th>Erreur</th>
    <th>Détails</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>Le domaine existe déjà.</i></td>
    <td>Un domaine du même nom existe déjà.</td>
  </tr>
  <tr>
    <td><i>Le domaine n’est pas mappé au domaine par défaut.</i></td>
    <td>Le domaine personnalisé n’est pas correctement mappé au domaine par défaut. Vérifiez les paramètres de mappage de domaine et assurez-vous que la configuration DNS pointe vers le domaine par défaut correct.</td>
  </tr>
  <tr>
    <td><i>Impossible d’émettre les certificats SSL en raison d’enregistrements CAA non pris en charge. Demandez à votre service informatique de mettre à jour vos enregistrements CAA.</i></td>
    <td>Les enregistrements CAA ne sont pas à jour. Pour les utilisateurs et utilisatrices qui utilisent des certificats SSL gérés par Marketo Engage, les enregistrements CAA doivent être mis à jour vers les certificats recommandés par notre fournisseur. Contactez votre service informatique pour mettre à jour les enregistrements CAA. Voir <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">cette page</a> pour plus d’informations.</td>
  </tr>
  <tr>
    <td><i>Le certificat SSL a déjà été émis.</i></td>
    <td>Un certificat SSL existe déjà pour ce domaine personnalisé. Aucune autre action n’est nécessaire, sauf si le certificat a expiré ou doit être réémis.</td>
  </tr>
  <tr>
    <td><i>Le domaine par défaut est introuvable. Contactez l’assistance pour obtenir de l’aide.</i></td>
    <td>Un problème s’est produit lors de la recherche du domaine par défaut. Contactez l’assistance pour qu’elle enquête.</td>
  </tr>
  <tr>
    <td><i>Erreur inattendue lors de la création d'un domaine. Contactez l’assistance pour obtenir de l’aide.</i></td>
    <td>Une erreur inattendue s’est produite. Veuillez rassembler les journaux et les détails de l'erreur, puis signaler le problème à l'assistance de <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo</a>.</td>
  </tr>
</tbody></table>

## Éléments à noter {#things-to-note}

* **Mappage DNS du domaine vers Marketo Engage** : avant d’ajouter des domaines dans l’interface utilisateur, vous devez [mapper des CNAME à un domaine fourni par Marketo](https://experienceleague.adobe.com/fr/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSL personnalisés** : si vous avez besoin d’un SSL personnalisé, envoyez un ticket [Support technique](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. N’utilisez pas la case à cocher en libre-service pour la création SSL.

* **SSL préexistants** : lors de l’ajout d’un domaine, le système recherche les SSL préexistants, qui peuvent avoir été créés manuellement au préalable. Si vous rencontrez cette validation, créez votre domaine sans sélectionner la création SSL, et nous les connecterons pour vous. [Contactez l’assistance](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} plus d’informations/d’options.

* **Suppression de domaines** : la suppression automatique d’un domaine **ne supprime pas** le certificat SSL. Ce mécanisme de sécurisation empêche les erreurs utilisateur qui entraînent la suppression des certificats SSL d’un site web. Si vous souhaitez supprimer les certificats SSL, [contactez l’assistance ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

>[!MORELIKETHIS]
>
>[Modifiez Votre Domaine De Branding Par Défaut](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
