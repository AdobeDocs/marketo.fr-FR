---
description: Configuration du suivi de domaine personnalisé - Documents Marketo - Documentation du produit
title: Configuration du suivi de domaine personnalisé
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Configuration du suivi de domaine personnalisé {#how-to-set-up-custom-domain-tracking}

Le suivi de domaine personnalisé permet à votre équipe d’utiliser le nom de votre propre société dans tous les liens pouvant faire l’objet d’un suivi ajoutés à vos e-mails de vente. Une fois cette configuration effectuée, nous placerons sur la liste autorisée tout lien contenu dans votre email qui apparaîtra sous la forme go.yourcompany.com. Ainsi, lorsque quelqu’un survole un lien, celui-ci lira go.yourcompany.com au lieu de go.toutapp.com.

Vous aurez besoin de l’aide de votre équipe informatique pour configurer un enregistrement CNAME pour votre domaine qui pointe vers go.toutapp.com. Ce CNAME s’affiche sur tous les liens de suivi (par exemple, go.yourcompany.com).

Une fois que vous avez confirmé auprès de votre équipe informatique que le CNAME est correctement configuré, vous pouvez l’ajouter à la page Suivi des domaines personnalisés dans Actions.

>[!NOTE]
>
>Si votre CNAME n’est pas configuré correctement et que vous l’activez en tant que domaine personnalisé dans Actions, il peut rompre les liens de suivi et les pixels.

## Activation du suivi de domaine personnalisé {#enable-custom-domain-tracking}

>[!NOTE]
>
>**Droits d’administrateur requis.**

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. Sous Paramètres d’administration, sélectionnez **Tracking**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. Dans l’onglet Suivi de domaine personnalisé , saisissez votre CNAME et cliquez sur **Se connecter**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
