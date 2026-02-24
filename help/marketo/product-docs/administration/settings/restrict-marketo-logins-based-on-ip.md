---
unique-page-id: 2360297
description: Restreindre les connexions Marketo en fonction de l’adresse IP - Documents Marketo - Documentation du produit
title: Restreindre les connexions à Marketo en fonction de l’adresse IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: b6680c404075f13b1713ce28299e60a4d26f4a06
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 7%

---

# Restreindre les connexions à Marketo en fonction de l’adresse IP {#restrict-marketo-logins-based-on-ip}

Vous pouvez empêcher ou autoriser des utilisateurs à accéder à Marketo en fonction de leurs adresses IP. Voici comment faire.

>[!NOTE]
>
>**Autorisations d’administration requises**

>[!IMPORTANT]
>
>Adobe Admin Console (AAC) prend en charge le [contrôle d’accès basé sur IP](https://helpx.adobe.com/fr/enterprise/using/ip-based-access.html){target="_blank"}. Pour garantir une transition en douceur, les restrictions IP Marketo Engage existantes seront actives, y compris pour les utilisateurs d’Adobe ID jusqu’au 1er trimestre 2027 dans les abonnements où cette fonctionnalité est activée.
>
>* Vous pouvez configurer l’accès basé sur l’adresse IP AAC à tout moment.
>* Les restrictions AAC et Marketo Engage peuvent s’exécuter simultanément. Utilisez la même liste autorisée IP pour la compatibilité.
>
>Après le 1er trimestre 2027, les restrictions IP de Marketo Engage seront supprimées. L’accès basé sur les adresses IP sera géré exclusivement par l’intermédiaire d’AAC et doit être configuré pour appliquer les restrictions de connexion. Une date de transition définitive sera annoncée ultérieurement.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Cliquez sur **[!UICONTROL Paramètres de connexion]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Cliquez sur **[!UICONTROL Modifier les restrictions IP]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Choisissez si vous souhaitez **Autoriser** ou **Bloquer** des adresses spécifiques, saisissez la ou les adresses, puis cliquez sur **[!UICONTROL Enregistrer]**.

   >[!NOTE]
   >
   >**Définition**
   >
   >* **[!UICONTROL Adresses IP autorisées]** : l’ajout d’adresses IP autorisées est un processus d’inclusion. Elle inclut toutes les adresses IP spécifiées et exclut tout le reste.
   >* **[!UICONTROL Bloquer les adresses IP]** : empêche des adresses IP spécifiques d’accéder à Marketo.
   >* **[!UICONTROL Désactiver les restrictions IP]** : si vous cochez cette case, toutes les règles de restriction cesseront de fonctionner. Utilisez-le à des fins de test.

   >[!NOTE]
   >
   >Vous pouvez ajouter plusieurs restrictions, mais elles peuvent uniquement être AUTORISÉES POUR TOUT ou BLOQUÉES POUR TOUT. Vous ne pouvez pas mélanger et faire correspondre les valeurs autorisées et bloquées.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)
