---
unique-page-id: 14352476
description: Comprenez le champ de type d'activité sur les tâches lors de la synchronisation de Sales Connect avec Salesforce. Découvrez comment les types de tâches sont mappés et affichés dans Salesforce.
title: Champ Type d’activité dans les tâches (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/UJAL2pE3Pq0n7Sn9ev7GMGkBbgx12pZ0I5lBzfLpF1c
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 5%

---

# Champ Type d’activité dans les tâches (SFDC) {#activity-type-field-on-tasks-sfdc}

Avec l’aide de [!DNL Sales Connect], vous pouvez enregistrer vos e-mails et appels en tant qu’activité dans [!DNL Salesforce]. Pour disposer de données utiles dans [!DNL Salesforce], il est essentiel que le champ [!UICONTROL Type] renseigne la valeur correcte.

>[!NOTE]
>
>La journalisation des e-mails en Cci ne s’effectue pas dans la liste de sélection Type de tâche et remplit automatiquement le champ de type en tant qu’« e-mail », car ils sont envoyés à [!DNL Salesforce] via votre adresse en Cci.

## Exigences {#requirements}

* Connexion avec [!DNL Salesforce]
* Aucune valeur Type par défaut sélectionnée dans la liste de sélection Type de tâche
* Les champs Appel, Réponse et E-mail doivent tous figurer dans la liste de sélection Type de tâche (les majuscules sont importantes)
* Aucun workflow ou déclencheur n’agissant sur la valeur du champ Type

## Configuration {#setup}

Vérifiez d’abord que vous avez mis en place les valeurs correctes dans la liste de sélection. Vous aurez besoin de l’aide de votre administrateur [!DNL Salesforce] pour apporter des modifications à votre liste de sélection.

1. Accédez à [Salesforce.com](https://salesforce.com) et cliquez sur Configurer dans le coin supérieur droit.
1. Cliquez sur **[!UICONTROL Personnaliser]**.
1. Cliquez sur **[!UICONTROL Activités]**.
1. Cliquez sur **[!UICONTROL Champs de tâche]**.
1. Cliquez sur **[!UICONTROL Type]**.
1. Vous êtes maintenant dans la liste de sélection des types de tâches. Assurez-vous que l’option « Par défaut » n’est pas sélectionnée.
1. Assurez-vous qu’une valeur [!UICONTROL Type] est répertoriée pour [!UICONTROL E-mail], [!UICONTROL Appel] et [!UICONTROL Réponse].

Maintenant que cela est en place, vous commencerez à voir le champ Type renseigner la valeur correspondante pour les e-mails, appels et réponses consignés. Ces valeurs ne seront _pas_ renseignées sur les tâches de rappel Sales Connect.

>[!NOTE]
>
>Si vous ne voyez pas &#39;Répondre&#39; comme valeur, ajoutez-la en cliquant sur **[!UICONTROL Nouveau]**. &#39;Reply&#39; n&#39;est pas une valeur standard dans [!DNL Salesforce].
