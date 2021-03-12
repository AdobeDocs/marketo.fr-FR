---
description: Octroi d’un consentement pour l’ID de client et l’enregistrement d’application - Documents marketing - Documentation du produit
title: Octroi d’un consentement pour l’ID de client et l’enregistrement d’application
translation-type: tm+mt
source-git-commit: 3a6d9987e214aa8606b9f5abdc780a81355b1001
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---


# Octroi d’un consentement pour l’ID de client et l’enregistrement d’application {#grant-consent-for-client-id-and-app-registration}

## Octroi d’autorisations d’utilisateur délégué à l’utilisateur de synchronisation {#grant-delegated-user-permissions-for-the-sync-user}

1. Utilisez un programme de texte propre (Bloc-notes pour Windows, Modification de texte pour Mac) pour créer un URI (Uniform Resource Identifier) pour l’autorisation en collant le texte ci-dessous et en substituant les valeurs client_id, redirect_uri et state.

   ```
   https://login.microsoftonline.com/common/oauth2/authorize?
   client_id='xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx'
   &response_type='code'
   &redirect_uri='https://www.<ourdomain>.com'
   &response_mode='query'
   &state='SOME_UNIQUE_UID'
   client_id value should be the client_id generated in App Registration process
   redirect_uri value should be same as value entered at the time of App registration-> Redirect URIs
   state value can be any ID (e.g.,12345)
   ```

   <table> 
    <colgroup> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>valeur client_id</strong></td> 
      <td>doit être l’ID_client généré dans le processus d’enregistrement de l’application.</td> 
     </tr> 
     <tr> 
      <td><strong>valeur redirect_uri</strong></td> 
      <td>doit être identique à la valeur saisie au moment de l’enregistrement de l’application &gt; URI de redirection</td> 
     </tr> 
     <tr> 
      <td><strong>valeur d’état</strong></td> 
      <td>peut être n’importe quel ID (ex. : 12345)</td> 
     </tr> 
    </tbody> 
   </table>

   L’URL finale doit ressembler à ceci : `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. Ouvrez l’URI que vous avez créé dans n’importe quel navigateur.

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. Connectez-vous en tant qu’utilisateur de synchronisation pour lequel vous accordez des autorisations.

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >Si vous êtes déjà connecté à Azure en tant qu&#39;administrateur dans un autre onglet, vous devrez utiliser un autre navigateur ou mode Incognito pour vous connecter en tant qu&#39;utilisateur de synchronisation.

1. Cliquez sur **Accepter**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Octroi du consentement à tous les utilisateurs {#grant-consent-for-all-users}

En tant qu’administrateur, vous pouvez également consentir aux autorisations déléguées d’une application au nom de tous les utilisateurs de votre client. Le consentement administratif empêche l&#39;affichage de la boîte de dialogue de consentement pour chaque utilisateur dans le client et peut être effectué dans le portail Azure par les utilisateurs ayant le rôle d&#39;administrateur. Pour savoir quels rôles d&#39;administrateur peuvent [consentir à des autorisations déléguées, cliquez ici](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. Dans votre portail Azure, accédez à la page d&#39;accueil de l&#39;application.

1. Sous Gérer, cliquez sur **Autorisations d&#39;API**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Cliquez sur le bouton **Octroyer le consentement de l’administrateur** (pour le client).

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Cliquez sur **Oui** pour confirmer.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

>[!MORELIKETHIS]
>
>[Configuration de l&#39;application Microsoft Dynamics CRM pour On-Prem](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/set-up-microsoft-dynamics-crm-app-for-on-prem.md)
