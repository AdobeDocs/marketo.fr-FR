---
unique-page-id: 45417125
description: Sales Insight for Non Native Salesforce Integrations - Marketo Docs - Documentation sur les produits
title: Insight commercial pour les intégrations Salesforce non natives
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 0%

---


# Insight commercial pour les intégrations Salesforce non natives {#sales-insight-for-non-native-salesforce-integrations}

Si votre compte Marketing est connecté à Salesforce par le biais d’une intégration personnalisée ou non native, utilisez ce document pour configurer Sales Insight.

>[!NOTE]
>
>**Conditions préalables**
>
>* Contactez votre responsable de succès client pour activer la fonction &quot;MSI non natif&quot; pour votre instance de marketing.
>* Un compte Salesforce avec la configuration du package MSI.
>* API REST de marketing [correctement configurée](http://developers.marketo.com/rest-api/). Les API CRUD exposées seront la base de la synchronisation non native.
>* Lisez [ce billet](http://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/) de blog afin de comprendre l&#39;objet et les relations.
>* Configurez les objets Salesforce pour qu’ils affichent l’identifiant unique global non sensible à la casse de 18 caractères plutôt que l’identifiant unique global sensible à la casse de 15 caractères.

>



>[!NOTE]
>
>La configuration de l’API REST dans le panneau d’administration MSI de Marketo ne peut pas être utilisée pour la synchronisation non native.

## La synchronisation non native réussie pour MSI nécessite les éléments suivants {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchronisez l&#39;utilisateur commercial Salesforce sur Marketo.

   L&#39;utilisateur commercial Salesforce est un utilisateur externe propriétaire des pistes/contacts dans Salesforce. Une personne commerciale du marketing doit être mise à jour pour l&#39;utilisateur commercial de Salesforce. Le champ *externalSalesPersonId* est obligatoire pour l&#39;insertion de la personne vendeuse.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Champ Personne commerciale</strong></td> 
   <td><strong>Champ Utilisateur commercial Salesforce</strong></td> 
   <td><strong>Description</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificateur unique global non sensible à la casse pour l'utilisateur commercial Salesforce</td> 
   <td><p>Identifie l'enregistrement de la personne vendeuse du marketing à un objet commercial Salesforce externe User.</p><p>Il a pour mandat de synchroniser d'abord la personne chargée des ventes avant de synchroniser les autres objets afin de créer les relations appropriées.</p></td> 
  </tr> 
 </tbody> 
</table>

Documentation de l’API pour le vendeur : [https://developers.marketo.com/rest-api/lead-database/sales-persons/](http://developers.marketo.com/rest-api/lead-database/sales-persons/)\
Documentation de l’API pour la synchronisation du Sales Person : [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/# !/Sales_Persons/syncSalesPersonsUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. Synchronisez les comptes Salesforce avec Marketo.

   Une Société de marketing devra être mise à jour pour le compte Salesforce. Les champs *externalCompanyId* et *externalSalesPersonId* sont obligatoires pour la sauvegarde de la Société.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Champ Société du marketing</strong></td> 
   <td><strong>Champ de compte Salesforce</strong></td> 
   <td><strong>Description</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificateur unique global non sensible à la casse du compte Salesforce</td> 
   <td>Identifie un enregistrement de Société Marketo à un objet Compte Salesforce externe.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificateur unique global non sensible à la casse pour l'utilisateur commercial Salesforce</td> 
   <td>Identifie un enregistrement de Société Marketo à un objet Utilisateur commercial Salesforce externe qui est le propriétaire du compte.<br><br>Également utilisé dans Marketo pour associer la Société à la personne qui détient l’enregistrement de Société. Il est obligatoire de synchroniser d'abord le responsable commercial avant de définir ce champ.</td> 
  </tr> 
 </tbody> 
</table>

Documentation de l’API pour les Sociétés : [https://developers.marketo.com/rest-api/lead-database/companies/](http://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Synchroniser les pistes/contacts Salesforce avec Marketo.

   Vous devez insérer une piste marketing pour le prospect/contact Salesforce. Les champs *externalPersonId*, *externalSalesPersonId* et *externalCompanyId* sont obligatoires pour la validation du prospect.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Champ de piste marketing</strong></td> 
   <td><strong>Champ de prospect/contact Salesforce</strong></td> 
   <td><strong>Description</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Identificateur unique global non sensible à la casse du prospect/contact Salesforce</td> 
   <td>Identifie l'enregistrement de piste marketing à un objet de piste/contact Salesforce externe.<br><br>Il s’agit d’un nouveau champ introduit pour MSI Non-Native.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificateur unique global non sensible à la casse pour l'utilisateur commercial Salesforce</td> 
   <td>Identifie l'objet Utilisateur commercial Salesforce externe propriétaire de ce prospect/contact.<br><br>Fait également le lien entre le responsable et le vendeur sur le marché. Il est obligatoire de synchroniser correctement la personne chargée des ventes en premier.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificateur unique global non sensible à la casse du compte Salesforce</td> 
   <td>Identifie l'objet Compte Salesforce externe auquel appartient le prospect/contact.<br><br>Associe également l'enregistrement de piste à une Société dans Marketo. Il est obligatoire que le compte Salesforce soit correctement synchronisé en premier.</td> 
  </tr> 
 </tbody> 
</table>

Documentation de l’API pour les pistes : [`https://developers.marketo.com/rest-api/lead-database/leads/`](http://developers.marketo.com/rest-api/lead-database/leads/)\
Documentation de l&#39;API pour la synchronisation des pistes :  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/# !/Leads/syncLeadUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Synchroniser les opportunités de Salesforce sur le marketing.

   Vous devez proposer une opportunité de marketing pour l&#39;opportunité Salesforce. Les champs *externalOpportunityId*, *externalCompanyId* et *externalSalesPersonId* sont obligatoires pour la promotion de l&#39;opportunité.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Champ d'objet Opportunité marketing</strong></td> 
   <td><strong>Champ d'objet Opportunité Salesforce</strong></td> 
   <td><strong>Description</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Identificateur unique global non sensible à la casse du prospect/contact Salesforce</td> 
   <td>Identifie l'enregistrement Opportunité marketing sur un objet Opportunité Salesforce externe.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificateur unique global non sensible à la casse du compte Salesforce</td> 
   <td>Identifie l'objet de compte Salesforce externe auquel cette opportunité appartient. <br><br>Il est obligatoire que le compte Salesforce soit correctement synchronisé en premier.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificateur unique global non sensible à la casse pour l'utilisateur commercial Salesforce</td> 
   <td>Identifie l'objet Utilisateur commercial Salesforce externe propriétaire de cette opportunité. </td> 
  </tr> 
 </tbody> 
</table>

Documentation de l&#39;API pour l&#39;opportunité : [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Synchroniser les rôles de contact Salesforce avec Marketo.

   Les rôles de contact Salesforce pour une opportunité Salesforce peuvent ensuite être synchronisés via le rôle Opportunité marketing. L&#39;enregistrement Rôle d&#39;opportunité requiert les champs *externalOpportunityId*, *role* et *leadId* .

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Champ de rôle Opportunité marketing</strong></td> 
   <td><strong>Champ de rôle de contact Salesforce</strong></td> 
   <td><strong>Description</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Identificateur unique global non sensible à la casse pour Salesforce Opportunity</td> 
   <td>Identifie le rôle Opportunité marketing sur un objet Opportunité Salesforce externe.<br><br>Il est obligatoire que l'opportunité Salesforce soit correctement synchronisée en premier.</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>S/O, il s’agirait d’un ID de piste marketing</td> 
   <td>Il s'agit de l'ID de piste marketing du contact Salesforce synchronisé.<br><br>Une fois le contact synchronisé dans Marketo, vous pouvez utiliser l'identifiant unique global non sensible à la casse pour le contact Salesforce en tant que paramètre externePersonId et requête pour le prospect Marketing à l'aide de l'API REST de Marketo.</td> 
  </tr> 
  <tr> 
   <td>rôle</td> 
   <td>Le champ Rôle du contact Salesforce</td> 
   <td>Décrit le rôle du contact pour cette opportunité.</td> 
  </tr> 
 </tbody> 
</table>

Documentation de l&#39;API pour l&#39;opportunité : [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Synchronisez les champs Dernier moment intéressant/Score MSI avec SFDC.

   Une fois que vos objets Salesforce sont correctement synchronisés sur Marketo, vous pouvez profiter des fonctionnalités MSI. Les champs MSI Dernier moment/Score intéressant seront exposés dans l’API REST pour les pistes. Ces champs sont calculés par MSI et sont en lecture seule.

   Les champs Dernier moment/Score intéressant d&#39;une piste marketing devront être régulièrement synchronisés avec Salesforce à l&#39;aide du point de terminaison de piste de l&#39;API REST. Requête de ce point de terminaison pour une piste marketing à l&#39;aide de la variable *externalPersonId* en tant que filterType et transmission du GUID de piste Salesforce en tant que filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Vous pouvez ensuite utiliser les valeurs de ces champs pour synchroniser votre objet de piste/contact Salesforce.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Champ de piste marketing</strong></td> 
   <td><strong>Champ de prospect/contact Salesforce</strong></td> 
   <td><strong>Description</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentType</td> 
   <td>Libellé : Last intéressant Moment<br>TypeName : Last_Intéesting_Moment_Type__c</td> 
   <td>Type du dernier moment intéressant pour la piste</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDate</td> 
   <td><p>Libellé : Date du dernier moment intéressant</p><p>Nom : Last_Intéesting_Moment_Date_c</p></td> 
   <td>Date du dernier moment intéressant pour la piste</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDesc</td> 
   <td><p>Libellé : Description du dernier moment intéressant</p><p>Nom : Last_Intéesting_Moment_Desc__c</p></td> 
   <td>Description du dernier moment intéressant pour la piste</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentSource</td> 
   <td><p>Libellé : Dernière source intéressante</p><p>Nom : Last_Intéesting_Moment_Source__c</p></td> 
   <td>Source du dernier moment intéressant pour la piste</td> 
  </tr> 
  <tr> 
   <td>priority</td> 
   <td><p>Libellé : Engagement</p><p>Nom : Priority__c</p></td> 
   <td>Priorité du responsable</td> 
  </tr> 
  <tr> 
   <td>relativeUrgency</td> 
   <td><p>Libellé : Valeur d’urgence relative</p><p>Nom : Urgency_Value__c</p></td> 
   <td>Urgence relative de la piste</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>Libellé : Valeur de score relative</p><p>Nom : Relative_Score_Value__c</p></td> 
   <td>Score relatif de la piste</td> 
  </tr> 
 </tbody> 
</table>

Documentation de l’API REST de piste :  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/# !/Leads/getLeadByIdUsingGET](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET).

Une bonne utilisation des champs externes est essentielle pour une synchronisation non native réussie. Si les données de certaines vues ne s’affichent pas, il est probable qu’un certain champ n’ait pas été correctement synchronisé. Par exemple, si les activités d&#39;un prospect et les moments intéressants ne s&#39;affichent pas lors de la recherche dans le widget MSI sous son compte, il est probable que la société du prospect ou le compte n&#39;a pas été correctement synchronisé. L&#39;exécution d&#39;une demande de GET pour ce prospect lors de la spécification des champs externes vous aidera à vérifier si le prospect a été correctement synchronisé. En outre, le courrier électronique de la personne chargée des ventes externes dans Marketo doit correspondre à celui de cet utilisateur dans Salesforce. Les données peuvent ne pas s&#39;afficher dans l&#39;onglet Marketo de Salesforce si les courriels ne correspondent pas.

