---
unique-page-id: 1147031
description: Supprimer une personne de SFDC - Documents marketing - Documentation du produit
title: Supprimer une personne de SFDC
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Supprimer une personne de SFDC {#delete-person-from-sfdc}

Si vous devez supprimer un ensemble spécifique de pistes de Salesforce mais les laisser en tant que personnes dans Marketo, vous pouvez utiliser l’action Supprimer une personne de SFDC.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Disponible uniquement lorsqu&#39;il est intégré à Salesforce.

1. Dans la base de données, cliquez sur la personne que vous souhaitez supprimer de Salesforce. Cliquez ensuite sur Actions **** personnelles et sélectionnez **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Sélectionnez **Supprimer une personne dans SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Assurez-vous que le paramètre **Supprimer dans Marketo** est **false**, puis cliquez sur **Exécuter maintenant**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Une fois l’étape de flux exécutée, votre personne ne sera plus une piste dans Salesforce, mais restera sur le marché.

   >[!CAUTION]
   >
   >Si vous définissez **Supprimer dans Marketo** sur **true** et supprimez les personnes de Marketo et les pistes de Salesforce, elles sont parties pour toujours. Cela ne peut pas être annulé.

