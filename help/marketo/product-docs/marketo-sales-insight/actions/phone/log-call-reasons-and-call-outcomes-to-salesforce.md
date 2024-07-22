---
description: Enregistrer les motifs des appels et les résultats des appels dans Salesforce - Documents Marketo - Documentation du produit
title: Enregistrer les motifs des appels et les résultats des appels dans Salesforce
exl-id: cfe71388-282b-45e5-a817-45a951f613bc
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 2%

---

# Enregistrer les motifs des appels et les résultats des appels dans Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Si vous souhaitez consigner les résultats des appels et les raisons des appels à Salesforce à des fins de reporting ou de visibilité, vous pouvez créer un champ d’activité personnalisé pour chacun d’eux. Chaque champ doit utiliser un nom d’API spécifique (appelé &quot;Nom de champ&quot; dans Salesforce).

* Appeler les résultats Nom du champ : mktosales_call_result
* Nom du champ Raisons de l’appel : mktosales_call_reason

Pour utiliser ces champs, vous devez d’abord créer le champ en tant que champ d’activité personnalisé. Pour le rendre visible par les utilisateurs, vous devez l’ajouter à la mise en page de la page de l’objet de tâche.

## Salesforce Classic {#salesforce-classic}

### Créer un champ d’activité personnalisé dans Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. Dans Salesforce, cliquez sur **Setup**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Saisissez &quot;Activités&quot; dans la zone Recherche rapide .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Cliquez sur **Champs personnalisés de l’activité**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Cliquez sur **New**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Sélectionnez le type de données &quot;Texte&quot; et cliquez sur **Suivant**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Attribuez au champ personnalisé le nom du champ tel que défini ci-dessus. La longueur du champ est limitée à 255 caractères. Le libellé du champ est le champ visible par votre équipe commerciale et peut être personnalisé en fonction des besoins de votre équipe.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Le reste des paramètres est facultatif. Une fois la configuration terminée, cliquez sur **Suivant**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Sélectionnez les paramètres de sécurité au niveau du champ de votre choix pour ce champ et cliquez sur **Suivant** (l’image ci-dessous n’est qu’un exemple).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Assurez-vous que le champ personnalisé est visible pour le profil que vos utilisateurs utilisent pour les actions d’aperçu des ventes, ainsi que tout autre champ que vous souhaitez voir.

1. Sélectionnez les mises en page auxquelles vous souhaitez ajouter le champ et cliquez sur **Enregistrer** (vous pouvez éventuellement cliquer sur **Enregistrer et nouveau** et répéter le processus pour le champ Motif de l’appel ).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Ajout d’un champ d’activité personnalisé à la disposition de la page de tâche dans Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Vous n’aurez à suivre ces étapes que si vous n’avez pas sélectionné la mise en page souhaitée à l’étape 9 ci-dessus.

1. Dans Salesforce, cliquez sur **Setup**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Saisissez &quot;Tâche&quot; dans la zone de recherche rapide.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Cliquez sur **Task Page Layouts**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Cliquez sur **Modifier** en regard de la mise en page de la tâche à laquelle vous souhaitez ajouter ce champ.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Faites glisser et déposez le champ dans la section souhaitée de la mise en page de la page Tâche .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### Créer un champ d’activité personnalisé dans Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. Dans Salesforce, cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **Configuration**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Cliquez sur **Object Manager**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Saisissez &quot;Activité&quot; dans la zone Recherche rapide .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Cliquez sur le libellé **Activité** .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Cliquez sur **Champs et relations**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Cliquez sur **New**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Ajout d’un champ d’activité personnalisé à la disposition de la page de tâche dans Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. Dans Salesforce, cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **Configuration**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Cliquez sur **Object Manager**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Saisissez &quot;Tâche&quot; dans la zone de recherche rapide.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Cliquez sur le libellé **Task** .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Cliquez sur **Dispositions de page**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Cliquez sur pn la mise en page de la page de la tâche à laquelle vous souhaitez ajouter ce champ.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Faites glisser et déposez le champ dans la section souhaitée de la mise en page de la page Tâche .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>* [Résultats des appels](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-outcomes.md)
>* [Raisons de l’appel](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-reasons.md)
