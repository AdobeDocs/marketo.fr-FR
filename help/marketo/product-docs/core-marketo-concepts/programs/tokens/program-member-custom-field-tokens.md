---
unique-page-id: 1147114
description: Jetons de champs personnalisés pour les membres de programme - Documents marketing - Documentation du produit
title: Jetons de champ personnalisés de membre de programme
translation-type: tm+mt
source-git-commit: 35e8b41574ebf8aafa27a59440c8ea9cb6413d50
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Jetons de champ personnalisés de membre de programme {#program-member-custom-field-tokens}

## Prise en charge des jetons pour les champs personnalisés des membres de Programme {#token-support-for-program-member-custom-fields}

Au verso des fonctionnalités Champs personnalisés des membres de Programme, la prise en charge des champs personnalisés des membres de Programme est étendue dans les cadres de jetons.

Les jetons PMCF seront pris en charge sous le domaine membre de la famille de jetons.

Les jetons de membre sont utilisés pour les champs relevant du champ Membre du Programme. À l&#39;heure actuelle, les jetons membres sont également utilisés pour insérer des valeurs uniques provenant de partenaires de services intégrés. `{{member.webinar url}}` résout automatiquement l’URL de confirmation unique générée par le prestataire. {{Member.register code}} correspond au code d&#39;enregistrement fourni par le prestataire.

>[!NOTE]
>
>* Les champs personnalisés des membres de programme ne peuvent être utilisés que dans le contexte d&#39;un programme.
>* Les jetons de champs personnalisés d&#39;un membre de programme ne peuvent pas être utilisés dans : scripts de courrier électronique, en-tête de courrier électronique, jetons de date dans les étapes d’attente ou extraits de code.
>* Le statut de membre de programme n&#39;est pas pris en charge dans les jetons de membre.


## Utilisation de jetons de champ personnalisés de membre de Programme dans les ressources {#using-program-member-custom-field-tokens-in-assets}

Vous pouvez insérer des jetons de champs personnalisés de membre de Programme dans des e-mails, des Landings page, des SMS, des notifications Push et des hameçons Web.

**Courriers électroniques**

1. Sélectionnez le courriel de votre choix et cliquez sur **Modifier le brouillon**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Cliquez sur l&#39;icône Insérer un jeton.

   ![](assets/program-member-custom-field-tokens-2.png)

1. Recherchez et sélectionnez le jeton de champ personnalisé de membre de Programme, entrez une valeur par défaut, puis cliquez sur **Insérer**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>N’oubliez pas d’approuver votre courriel.

**landings page**

1. Sélectionnez votre Landing page et cliquez sur **Modifier le brouillon**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >Le concepteur de landing page s’ouvre dans une nouvelle fenêtre.

1. Cliquez avec le doublon sur la zone de texte enrichi à laquelle vous souhaitez ajouter le jeton.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Cliquez à l’endroit où vous souhaitez placer le jeton, puis cliquez sur l’icône Insérer un jeton.

   ![](assets/program-member-custom-field-tokens-7.png)

1. Recherchez et sélectionnez le jeton de votre choix.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Saisissez une valeur par défaut et cliquez sur **Insérer**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Sélectionnez le SMS souhaité et cliquez sur **Modifier le brouillon**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Cliquez sur le bouton **`{{ Token`**.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Recherchez et sélectionnez le jeton de champ personnalisé de membre de Programme souhaité. Saisissez une valeur par défaut et cliquez sur Insérer.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Cliquez sur la liste déroulante Actions SMS et sélectionnez **Approuver et fermer**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Notifications Push**

1. Sélectionnez la notification Push souhaitée et cliquez sur **Modifier le brouillon**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Cliquez sur **Notification Push**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Cliquez sur le message dans l&#39;éditeur et cliquez sur le bouton `{{` pour obtenir le sélecteur de jetons.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Recherchez et sélectionnez le jeton de champ personnalisé de membre de Programme souhaité. Saisissez une valeur par défaut et cliquez sur **Insérer**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Cliquez sur **Terminer** pour enregistrer et quitter (ou **Suivant** pour passer en revue en premier).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Si le champ personnalisé de membre de Programme d&#39;un membre du programme n&#39;a pas de valeur, le jeton sera remplacé par la valeur par défaut si elle a été fournie.

## Utilisation de jetons de champ personnalisés de membre de Programme dans les campagnes {#using-program-member-custom-field-tokens-in-campaigns}

Les jetons de champ personnalisés de membre de programme peuvent être utilisés dans :

* Créer une Tâche
* Créer une Tâche dans Microsoft
* Moments intéressants
* Modifier les actions de flux de valeurs de données
* Liens Web
