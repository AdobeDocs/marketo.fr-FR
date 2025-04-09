---
description: Ajout de SSL à vos pages d’entrée - Documentation Marketo - Documentation produit
title: Ajout de SSL à vos pages d’entrée
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: 1112af01c08835876f4a2385f304a33e2ddd48ff
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Ajout de SSL à vos pages d’entrée {#add-ssl-to-your-landing-pages}

Le chiffrement SSL (Secure Socket Layer) vous permet de sécuriser toutes vos pages de destination pour une instance Marketo Engage.

Lorsque vous remplissez un formulaire web ou que vous visitez une page de destination hébergée par Marketo Engage, les informations sont envoyées par défaut via un protocole non sécurisé (HTTP). Conformément à la politique de votre entreprise, vous souhaiterez peut-être sécuriser les informations soumises à Marketo via (HTTPS). Par exemple, lors de votre visite `http://info.mydomain.com/` , il sera `https://info.mydomain.com/`désormais .

Marketo Engage suit par défaut « Page Web visitée » et « Cliquer sur le lien sur la page Web » sur un protocole HTTP non sécurisé. Si vous souhaitez que vos liens de suivi soient sécurisés avec leur propre certificat, vous devez demander à Marketo de créer un serveur non partagé distinct pour l’activer. Pour sécuriser tous les aspects de l’interaction d’un contact avec vous, il faut généralement sécuriser à la fois les pages de destination et les liens de suivi.

CAPTURE D’ÉCRAN

## Activer la certification SSL {#enable-ssl-certification}

Ajoutez automatiquement SSL pour tous les alias de domaine que vous créez dans le cadre des règles de page d’entrée.

1. Accédez à la **zone Administration** .

   CAPTURE D’ÉCRAN

1. Sélectionnez **Landing Pages** dans l’arborescence. Dans l’onglet **Règles** , cliquez sur la **liste déroulante Nouveau** et sélectionnez **Nouvel alias de** domaine.

   CAPTURE D’ÉCRAN

1. Cochez la case Générer un **certificat** SSL.

   CAPTURE D’ÉCRAN

Cette opération ajoute automatiquement un certificat SSL pour ce domaine.

CAPTURE D’ÉCRAN

## Activation du protocole SSL pour votre domaine par défaut {#enable-ssl-default-domain}

CAPTURE D’ÉCRAN

>[!NOTE]
>
>* La colonne Certificat SSL dans la liste affiche l’état du certificat pour tous les alias de domaine créés après la sortie de cette fonctionnalité (DATE). Si vous aviez activé le SSL pour un domaine via le support Marketo, le certificat continuera d’exister, mais ne s’affichera pas dans le tableau. Ce tableau reflète uniquement les certificats SSL pour les domaines ajoutés à l’aide des étapes décrites dans cet article.
>
>* Il peut s’écouler jusqu’à trois minutes avant que le SSL ne soit à l’état PRÊT. Vous devez actualiser la page pour que les modifications s’affichent.
