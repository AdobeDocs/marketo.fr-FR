---
description: Enregistrer les motifs des appels et les résultats des appels dans Salesforce - Documents Marketo - Documentation du produit
title: Enregistrer les motifs des appels et les résultats des appels dans Salesforce
hide: true
hidefromtoc: true
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
source-git-commit: 0fc2551ffc85260a282b64995c698098846eb10c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Enregistrer les motifs des appels et les résultats des appels dans Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Si vous souhaitez consigner les résultats des appels et les raisons des appels à Salesforce à des fins de reporting ou de visibilité, vous pouvez créer un champ d’activité personnalisé pour chacun d’eux. Chaque champ doit utiliser un nom d’API spécifique (appelé &quot;Nom de champ&quot; dans Salesforce).

* Nom du champ des résultats de l’appel : mktosales_call_result
* Nom du champ Raisons de l’appel : mktosales_call_reason

Pour utiliser ces champs, vous devez d’abord créer le champ en tant que champ d’activité personnalisé. Pour le rendre visible par les utilisateurs, vous devez l’ajouter à la mise en page de la page de l’objet de tâche.

## Salesforce Classic {#salesforce-classic}

### Créer un champ d’activité personnalisé dans Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. Dans Salesforce, cliquez sur **Configuration**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Saisissez &quot;Activités&quot; dans la zone Recherche rapide .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Cliquez sur **Champs personnalisés d’une activité**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Cliquez sur **Nouveau**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Sélectionnez le type de données &quot;Texte&quot; et cliquez sur **Suivant**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Attribuez au champ personnalisé le nom du champ tel que défini ci-dessus. La longueur du champ est limitée à 255 caractères. Le libellé du champ est le champ visible par votre équipe commerciale et peut être personnalisé en fonction des besoins de votre équipe.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Le reste des paramètres est facultatif. Une fois la configuration terminée, cliquez sur **Suivant**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Sélectionnez les paramètres de sécurité au niveau du champ de votre choix pour ce champ, puis cliquez sur **Suivant** (l’image ci-dessous n’est qu’un exemple).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Assurez-vous que le champ personnalisé est visible pour le profil que vos utilisateurs de Sales Connect utilisent, ainsi que tout autre champ que vous souhaitez voir.

1. Sélectionnez les mises en page auxquelles vous souhaitez ajouter le champ, puis cliquez sur **Enregistrer** (Si vous le souhaitez, vous pouvez cliquer sur **Enregistrer et nouveau** et répétez le processus pour le champ Motif de l’appel .)

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Ajout d’un champ d’activité personnalisé à la disposition de la page de tâche dans Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

1. Dans Salesforce, cliquez sur **Configuration**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Saisissez &quot;Tâche&quot; dans la zone de recherche rapide.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Cliquez sur **Mises en page de tâche**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Cliquez sur **Modifier** en regard de la mise en page de la tâche à laquelle vous souhaitez ajouter ce champ.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Faites glisser et déposez le champ dans la disposition de la page Tâche .

   PICC

1. Cliquez sur **Enregistrer**.

   PICC

## Salesforce Lightning {#salesforce-lightning}

### Créer un champ d’activité personnalisé dans Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. Dans Salesforce, cliquez sur l’icône d’engrenage en haut à droite.

PICC

1. Cliquez sur **Configuration**.

PICC

1. Cliquez sur **Object Manager**.

PICC

1. Saisissez Activité dans la zone Recherche rapide , puis cliquez sur le libellé Activité pour ouvrir la configuration de l’objet.

PICC

1. Sur le côté gauche, cliquez sur **Champs et relations**.

PICC

1. Cliquez sur **Nouveau**.

PICC

## Ajout d’un champ d’activité personnalisé à la disposition de la page de tâche dans Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. Dans Salesforce, cliquez sur l’icône d’engrenage en haut à droite.

PICC

1. Cliquez sur **Configuration**.

PICC

1. Accédez à Configuration.?????????

PICC

1. Saisissez &quot;Tâche&quot; dans la zone de recherche rapide.

PICC

1. Cliquez sur Tâche.

PICC

1. Cliquez sur Mise en page.

PICC

1. Cliquez sur pn la mise en page de la page de la tâche à laquelle vous souhaitez ajouter ce champ.

PICC

1. Faites glisser et déposez le champ dans la disposition de la page Tâche .

PICC

1. Cliquez sur Enregistrer.

PICC

>[!MORELIKETHIS]
>
>[Installation des champs d’événement de connexion aux ventes dans l’historique des activités](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
