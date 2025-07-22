---
unique-page-id: 45417125
description: '[!DNL Sales Insight] pour les intégrations  [!DNL Salesforce]  natives - Documents Marketo - Documentation du produit'
title: '[!DNL Sales Insight] pour les intégrations  [!DNL Salesforce] '
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 0%

---

# [!DNL Sales Insight] pour les intégrations [!DNL Salesforce] non natives {#sales-insight-for-non-native-salesforce-integrations}

Si votre compte Adobe Marketo Engage est connecté à [!DNL Salesforce] par le biais d’une intégration personnalisée ou non native, utilisez cet article pour configurer [!DNL Sales Insight].

>[!PREREQUISITES]
>
>* La fonction « MSI non natif » est activée pour votre instance Marketo avant que vous ne commenciez à configurer MSI. Si ce n’est pas le cas et que vous avez déjà acheté la fonctionnalité, contactez l’assistance technique de [Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Si vous n’avez pas encore acheté cette fonctionnalité, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>* Un compte Salesforce avec [configuration du package MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* API REST Marketo [configuration réussie](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Les API CRUD exposées seront la base de l’exécution de la synchronisation non native.
>* Lisez [cet article de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} afin de mieux comprendre l’objet et les relations.
>* Configurez les objets [!DNL Salesforce] pour afficher l’identifiant global unique non sensible à la casse de 18 caractères au lieu de l’identifiant global unique sensible à la casse de 15 caractères.

>[!NOTE]
>
>La configuration de l’API REST dans le panneau d’administration MSI de Marketo ne peut pas être utilisée pour la synchronisation non native.

## Une synchronisation non native réussie pour MSI nécessite les éléments suivants {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchronisez l’utilisateur commercial [!DNL Salesforce] à Marketo.

   L’utilisateur commercial [!DNL Salesforce] est un utilisateur externe qui possède les leads/contacts dans [!DNL Salesforce]. Un commercial Marketo doit être mis en place pour l’utilisateur commercial [!DNL Salesforce]. Le champ *externalSalesPersonId* est obligatoire pour l’upsert du commercial.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ Vendeur Marketo</strong></td> 
        <td><strong><span class="dnl">Salesforce </span> Champ Utilisateur Commercial</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse pour l'utilisateur commercial</td> 
      <td><p>Identifie l'enregistrement Vendeur Marketo sur un objet Utilisateur commercial <span class="dnl">Salesforce</span> externe.</p><p>Il est obligatoire que le commercial soit synchronisé en premier avant de synchroniser les autres objets afin que les relations appropriées soient créées.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour le commercial : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * Documentation de l’API pour la synchronisation du commercial : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisez les comptes [!DNL Salesforce] avec Marketo.

   Une société Marketo devra être insérée pour le compte [!DNL Salesforce]. Les champs _externalCompanyId_ et _externalSalesPersonId_ sont obligatoires pour l’upsert de la Société.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ d’entreprise Marketo</strong></td> 
        <td><strong>Champ de compte <span class="dnl">Salesforce</span></strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse du compte</td> 
        <td>Identifie un enregistrement Société Marketo sur un objet Compte <span class="dnl">Salesforce</span> externe.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse pour l'utilisateur commercial</td> 
        <td>Identifie un enregistrement Société Marketo sur un objet Utilisateur commercial <span class="dnl">Salesforce</span> externe propriétaire du compte.<br><br>Également utilisé dans Marketo pour associer la société au vendeur propriétaire de l'enregistrement de la société. Il est obligatoire de synchroniser le commercial avant de définir ce champ.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour les entreprises : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentation de l’API pour la synchronisation des entreprises : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Synchronisez les leads/contacts [!DNL Salesforce] à Marketo.

   Vous devez mettre à jour un prospect Marketo pour le prospect/contact [!DNL Salesforce]. Les champs _externalPersonId_, _externalSalesPersonId_ et _externalCompanyId_ sont obligatoires pour l&#39;upsert du lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ de lead Marketo</strong></td> 
        <td><strong><span class="dnl">Salesforce</span> Champ de lead/contact</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse du lead/contact</td> 
        <td>Identifie l’enregistrement Lead Marketo sur un objet externe <span class="dnl">Salesforce</span> Lead/Contact.<br><br>Il s’agit d’un nouveau champ introduit pour MSI non natif.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse pour l'utilisateur commercial</td> 
        <td>Identifie l'objet externe <span class="dnl">Salesforce</span> Sales User propriétaire de ce lead/contact.<br><br> Associe également le prospect au commercial dans Marketo. Il est obligatoire que le commercial soit correctement synchronisé en premier.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse du compte</td> 
        <td>Identifie l'objet compte <span class="dnl">Salesforce</span> externe auquel le lead/contact appartient.<br><br>Associe également l’enregistrement de prospect à une société dans Marketo. Il est obligatoire que le compte Salesforce soit correctement synchronisé en premier.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour les leads : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads)
   * Documentation de l’API pour la synchronisation des prospects : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Synchronisez [!DNL Salesforce] opportunités avec Marketo.

   Vous devez mettre à jour une opportunité Marketo pour l’opportunité [!DNL Salesforce]. Les champs _externalOpportunityId_, _externalCompanyId_ et _externalSalesPersonId_ sont obligatoires pour l’upsert de l’opportunité.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ d’objet de l’opportunité Marketo</strong></td> 
        <td><strong><span class="dnl">Salesforce</span> Champ D’Objet D’Opportunité</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identifiant global unique non sensible à la casse du lead/contact Salesforce</td> 
      <td>Identifie l’enregistrement d’opportunité Marketo sur un objet d’opportunité Salesforce externe.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse du compte</td> 
        <td>Identifie l’objet Compte <span class="dnl">Salesforce</span> externe auquel cette opportunité appartient. <br><br>Il est obligatoire que le compte <span class="dnl">Salesforce</span> soit correctement synchronisé en premier.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse pour l'utilisateur commercial</td> 
        <td>Identifie l'objet Utilisateur commercial <span class="dnl">Salesforce</span> externe propriétaire de cette opportunité. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour Opportunité : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentation de l’API pour la synchronisation des opportunités : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisez [!DNL Salesforce] rôles de contact avec Marketo.

   [!DNL Salesforce] rôles de contact d’une opportunité [!DNL Salesforce] peuvent ensuite être synchronisés via le rôle d’opportunité Marketo. L’enregistrement Rôle de l’opportunité rend obligatoires les champs _externalOpportunityId_, _role_ et _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ Rôle de l’opportunité Marketo</strong></td> 
      <td><strong>Champ Rôle du contact Salesforce</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
        <td><span class="dnl">Salesforce </span> Identifiant global unique non sensible à la casse pour l’opportunité</td> 
        <td>Identifie le rôle d’opportunité Marketo sur un objet d’opportunité <span class="dnl">Salesforce</span> externe.<br><br>L’opportunité <span class="dnl">Salesforce</span> doit d’abord être correctement synchronisée.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>S.O., il s’agirait d’un ID de lead Marketo</td> 
        <td>Il s’agit de l’ID de lead Marketo du contact <span class="dnl">Salesforce</span> synchronisé.<br><br>Une fois le contact synchronisé dans Marketo, vous pouvez utiliser l’identifiant global unique <span class="dnl">Salesforce</span> qui ne respecte pas la casse, en tant qu’externalPersonId et interroger le prospect Marketo à l’aide de l’API REST Marketo.</td> 
     </tr> 
     <tr> 
      <td>Rôle</td> 
        <td>Champ Rôle du contact <span class="dnl">Salesforce</span></td> 
      <td>Décrit le rôle du contact pour cette opportunité.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour Opportunité : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentation de l’API pour la synchronisation des opportunités : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisez les champs de dernier moment intéressant/Score MSI avec SFDC.

   Une fois que vos objets [!DNL Salesforce] sont correctement synchronisés avec Marketo, vous pouvez tirer parti des fonctionnalités MSI. Les champs Dernier moment intéressant/Score MSI seront exposés dans l’API REST pour les prospects. Ces champs sont calculés par MSI et sont en lecture seule.

   Les champs Dernier moment intéressant/Score d’un lead Marketo devront être régulièrement synchronisés avec [!DNL Salesforce] à l’aide du point d’entrée de lead de l’API REST. Interrogez ce point d’entrée pour un prospect Marketo à l’aide de _externalPersonId_ comme filterType et en transmettant le GUID de prospect [!DNL Salesforce] comme filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Vous pouvez ensuite utiliser les valeurs de ces champs pour les synchroniser avec votre objet de lead/contact [!DNL Salesforce].

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ de lead Marketo</strong></td> 
        <td><strong><span class="dnl">Salesforce</span> Champ de lead/contact</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentType</td> 
      <td>Libellé : Dernier moment intéressant Type<br>Nom : Last_Interesting_Moment_Type__c</td> 
      <td>Type du dernier moment intéressant pour le lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDate</td> 
      <td><p>Libellé : Date du dernier moment intéressant</p><p>Nom : Last_Interesting_Moment_Date__c</p></td> 
      <td>Date du dernier moment intéressant pour le lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDesc</td> 
      <td><p>Libellé : Description du dernier moment intéressant</p><p>Nom : Last_Interesting_Moment_Desc__c</p></td> 
      <td>Description du dernier moment intéressant pour le lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentSource</td> 
      <td><p>Libellé : Source du dernier moment intéressant</p><p>Nom : Last_Interesting_Moment_Source__c</p></td> 
      <td>Source du dernier moment intéressant pour le lead</td> 
     </tr> 
     <tr> 
      <td>priorité</td> 
      <td><p>Libellé : Engagement</p><p>Nom : Priorité__c</p></td> 
      <td>Priorité du lead</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>Libellé : valeur d’urgence relative</p><p>Nom : Urgency_Value__c</p></td> 
      <td>Urgence relative du lead</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Libellé : valeur de score relative</p><p>Nom : Relative_Score_Value__c</p></td> 
      <td>Score relatif du lead</td> 
     </tr> 
    </tbody> 
   </table>

   Documentation pour l’API REST de lead : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   L’utilisation appropriée des champs externes est essentielle pour une synchronisation non native réussie. Si vous ne parvenez pas à voir les données dans certaines vues, il est probable qu’un certain champ n’ait pas été correctement synchronisé. Par exemple, si les activités et les moments intéressants d’un prospect ne s’affichent pas lors de la recherche dans le widget MSI sous son compte, il est probable que la société du prospect ou le compte n’ait pas été correctement synchronisé. L’exécution d’une requête GET pour ce prospect lors de la spécification des champs externes vous aidera à vérifier si le prospect a été correctement synchronisé. De plus, l’adresse e-mail du commercial externe dans Marketo doit correspondre à celle de cet utilisateur dans Salesforce. Les données peuvent ne pas s’afficher dans l’onglet Marketo de Salesforce si les e-mails ne correspondent pas.
