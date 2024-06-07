---
unique-page-id: 45417125
description: Sales Insight for Non Native Salesforce Integrations - Documents Marketo - Documentation du produit
title: Statistiques des ventes pour les intégrations Salesforce non natives
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1230'
ht-degree: 0%

---

# Statistiques des ventes pour les intégrations Salesforce non natives {#sales-insight-for-non-native-salesforce-integrations}

Si votre compte Adobe Marketo Engage est connecté à Salesforce par le biais d’une intégration personnalisée ou non native, utilisez cet article pour configurer Sales Insight.

>[!PREREQUISITES]
>
>* La fonction &quot;MSI Non natif&quot; est activée pour votre instance Marketo avant de commencer à configurer MSI. Si ce n’est pas le cas, veuillez contacter [Prise en charge de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Si vous n’avez pas encore acheté cette fonctionnalité, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>* Un compte Salesforce avec [Configuration du package MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* API REST MARKETO [configuration réussie](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Les API CRUD exposées seront la base de la synchronisation non native.
>* Lecture [billet de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} afin d’obtenir une compréhension de l’objet et des relations.
>* Configurez les objets Salesforce pour qu’ils affichent l’identifiant unique global non sensible à la casse de 18 caractères plutôt que l’identifiant unique global sensible à la casse de 15 caractères.

>[!NOTE]
>
>La configuration de l’API REST dans le panneau d’administration MSI de Marketo ne peut pas être utilisée pour la synchronisation non native.

## Une synchronisation non native réussie pour MSI nécessite les éléments suivants : {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchroniser l’utilisateur commercial Salesforce avec Marketo.

   L’utilisateur commercial Salesforce est un utilisateur externe propriétaire des Leads/Contacts dans Salesforce. Un représentant commercial Marketo doit être mis à jour pour l’utilisateur commercial Salesforce. La variable *externalSalesPersonId* est obligatoire pour l’insertion de la personne commerciale.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ Personne Vente Marketo</strong></td> 
      <td><strong>Champ d’utilisateur des ventes Salesforce</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identifiant unique global sensible à la casse des utilisateurs Salesforce Sales</td> 
      <td><p>Identifie l’enregistrement Marketo Sales Person à un objet Salesforce Sales User externe.</p><p>Il est obligatoire que la personne commerciale soit synchronisée avant de synchroniser les autres objets afin que les relations appropriées soient créées.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour le représentant commercial : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * Documentation de l’API pour la synchronisation de la personne commerciale : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisation des comptes Salesforce avec Marketo.

   Une société Marketo doit être mise à niveau pour le compte Salesforce. La variable _externalCompanyId_ et _externalSalesPersonId_ Les champs sont obligatoires pour l’insertion de la société.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ de société Marketo</strong></td> 
      <td><strong>Champ de compte Salesforce</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identifiant unique global sensible à la casse du compte Salesforce</td> 
      <td>Identifie un enregistrement Marketo Company à un objet de compte Salesforce externe.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identifiant unique global sensible à la casse des utilisateurs Salesforce Sales</td> 
      <td>Identifie un enregistrement Marketo Company à un objet Salesforce Sales User externe propriétaire du compte.<br><br>Également utilisé dans Marketo pour associer la société à la personne commerciale propriétaire de l’enregistrement de société. Il est obligatoire de synchroniser d’abord la personne commerciale avant de définir ce champ.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation API pour les entreprises : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentation de l’API pour la synchronisation des entreprises : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Synchronisez les contacts/prospects Salesforce avec Marketo.

   Vous devez insérer un prospect Marketo pour le prospect/contact Salesforce. La variable _externalPersonId_, _externalSalesPersonId_, et _externalCompanyId_ Les champs sont obligatoires pour l’insertion du prospect.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ de piste Marketo</strong></td> 
      <td><strong>Champ de prospect/contact Salesforce</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Identifiant unique global non sensible à la casse des leads/contacts Salesforce</td> 
      <td>Identifie l’enregistrement de piste Marketo à un objet de piste/contact Salesforce externe.<br><br>Il s’agit d’un nouveau champ qui est introduit pour MSI Non-Native.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identifiant unique global sensible à la casse des utilisateurs Salesforce Sales</td> 
      <td>Identifie l’objet externe Salesforce Sales User propriétaire de ce prospect/contact.<br><br>Fait également le lien entre le prospect et la personne qui effectue les ventes dans Marketo. Il est obligatoire que la personne commerciale soit synchronisée correctement en premier.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identifiant unique global sensible à la casse du compte Salesforce</td> 
      <td>Identifie l’objet de compte Salesforce externe auquel le prospect/contact appartient.<br><br>Associe également l’enregistrement de piste à une société dans Marketo. Il est obligatoire que le compte Salesforce soit correctement synchronisé en premier.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour Leads : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads)
   * Documentation de l’API pour la synchronisation des pistes : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Synchronisation des opportunités Salesforce avec Marketo.

   Vous devez insérer une opportunité Marketo pour l’opportunité Salesforce. La variable _externalOpportunityId_, _externalCompanyId_, et _externalSalesPersonId_ Les champs sont obligatoires pour la promotion de l’opportunité.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ d’objet d’opportunité Marketo</strong></td> 
      <td><strong>Champ d’objet d’opportunité Salesforce</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identifiant unique global non sensible à la casse des leads/contacts Salesforce</td> 
      <td>Identifie l’enregistrement Marketo Opportunity à un objet Salesforce Opportunity externe.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identifiant unique global sensible à la casse du compte Salesforce</td> 
      <td>Identifie l’objet de compte Salesforce externe auquel cette opportunité appartient. <br><br>Il est obligatoire que le compte Salesforce soit correctement synchronisé en premier.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identifiant unique global sensible à la casse des utilisateurs Salesforce Sales</td> 
      <td>Identifie l’objet externe Salesforce Sales User propriétaire de cette opportunité. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour Opportunity : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentation de l’API pour la synchronisation des opportunités : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchroniser les rôles de contact Salesforce avec Marketo.

   Les rôles de contact Salesforce pour une opportunité Salesforce peuvent ensuite être synchronisés via le rôle d’opportunité Marketo. L’enregistrement Rôle d’opportunité requiert le _externalOpportunityId_, _rôle_, et _leadId_ des champs.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ Rôle de l’opportunité Marketo</strong></td> 
      <td><strong>Champ de rôle de contact Salesforce</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identifiant unique global non sensible à la casse pour Salesforce Opportunity</td> 
      <td>Identifie le rôle d’opportunité Marketo à un objet d’opportunité Salesforce externe.<br><br>Il est obligatoire que l’opportunité Salesforce soit correctement synchronisée en premier.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>S.O. : il s’agit d’un ID de piste Marketo</td> 
      <td>Il s’agit de l’ID de piste Marketo du contact Salesforce synchronisé.<br><br>Une fois le contact synchronisé dans Marketo, vous pouvez utiliser l’identifiant unique global sensible à la casse des contacts Salesforce comme externalPersonId et la requête pour le prospect Marketo à l’aide de l’API REST Marketo.</td> 
     </tr> 
     <tr> 
      <td>Rôle</td> 
      <td>Le champ Rôle du contact Salesforce</td> 
      <td>Décrit le rôle du contact pour cette opportunité.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour Opportunity : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentation de l’API pour la synchronisation des opportunités : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchroniser les champs de notation MSI/Dernier moment intéressant avec SFDC.

   Une fois vos objets Salesforce correctement synchronisés avec Marketo, vous pouvez profiter des fonctionnalités MSI. Les champs MSI Last intéressant Moment/Score seront exposés dans l’API REST pour Leads. Ces champs sont calculés par MSI et sont en lecture seule.

   Les champs Dernier moment/Score intéressant d’un prospect Marketo doivent être régulièrement synchronisés avec Salesforce à l’aide du point de terminaison de l’API REST. Interrogez ce point de terminaison pour un prospect Marketo à l’aide de la variable _externalPersonId_ comme filterType et transmission du GUID de prospect Salesforce en tant que filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Vous pouvez ensuite utiliser les valeurs de ces champs pour vous synchroniser à votre objet Lead/contact Salesforce.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ de piste Marketo</strong></td> 
      <td><strong>Champ de prospect/contact Salesforce</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentType</td> 
      <td>Libellé : Dernier type de moment intéressant<br>Nom : Last_Interesting_Moment_Type__c</td> 
      <td>Type du dernier moment intéressant pour l'affaire</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDate</td> 
      <td><p>Libellé : Date du dernier moment intéressant</p><p>Nom : Last_Interesting_Moment_Date__c</p></td> 
      <td>Date du dernier moment intéressant pour le prospect</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDesc</td> 
      <td><p>Libellé : Dernier moment intéressant Description</p><p>Nom : Last_Interesting_Moment_Desc__c</p></td> 
      <td>Description du dernier moment intéressant pour le prospect</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentSource</td> 
      <td><p>Libellé : Dernière source de moment intéressant</p><p>Nom : Last_Interesting_Moment_Source__c</p></td> 
      <td>Source du dernier moment intéressant pour l'affaire</td> 
     </tr> 
     <tr> 
      <td>priorité</td> 
      <td><p>Libellé : Engagement</p><p>Nom : Priority__c</p></td> 
      <td>Priorité de la piste</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>Libellé : valeur d’urgence relative</p><p>Nom : Urgency_Value__c</p></td> 
      <td>Urgence relative de l’avance</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Libellé : valeur de notation relative</p><p>Nom : Relative_Score_Value__c</p></td> 
      <td>Score relatif de la piste</td> 
     </tr> 
    </tbody> 
   </table>

   Documentation de l’API REST Lead : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   Une bonne utilisation des champs externes est essentielle pour une synchronisation non native réussie. Si vous ne voyez pas les données dans certaines des vues, il est probable qu’un certain champ n’ait pas été correctement synchronisé. Par exemple, si les activités d’une piste et les moments intéressants ne s’affichent pas lors de la recherche dans le widget MSI sous leur compte, il est probable que la société de la piste ou le compte n’ont pas été correctement synchronisés. L’exécution d’une demande de GET pour ce prospect lors de la spécification des champs externes vous aidera à vérifier si le prospect a été correctement synchronisé. De plus, le courrier électronique du commercial externe dans Marketo doit correspondre à celui de cet utilisateur dans Salesforce. Les données peuvent ne pas s’afficher dans l’onglet Marketo de Salesforce si les emails ne correspondent pas.
