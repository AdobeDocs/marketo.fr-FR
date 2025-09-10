---
unique-page-id: 2359828
description: Ajouter SSL à vos pages de destination - Documents Marketo - Documentation du produit
title: Ajouter SSL à vos pages de destination
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: 2bbfe8f1d000f182aba3a1d3e0c58c1be47b76a7
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 2%

---

# Ajouter SSL à vos pages de destination {#add-ssl-to-your-landing-pages}

Le chiffrement SSL (Secure Socket Layer) vous permet de sécuriser toutes vos pages de destination pour une instance Marketo Engage.

Lorsque vous remplissez un formulaire web ou que vous visitez une page de destination hébergée par Marketo Engage, les informations sont envoyées via un protocole non sécurisé (HTTP). Conformément à la politique de votre société, vous pouvez sécuriser les informations envoyées à Marketo via (HTTPS). Par exemple, lorsque vous visitez `http://info.mydomain.com/`, il sera désormais `https://info.mydomain.com/`.

Par défaut, Marketo Engage effectue le suivi de la « Page web visitée » et du « Lien de clic sur la page web » via un protocole HTTP non sécurisé. Si vous souhaitez que vos liens de suivi soient sécurisés avec leur propre certificat, vous devez demander à Marketo de créer un serveur non partagé distinct pour l’activer. Pour sécuriser tous les aspects de l’interaction d’un contact avec vous, vous devez généralement sécuriser à la fois les pages de destination et les liens de suivi.

>[!IMPORTANT]
>
>Avant d’ajouter un protocole SSL, vérifiez le nombre total de domaines autorisés dans votre contrat. Dans le cas contraire, des frais peuvent être encourus. Si vous ne trouvez pas ces informations, contactez l’équipe chargée de votre compte Adobe (votre gestionnaire de compte) pour obtenir plus d’informations.

## Activer la certification SSL {#enable-ssl-certification}

Ajoutez automatiquement le protocole SSL pour tous les alias de domaine que vous créez dans le cadre des règles de page de destination.

1. Accédez à la zone **Admin**.

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. Sélectionnez **Pages de destination** dans l’arborescence. Dans l’onglet **Règles**, cliquez sur la liste déroulante **Nouveau** et sélectionnez **Nouvel alias de domaine**.

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. Saisissez vos _Alias de domaine_ et _Page par défaut_. Cochez la case **Générer un certificat SSL**. Cliquez sur **Créer** lorsque vous avez terminé.

   ![](assets/add-ssl-to-your-landing-pages-3.png)

Un certificat SSL est automatiquement ajouté pour ce domaine.

## Activer SSL pour votre domaine par défaut {#enable-ssl-default-domain}

Suivez les étapes ci-dessous pour activer SSL pour votre domaine par défaut.

1. Toujours dans la section **Admin**, sélectionnez **Pages de destination**. Cliquez sur le bouton orange **Modifier** en regard de _Paramètres_.

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Si vous le souhaitez, vous pouvez également modifier le nom de domaine ici (domaine valide requis).

1. Sélectionnez la case à cocher « Générer un certificat SSL » et cliquez sur Enregistrer.

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>Le statut PRÊT du SSL peut prendre jusqu’à trois minutes. Vous devez actualiser la page pour que les modifications s’affichent.

## Message d&#39;erreur {#error-messages}

Vous trouverez ci-dessous les messages d’erreur que vous pouvez recevoir, ainsi que leurs définitions.

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
