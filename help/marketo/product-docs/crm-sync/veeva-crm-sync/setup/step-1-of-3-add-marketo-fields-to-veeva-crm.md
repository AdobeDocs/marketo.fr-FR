---
description: Étape 1 sur 3 - Ajout de champs Marketo à  [!DNL Veeva]  CRM - Documentation de Marketo - Documentation du produit
title: Étape 1 sur 3 - Ajout de champs Marketo à  [!DNL Veeva]  CRM
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 8%

---

# Étape 1 sur 3 : ajouter des champs Marketo à [!DNL Veeva] CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>Votre instance CRM [!DNL Veeva] doit avoir accès aux API Salesforce pour synchroniser les données entre Marketo Engage et [!DNL Veeva] CRM.

Marketo Engage utilise un ensemble de champs pour capturer certains types d’informations liées au marketing. Si vous souhaitez obtenir ces données dans [!DNL Veeva] CRM, suivez les instructions ci-dessous.

`1.` Créer un champ personnalisé dans [!DNL Veeva] CRM sur les objets de contact : Score

`2.` Si vous le souhaitez, vous pouvez créer des champs supplémentaires (voir le tableau ci-dessous).

Tous ces champs personnalisés sont facultatifs et ne sont pas obligatoires pour synchroniser Marketo Engage et [!DNL Veeva] CRM.

## Ajout de champs Marketo à [!DNL Veeva] CRM {#add-marketo-fields-to-veeva-crm}

Ajoutez un champ personnalisé sur les objets de lead et de contact dans [!DNL Veeva] CRM répertorié ci-dessus. Si vous souhaitez en ajouter d&#39;autres, consultez le tableau des champs disponibles à la fin de cette section.

Effectuez les étapes suivantes pour que le champ Score l’ajoute.

1. Connectez-vous au CRM [!DNL Veeva] et cliquez sur **[!UICONTROL Configuration]**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Cliquez sur **[!UICONTROL Objets et champs]** et sélectionnez **[!UICONTROL Gestionnaire d’objets]**.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. Dans la barre de recherche, recherchez « Contact ».

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Cliquez sur l’objet **[!UICONTROL Contact]**.

1. Sélectionnez **[!UICONTROL Champs et relations]**.

1. Cliquez sur **[!UICONTROL Nouveau]**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Sélectionnez le type de champ approprié (pour Score - nombre).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Saisissez les **[!UICONTROL Libellé du champ]**, **[!UICONTROL Longueur]** et **[!UICONTROL Nom du champ]** pour le champ, comme illustré dans le tableau ci-dessous.

<table>
 <tbody>
  <tr>
   <th>Intitulé de champ
   <th>Nom du champ
   <th>Type de données
   <th>Attributs de champ
  </tr>
  <tr>
   <td>Score</td>
   <td>mkto71_Lead_Score</td>
   <td>Nombre</td>
   <td>Longueur 10<br/>
Nombre de décimales 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>[!DNL Veeva] CRM ajoute __c aux noms de champ lorsqu’il les utilise pour créer des noms d’API.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>Les champs de texte et de nombre nécessitent une longueur, mais pas les champs Date/Heure. Une description est facultative.

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Spécifiez les paramètres d’accès et cliquez sur **[!UICONTROL Suivant]**.

1. Définissez tous les rôles sur **[!UICONTROL Visible]** et **[!UICONTROL Lecture seule]**.

1. Désélectionnez la case **[!UICONTROL Lecture seule]** pour le profil de l’utilisateur de synchronisation :

* Si un utilisateur possède le profil d’un administrateur système en tant qu’utilisateur de synchronisation, désélectionnez la case [!UICONTROL Lecture seule] du profil d’administrateur système (comme illustré ci-dessous).
* Si vous avez créé un profil personnalisé pour l’utilisateur de synchronisation, décochez la case [!UICONTROL Lecture seule] correspondant à ce profil personnalisé.

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Choisissez les mises en page qui doivent afficher le champ.

1. Cliquez sur **[!UICONTROL Enregistrer et nouveau]** pour revenir en arrière et créer chacun des deux autres champs personnalisés.

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé les trois.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>En ajoutant le champ à l’objet Contact , ils sont également ajoutés à l’objet Compte de personne .

FACULTATIF : utilisez la procédure ci-dessus pour tout champ personnalisé supplémentaire du tableau ci-dessous.

<table>
 <tbody>
  <tr>
   <th>Intitulé de champ
   <th>Nom du champ
   <th>Type de données
   <th>Attributs de champ
  </tr>
  <tr>
   <td>Ville déduite</td>
   <td>mkto71_Inferred_City</td>
   <td>Texte</td>
   <td>Longueur 255</td>
  </tr>
  <tr>
   <td>Société déduite</td>
   <td>mkto71_Inferred_Company</td>
   <td>Texte</td>
   <td>Longueur 255</td>
  </tr>
  <tr>
   <td>Pays déduit</td>
   <td>mkto71_Inferred_Country</td>
   <td>Texte</td>
   <td>Longueur 255</td>
  </tr>
  <tr>
   <td>Aire métropolitaine déduite</td>
   <td>mkto71_Inferred_Metropolitan_Area</td>
   <td>Texte</td>
   <td>Longueur 255</td>
  </tr>
  <tr>
   <td>Indicatif téléphonique local déduit</td>
   <td>mkto71_Inferred_Phone_Area_Code</td>
   <td>Texte</td>
   <td>Longueur 255</td>
  </tr>
  <tr>
   <td>Code postal déduit</td>
   <td>mkto71_Inferred_Postal_Code</td>
   <td>Texte</td>
   <td>Longueur 255</td>
  </tr>
  <tr>
   <td>Région déduite</td>
   <td>mkto71_Inferred_State_Region</td>
   <td>Texte</td>
   <td>Longueur 255</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Les valeurs des champs automatiquement assignés par Marketo ne seront pas immédiatement disponibles dans [!DNL Veeva] CRM lors de la création du champ. Marketo synchronise les données avec [!DNL Veeva] CRM lors de la prochaine mise à jour de l’enregistrement sur l’un des systèmes (c’est-à-dire une mise à jour de l’un des champs synchronisés entre Marketo et [!DNL Veeva] CRM).
