---
description: Ajouter SSL à vos pages de destination - Documents Marketo - Documentation du produit
title: Ajouter SSL à vos pages de destination
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: 0e73866a4187d7bff67ce199e8d01e55081bcbef
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Ajouter SSL à vos pages de destination {#add-ssl-to-your-landing-pages}

Découvrez comment ajouter l’alias de votre domaine de marque (par exemple, `http://business.adobe.com`) aux pages de destination créées dans Marketo Engage afin qu’elles soient accessibles sous leurs domaines de marque.

CAPTURE D’ÉCRAN

## Activer la certification SSL {#enable-ssl-certification}

Ajoutez automatiquement le protocole SSL pour tous les alias de domaine que vous créez dans le cadre des règles de page de destination.

1. Accédez à la zone **Admin**.

   CAPTURE D’ÉCRAN

1. Sélectionnez **Pages de destination** dans l’arborescence. Dans l’onglet **Règles**, cliquez sur la liste déroulante **Nouveau** et sélectionnez **Nouvel alias de domaine**.

   CAPTURE D’ÉCRAN

1. Cochez la case **Générer un certificat SSL**.

   CAPTURE D’ÉCRAN

Un certificat SSL est automatiquement ajouté pour ce domaine.

CAPTURE D’ÉCRAN

## Activer SSL pour votre domaine par défaut

CAPTURE D’ÉCRAN

>[!NOTE]
>
>* La colonne Certificat SSL de la liste indique le statut du certificat pour tous les alias de domaine créés après la publication de cette fonctionnalité (DATE). Si le SSL a été activé pour un domaine via la prise en charge de Marketo, le certificat continuera d’exister, mais ne s’affichera pas dans le tableau. Ce tableau reflète uniquement les certificats SSL pour les domaines ajoutés à l’aide des étapes de cet article.
>
>* Le statut PRÊT du SSL peut prendre jusqu’à trois minutes. Vous devez actualiser la page pour que les modifications s’affichent.
