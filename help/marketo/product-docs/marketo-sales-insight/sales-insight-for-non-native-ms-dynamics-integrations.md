---
description: '[!DNL Sales Insight] pour les intégrations MS [!DNL Dynamics] natives - Documents Marketo - Documentation du produit'
title: '[!DNL Sales Insight] pour les intégrations MS [!DNL Dynamics] natives'
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1228'
ht-degree: 0%

---

# [!DNL Sales Insight] pour les intégrations MS [!DNL Dynamics] non natives {#sales-insight-for-non-native-ms-dynamics-integrations}

Si votre compte Adobe Marketo Engage est connecté à MS [!DNL Dynamics] par le biais d’une intégration personnalisée ou non native, utilisez cet article pour configurer [!DNL Sales Insight].

>[!PREREQUISITES]
>
>* La fonction « MSI non natif » est activée pour votre instance Marketo avant que vous ne commenciez à configurer MSI. Si ce n’est pas le cas et que vous avez déjà acheté la fonctionnalité, contactez l’assistance technique de [Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Si vous n’avez pas encore acheté cette fonctionnalité, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>* Téléchargez [ Package MSI pour la synchronisation personnalisée](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* Un abonnement MS Dynamics avec configuration MSI (pour le moment, nous ne prenons en charge que [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"}).
>* API REST Marketo [configuration réussie](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Les API CRUD exposées seront la base de l’exécution de la synchronisation non native.
>* Lisez [cet article de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} afin de mieux comprendre l’objet et les relations.

## Une synchronisation non native réussie pour MSI nécessite les éléments suivants {#successful-non-native-sync-for-msi-requires-the-following}

1. Synchronisez l’utilisateur commercial MS [!DNL Dynamics] avec Marketo.

   L’utilisateur commercial MS [!DNL Dynamics] est un utilisateur externe qui possède les leads/contacts dans MS [!DNL Dynamics]. Un commercial Marketo doit être mis en place pour le commercial MS [!DNL Dynamics]. Le champ externalSalesPersonId est obligatoire pour la mise à jour du commercial.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ Vendeur Marketo</strong></td> 
        <td><strong>Champ utilisateur MS <span class="dnl">Dynamics</span></strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> Identifiant global unique non sensible à la casse</td> 
      <td><p>Identifie l'enregistrement Vendeur Marketo sur un objet Utilisateur MS <span class="dnl">Dynamics</span> externe.</p><p>Il est obligatoire que le commercial soit synchronisé en premier avant de synchroniser les autres objets afin que les relations appropriées soient créées.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * [Documentation de l’API pour le commercial](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * [Documentation de l’API pour la synchronisation du commercial](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisez les comptes MS [!DNL Dynamics] avec Marketo.

   Une société Marketo devra être insérée pour le compte MS [!DNL Dynamics]. Les champs _externalCompanyId_ et _externalSalesPersonId_ sont obligatoires pour l’upsert de la Société.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ d’entreprise Marketo</strong></td> 
        <td><strong>Champ de compte MS <span class="dnl">Dynamics</span></strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span> Identifiant global unique non sensible à la casse du compte</td> 
        <td>Identifie un enregistrement Société Marketo sur un objet Compte MS <span class="dnl">Dynamics</span> externe.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>Identifiant global unique MS <span class="dnl">Dynamics</span> Sales User non sensible à la casse</td> 
        <td>Identifie un enregistrement Société Marketo sur un objet Utilisateur commercial MS <span class="dnl">Dynamics</span> externe propriétaire du compte.<br><br>Également utilisé dans Marketo pour associer la société au vendeur propriétaire de l'enregistrement de la société. Il est obligatoire de synchroniser le commercial avant de définir ce champ.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour les entreprises : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentation de l’API pour la synchronisation des entreprises : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synchronisez les leads/contacts MS [!DNL Dynamics] avec Marketo.

   Vous devez mettre à jour un lead Marketo pour le lead/contact MS [!DNL Dynamics]. Les champs _externalPersonId_, _externalSalesPersonId_ et _externalCompanyId_ sont obligatoires pour l&#39;upsert du lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ de lead Marketo</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> Champ de lead/contact</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> Identifiant global unique non sensible à la casse du lead/contact</td> 
        <td>Identifie l’enregistrement Lead Marketo sur un objet MS <span class="dnl">Dynamics</span> Lead/Contact externe.<br><br>Il s’agit d’un nouveau champ introduit pour MSI non natif.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>Identifiant global unique MS <span class="dnl">Dynamics</span> Sales User non sensible à la casse</td> 
        <td>Identifie l'objet MS <span class="dnl">Dynamics</span> Sales User externe propriétaire de ce lead/contact.<br><br> Associe également le prospect au commercial dans Marketo. Il est obligatoire que le commercial soit correctement synchronisé en premier.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span> Identifiant global unique non sensible à la casse du compte</td> 
        <td>Identifie l’objet MS <span class="dnl">Dynamics</span> Account externe auquel le lead/contact appartient.<br><br>Associe également l’enregistrement de prospect à une société dans Marketo. Il est obligatoire que le compte MS <span class="dnl">Dynamics</span> soit correctement synchronisé en premier.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour les leads : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database){target="_blank"}
   * Documentation de l’API pour la synchronisation des prospects : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}

1. Synchronisez les opportunités de [!DNL Dynamics] MS avec Marketo.

   Vous devez mettre à jour une opportunité Marketo pour l’opportunité MS [!DNL Dynamics]. Les champs _externalOpportunityId_, _externalCompanyId_ et _externalSalesPersonId_ sont obligatoires pour l’upsert de l’opportunité.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ d’objet de l’opportunité Marketo</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> Champ d’objet d’opportunité</strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
        <td>MS <span class="dnl">Dynamics</span> Identifiant global unique non sensible à la casse du lead/contact</td> 
      <td>Identifie l’enregistrement d’opportunité Marketo sur un objet d’opportunité MS <span class="dnl">Dynamics</span> externe.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span> Identifiant global unique non sensible à la casse du compte</td> 
        <td>Identifie l’objet compte MS <span class="dnl">Dynamics</span> externe auquel cette opportunité appartient. <br><br>Il est obligatoire que le compte MS <span class="dnl">Dynamics</span> soit correctement synchronisé en premier.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>Identifiant global unique MS <span class="dnl">Dynamics</span> Sales User non sensible à la casse</td> 
        <td>Identifie l’objet Utilisateur commercial MS <span class="dnl">Dynamics</span> externe propriétaire de cette opportunité. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour Opportunité : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentation de l’API pour la synchronisation des opportunités : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisez les rôles de contact MS [!DNL Dynamics] avec Marketo.

   Les rôles de contact MS [!DNL Dynamics] d’une opportunité MS [!DNL Dynamics] peuvent ensuite être synchronisés via le rôle d’opportunité Marketo. L’enregistrement Rôle de l’opportunité rend obligatoires les champs _externalOpportunityId_, _role_ et _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ Rôle de l’opportunité Marketo</strong></td> 
        <td><strong>Champ Rôle du contact MS <span class="dnl">Dynamics</span></strong></td> 
      <td><strong>Description</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
        <td>Identifiant global unique MS <span class="dnl">Dynamics</span> non sensible à la casse des opportunités</td> 
      <td>Identifie le rôle d’opportunité Marketo sur un objet d’opportunité MS <span class="dnl">Dynamics</span> externe.<br><br>Il est obligatoire que l’opportunité MS <span class="dnl">Dynamics</span> soit correctement synchronisée en premier.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>S.O., il s’agirait d’un ID de lead Marketo</td> 
        <td>Il s’agit de l’ID de lead Marketo du contact MS <span class="dnl">Dynamics</span> synchronisé.<br><br>Une fois le contact synchronisé dans Marketo, vous pouvez utiliser l’identifiant global unique MS <span class="dnl">Dynamics</span> qui ne respecte pas la casse du contact en tant qu’externalPersonId et interroger le prospect Marketo à l’aide de l’API REST Marketo.</td> 
     </tr> 
     <tr> 
      <td>Rôle</td> 
        <td>Le champ Rôle pour le contact MS <span class="dnl">Dynamics</span></td> 
      <td>Décrit le rôle du contact pour cette opportunité.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentation de l’API pour Opportunité : [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentation de l’API pour la synchronisation des opportunités : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synchronisez les champs de dernier moment intéressant/Score MSI avec MS [!DNL Dynamics].

   Une fois que vos objets MS [!DNL Dynamics] sont correctement synchronisés avec Marketo, vous pouvez tirer parti des fonctionnalités MSI. Les champs Dernier moment intéressant/Score MSI seront exposés dans l’API REST pour les prospects. Ces champs sont calculés par MSI et sont en lecture seule.

   Les champs Dernier moment intéressant/Score d’un lead Marketo devront être régulièrement synchronisés avec MS [!DNL Dynamics] à l’aide du point d’entrée de lead de l’API REST. Interrogez ce point d’entrée pour un prospect Marketo à l’aide de _externalPersonId_ comme filterType et en transmettant le GUID de prospect MS [!DNL Dynamics] comme filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   Vous pouvez ensuite utiliser les valeurs de ces champs pour les synchroniser avec votre objet de lead/contact MS [!DNL Dynamics].

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Champ de lead Marketo</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> Champ de lead/contact</strong></td> 
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

   * Documentation pour l’API REST de lead : [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   L’utilisation appropriée des champs externes est essentielle pour une synchronisation non native réussie. Si vous ne parvenez pas à voir les données dans certaines vues, il est probable qu’un certain champ n’ait pas été correctement synchronisé. Par exemple, si les activités et les moments intéressants d’un prospect ne s’affichent pas lors de la recherche dans le widget MSI sous son compte, il est probable que la société du prospect ou le compte n’ait pas été correctement synchronisé. L’exécution d’une requête GET pour ce prospect lors de la spécification des champs externes vous aidera à vérifier si le prospect a été correctement synchronisé. De plus, l’adresse e-mail du commercial externe dans Marketo doit correspondre à celle de cet utilisateur dans MS Dynamics. Les données peuvent ne pas s’afficher dans l’onglet Marketo de MS Dynamics si les e-mails ne correspondent pas.
