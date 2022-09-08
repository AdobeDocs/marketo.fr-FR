---
unique-page-id: 2949711
description: Installation du module complémentaire de messagerie Marketo pour Outlook avec un code d’enregistrement - Documents Marketo - Documentation du produit
title: Installation du module complémentaire de messagerie Marketo pour Outlook avec un code d’enregistrement
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
source-git-commit: 0dec1dc142a7296ce9d5db91493f654dbe7ee99a
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 5%

---

# Installation du module complémentaire de messagerie Marketo pour Outlook avec un code d’enregistrement {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Si les utilisateurs peuvent accéder aux paramètres d’administration sur leurs ordinateurs portables, vous pouvez leur envoyer directement un code d’enregistrement.

Si vous n’avez pas reçu de courrier électronique d’invitation, demandez à votre administrateur Marketo de vous inviter.

>[!PREREQUISITES]
>
>Vous devez être [Envoi d’une licence de module complémentaire de messagerie Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>L’installation n’est pas prise en charge sur les PC où le dossier des utilisateurs Windows contient des caractères non anglais. Ce dossier est généré automatiquement par Windows sous <System Root>\Users\ en fonction du nom d’utilisateur Windows et peut contenir des caractères non anglais si le nom d’utilisateur Windows est un nom non anglais. Contactez votre équipe informatique pour vérifier si vous rencontrez des problèmes d’installation.

>[!NOTE]
>
>Le 10/1/20, la dernière version du module externe Outlook a cessé de prendre en charge le mode hors ligne.

## Télécharger le programme {#download-installer}

1. Identifiez votre [Version de Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c)

1. Cliquez sur le lien pour télécharger le programme d’installation approprié à votre version de Microsoft Outlook.

   >[!NOTE]
   >
   >Actuellement, les liens ci-dessous ne fonctionnent que dans Microsoft Edge ou en cliquant avec le bouton droit de la souris dans Chrome. Désolé pour tout désagrément.

   | Version d’Outlook | Outlook 32 bits | Outlook 64 bits |
   |---|---|---|
   | Outlook 2000 | Non pris en charge | S/O |
   | Outlook 2003 | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | S/O |
   | Outlook 2007 | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | S/O |
   | Outlook 2010 | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook pour Mac | Non pris en charge | Non pris en charge |
   | Outlook Web App | Non pris en charge | Non pris en charge |
   | Office 365* | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Télécharger](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Version d’Office 365 : Client Windows uniquement (sous Windows 10, Enterprise ou Pro).

## Copie de votre code d’enregistrement {#copy-your-registration-code}

1. Copiez le code d’enregistrement du courrier électronique d’invitation que vous avez reçu.

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

1. Remplir **Prénom**, **Nom**, **Adresse électronique**, puis copiez et collez le **Code d’enregistrement** dans le formulaire, puis cliquez sur **Suivant**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Si l’installation échoue, vérifiez auprès de votre service informatique que le trafic HTTPS n’est pas bloqué. Le programme d’installation nécessite l’ouverture du trafic HTTPS.

1. Cliquez sur **Suivant** pour effectuer l’installation à l’emplacement par défaut.

   ![](assets/select-installation-folder-hand.png)

1. Cliquez sur **Suivant**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Si vous recevez une invite de sécurité concernant un éditeur inconnu, cliquez sur **Oui**.

1. L’installation est maintenant terminée, cliquez sur **Fermer**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Ouvrez maintenant Microsoft Outlook et affichez les boutons Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Excellent ! Les boutons de Marketo sont désormais mieux placés.

En savoir plus sur l’utilisation des actions Marketo Message et Log With Marketo .

>[!MORELIKETHIS]
>
>* [Envoi et suivi d’un courrier électronique avec le module complémentaire de messagerie Marketo pour Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Envoi et suivi depuis Outlook à l’aide d’un modèle Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

