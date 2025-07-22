---
unique-page-id: 14352476
description: Champ de type d’activité sur Tâches (SFDC) - Documents Marketo - Documentation du produit
title: Champ Type d’activité sur Tâches (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# Champ Type d’activité sur Tâches (SFDC) {#activity-type-field-on-tasks-sfdc}

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
1. Vous êtes maintenant dans la liste de sélection des types de tâches. Vérifiez qu&#39;aucun paramètre « Default » n&#39;est sélectionné.
1. Assurez-vous qu’une valeur [!UICONTROL Type] est répertoriée pour [!UICONTROL E-mail], [!UICONTROL Appel] et [!UICONTROL Réponse].

Maintenant que cela est en place, vous commencerez à voir le champ Type renseigner la valeur correspondante pour les e-mails, appels et réponses consignés. Ces valeurs ne seront _pas_ renseignées sur les tâches de rappel Sales Connect.

>[!NOTE]
>
>Si vous ne voyez pas &#39;Répondre&#39; comme valeur, ajoutez-la en cliquant sur **[!UICONTROL Nouveau]**. &#39;Reply&#39; n&#39;est pas une valeur standard dans [!DNL Salesforce].
