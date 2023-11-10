---
description: Accorder le consentement pour l’ID de client et l’enregistrement d’application - Documents Marketo - Documentation du produit
title: Octroi du consentement pour l’ID de client et l’enregistrement de l’application
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Octroi du consentement pour l’ID de client et l’enregistrement de l’application {#grant-consent-for-client-id-and-app-registration}

Suivez les étapes ci-dessous pour savoir comment accorder le consentement/les autorisations nécessaires.

## Octroi d’autorisations d’utilisateur déléguées à l’utilisateur de synchronisation {#grant-delegated-user-permissions-for-the-sync-user}

1. Utilisez un programme de texte clair (Bloc-notes pour Windows, Édition de texte pour Mac) pour créer un URI (Uniform Resource Identifier) d’autorisation en collant le texte ci-dessous et en substituant les valeurs client_id, redirect_uri et state.

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
      <td>doit être client_id généré dans le processus d’enregistrement de l’application</td> 
     </tr> 
     <tr> 
      <td><strong>valeur redirect_uri</strong></td> 
      <td>doit être identique à la valeur saisie au moment de l’enregistrement de l’application &gt; URI de redirection</td> 
     </tr> 
     <tr> 
      <td><strong>valeur d’état</strong></td> 
      <td>peut être n’importe quel ID (par exemple, 12345).</td> 
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
   >Si vous êtes déjà connecté à Azure en tant qu’administrateur dans un autre onglet, vous devrez utiliser un autre navigateur ou mode Incognito pour vous connecter en tant qu’utilisateur de synchronisation.

1. Cliquez sur **[!UICONTROL Accepter]**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Octroi du consentement à tous les utilisateurs {#grant-consent-for-all-users}

En tant qu’administrateur, vous pouvez également consentir aux autorisations déléguées d’une application au nom de tous les utilisateurs de votre client. Le consentement administratif empêche l’affichage de la boîte de dialogue de consentement pour chaque utilisateur du client et peut être effectué sur le portail Azure par les utilisateurs dotés du rôle d’administrateur. Découvrez quels rôles d’administrateur peuvent [consentement aux autorisations déléguées ici](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. Dans votre portail Azure, accédez à la page d’accueil de l’application.

1. Sous Gérer, cliquez sur **[!UICONTROL Autorisations d’API]**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Cliquez sur le bouton **[!UICONTROL Autorisation du consentement de l’administrateur]** (pour le client).

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Cliquez sur **[!UICONTROL Oui]** pour confirmer.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)
