---
unique-page-id: 2359828
description: Ajouter SSL à vos pages de destination - Documents Marketo - Documentation du produit
title: Ajouter SSL à vos pages de destination
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: 7ec3687c0c16738805394377b2080295c2f18032
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

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
>* La colonne Certificat SSL de la liste indique le statut du certificat pour tous les alias de domaine créés après la publication de cette fonctionnalité (DATE). Si le SSL a été activé pour un domaine via la prise en charge de Marketo, le certificat continuera d’exister, mais ne s’affichera pas dans le tableau. Ce tableau reflète uniquement les certificats SSL pour les domaines ajoutés à l’aide des étapes de cet article.
>
>* Le statut PRÊT du SSL peut prendre jusqu’à trois minutes. Vous devez actualiser la page pour que les modifications s’affichent.
