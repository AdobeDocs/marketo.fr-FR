---
unique-page-id: 2359828
description: Ajouter SSL à vos pages de destination - Documents Marketo - Documentation du produit
title: Ajouter SSL à vos pages de destination
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: de396f08c50a1862fbdd3ae1e435ac5671d96b0e
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# Ajouter SSL à vos pages de destination {#add-ssl-to-your-landing-pages}

Le chiffrement SSL (Secure Socket Layer) vous permet de sécuriser toutes vos pages de destination pour une instance Marketo Engage.

Lorsque vous remplissez un formulaire web ou que vous visitez une page de destination hébergée par Marketo Engage, les informations sont envoyées via un protocole non sécurisé (HTTP). Conformément à la politique de votre société, vous pouvez sécuriser les informations envoyées à Marketo via (HTTPS). Par exemple, lorsque vous visitez `http://info.mydomain.com/`, il sera désormais `https://info.mydomain.com/`.

Par défaut, Marketo Engage effectue le suivi de la « Page web visitée » et du « Lien de clic sur la page web » via un protocole HTTP non sécurisé. Si vous souhaitez que vos liens de suivi soient sécurisés avec leur propre certificat, vous devez demander à Marketo de créer un serveur non partagé distinct pour l’activer. Pour sécuriser tous les aspects de l’interaction d’un contact avec vous, vous devez généralement sécuriser à la fois les pages de destination et les liens de suivi.

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
>* La colonne Certificat SSL de la liste indique le statut du certificat pour tous les alias de domaine créés après la publication de cette fonctionnalité (25 avril 2025). Si le SSL a été activé pour un domaine via la prise en charge de Marketo, le certificat continuera d’exister, mais ne s’affichera pas dans le tableau. Ce tableau reflète uniquement les certificats SSL pour les domaines ajoutés à l’aide des étapes de cet article.
>
>* Le statut PRÊT du SSL peut prendre jusqu’à trois minutes. Vous devez actualiser la page pour que les modifications s’affichent.

## Message d&#39;erreur {#error-messages}

Vous trouverez ci-dessous les messages d’erreur que vous pouvez recevoir, ainsi que leurs définitions.

<table><thead>
  <tr>
    <th>Erreur</th>
    <th>Détails</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>Erreur inattendue lors de la création d'un domaine. Contactez l’assistance pour obtenir de l’aide.</i></td>
    <td>Une erreur inattendue s’est produite. Rassemblez les journaux et les détails de l’erreur, puis signalez le problème à l’assistance.</td>
  </tr>
  <tr>
    <td><i>Le domaine par défaut est introuvable. Contactez l’assistance pour obtenir de l’aide.</i></td>
    <td>Un problème s’est produit lors de la recherche du domaine par défaut. Contactez l’assistance pour qu’elle enquête.</td>
  </tr>
  <tr>
    <td><i>Le certificat SSL a déjà été émis.</i></td>
    <td>Un certificat SSL existe déjà pour ce domaine personnalisé. Aucune autre action n’est nécessaire, sauf si le certificat a expiré ou doit être réémis.</td>
  </tr>
  <tr>
    <td><i>Le domaine n’est pas mappé au domaine par défaut.</i></td>
    <td>Le domaine personnalisé n’est pas correctement mappé au domaine par défaut. Vérifiez les paramètres de mappage de domaine et assurez-vous que la configuration DNS pointe vers le domaine par défaut correct.</td>
  </tr>
  <tr>
    <td><i>Le domaine existe déjà.</i></td>
    <td>Un domaine du même nom existe déjà.</td>
  </tr>
  <tr>
    <td><i>Une configuration IP ponctuelle est requise avant d’ajouter d’autres domaines. Contactez l’assistance pour terminer la configuration et tentez à nouveau d’ajouter un autre domaine.</i></td>
    <td>Le premier domaine personnalisé après le domaine par défaut nécessite une configuration unique que vous devez initier. Veuillez créer un ticket d’assistance pour terminer la configuration et ajouter le domaine une fois celle-ci terminée.</td>
  </tr>
</tbody></table>

## Éléments à noter {#things-to-note}

* **Mappage DNS du domaine vers Marketo Engage** : avant d’ajouter des domaines dans l’interface utilisateur, vous devez [mapper des CNAME à un domaine fourni par Marketo](https://experienceleague.adobe.com/fr/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSL personnalisés** : si vous avez besoin d’un SSL personnalisé, envoyez un ticket [Support technique](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. N’utilisez pas la case à cocher en libre-service pour la création SSL.

* **SSL préexistants** : lors de l’ajout d’un domaine, le système recherche les SSL préexistants, qui peuvent avoir été créés manuellement au préalable. Si vous rencontrez cette validation, créez votre domaine sans sélectionner la création SSL, et nous les connecterons pour vous. [Contactez l’assistance](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} plus d’informations/d’options.

* **Premier domaine de suivi** : la première création des domaines de liens de suivi des e-mails nécessitera une intervention manuelle de la part de l’assistance [Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. La création ultérieure de sous-domaines sous le même domaine est autorisée dans l’interface utilisateur.

* **Ajout de certificats à des domaines existants** : l’ajout de certificats à des domaines existants n’est pas pris en charge pour le moment. Pour les domaines préexistants ou dans les cas où vous n’avez pas coché la case de certificat SSL, vous devez contacter [l’assistance Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} pour obtenir le certificat ajouté.

* **Suppression de domaines** : la suppression d’un domaine ne supprime pas automatiquement le certificat SSL pour le moment. Ce problème sera résolu dans une version ultérieure.
