---
unique-page-id: 2949711
description: Installez le complément de messagerie Marketo pour Outlook avec un code d'enregistrement - Marketo Docs - Documentation du produit
title: Installer le complément de messagerie Marketo pour Outlook avec un code d'enregistrement
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: ac6c84a82b9bcb535d5f50897d1a068a5a746287
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 6%

---

# Installer le complément de messagerie Marketo pour Outlook avec un code d&#39;enregistrement {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Si les utilisateurs peuvent accéder aux paramètres d’administration sur leurs ordinateurs portables, vous pouvez leur envoyer directement un code d’enregistrement.

Si vous n’avez pas reçu d’e-mail d’invitation, demandez à votre administrateur Marketo de vous inviter.

>[!PREREQUISITES]
>
>Vous devez recevoir [une licence de complément d’e-mail Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>L&#39;installation n&#39;est pas prise en charge sur les PC où le dossier Utilisateur Windows contient des caractères non anglais. Ce dossier est généré automatiquement par Windows sous `<System Root>\Users\` en fonction du nom d&#39;utilisateur Windows et peut contenir des caractères non anglais si le nom d&#39;utilisateur Windows est un nom non anglais. Contactez votre équipe informatique pour vérifier si vous rencontrez des problèmes d’installation.

>[!NOTE]
>
>Les fonctionnalités Actions de Sales Insight, notamment Envoyer un e-mail de vente, Ajouter à la campagne de vente et Tâches, ne sont pas disponibles dans les plug-ins de messagerie de Sales Insight pour Gmail et Outlook. Actuellement, les utilisateurs ne peuvent envoyer qu’un e-mail trackable avec ou sans modèle d’e-mail Marketo à partir de leur client de messagerie lors de l’utilisation des modules externes d’e-mail Sales Insight.

## Télécharger le programme d’installation {#download-installer}

1. Identifiez votre [version Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}.

1. Dans le tableau ci-dessous, cliquez sur le lien pour télécharger le fichier .ZIP correspondant à votre version de Microsoft Outlook.

1. Décompressez le fichier pour accéder au fichier .MSI nécessaire et poursuivre l’installation.

   >[!NOTE]
   >
   >Actuellement, les liens ci-dessous ne fonctionnent que dans Microsoft Edge ou en cliquant avec le bouton droit de la souris dans Chrome. Nous sommes désolés pour la gêne occasionnée.

<table><thead>
  <tr>
    <th>Version Outlook</th>
    <th>Outlook 32 bits</th>
    <th>Outlook 64 bits</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Outlook 2000</td>
    <td>Non pris en charge</td>
    <td>S/O</td>
  </tr>
  <tr>
    <td>Outlook 2003</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Téléchargement</a></td>
    <td>S/O</td>
  </tr>
  <tr>
    <td>Outlook 2007</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Téléchargement</a></td>
    <td>S/O</td>
  </tr>
  <tr>
    <td>Outlook 2010</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Téléchargement</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Téléchargement</a></td>
  </tr>
  <tr>
    <td>Outlook 2013</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Téléchargement</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Téléchargement</a></td>
  </tr>
  <tr>
    <td>Outlook 2016</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Téléchargement</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Téléchargement</a></td>
  </tr>
  <tr>
    <td>Outlook 2019</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Téléchargement</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Téléchargement</a></td>
  </tr>
  <tr>
    <td>Outlook pour Mac</td>
    <td>Non pris en charge</td>
    <td>Non pris en charge</td>
  </tr>
  <tr>
    <td>Outlook Web App</td>
    <td>Non pris en charge</td>
    <td>Non pris en charge</td>
  </tr>
  <tr>
    <td>Office 365*</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Téléchargement</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Téléchargement</a></td>
  </tr>
</tbody></table>

*Version Office 365 : client Windows uniquement (sous Windows 10, Enterprise ou Pro).

>[!IMPORTANT]
>
>Microsoft a publié une [nouvelle version d&#39;Outlook pour Windows](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}. Cette nouvelle version ne prend pas en charge le plug-in MSI Outlook existant. Le plug-in MSI Outlook continuera à fonctionner pour les ordinateurs de bureau Windows exécutant la version classique d&#39;Outlook. Pour en savoir plus sur la nouvelle version d&#39;Outlook pour Windows pour les organisations, [cliquez ici](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}.

## Copiez votre code d’enregistrement {#copy-your-registration-code}

1. Copiez le code d’enregistrement de l’e-mail d’invitation que vous avez reçu.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Fermez Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

## Installer {#install}

1. Exécutez le programme d’installation.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Si vous recevez un avertissement de sécurité, ne vous inquiétez pas ! Cliquez simplement sur **Exécuter**.

1. Cliquez sur **Suivant**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Renseignez **Prénom**, **Nom** et **Adresse e-mail**, puis copiez et collez le **Code d’enregistrement** de l’e-mail dans le formulaire et cliquez sur **Suivant**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Si l’installation échoue, contactez votre service informatique pour vous assurer que le trafic HTTPS n’est pas bloqué. Le programme d’installation nécessite l’ouverture du trafic HTTPS.

1. Cliquez sur **Suivant** pour effectuer l’installation à l’emplacement par défaut.

   ![](assets/select-installation-folder-hand.png)

1. Cliquez sur **Suivant**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Si vous recevez une invite de sécurité concernant un éditeur inconnu, cliquez sur **Oui**.

1. L&#39;installation est terminée, cliquez sur **Fermer**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Ouvrez maintenant Microsoft Outlook et affichez les boutons Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Excellent ! Désormais, les boutons Marketo sont mieux placés.

En savoir plus sur l’utilisation des actions Message et Se connecter avec Marketo de Marketo.

>[!MORELIKETHIS]
>
>* [Envoyer et suivre un e-mail avec le complément d&#39;e-mail Marketo pour Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Envoi et suivi depuis Outlook à l&#39;aide d&#39;un modèle Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
