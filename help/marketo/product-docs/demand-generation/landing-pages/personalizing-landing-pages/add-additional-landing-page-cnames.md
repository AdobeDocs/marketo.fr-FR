---
unique-page-id: 2359798
description: Ajout de CNAME de page de destination supplémentaires - Documents Marketo - Documentation du produit
title: Ajout de CNAME de page de destination supplémentaires
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Ajout de CNAME de page de destination supplémentaires {#add-additional-landing-page-cnames}

Vous pouvez ajouter des CNAME de page de destination pour permettre à différentes URL de pointer vers vos pages de destination Marketo. Suivez les étapes ci-dessous pour gérer plusieurs domaines.

>[!CAUTION]
>
>Les cookies ne peuvent pas être partagés sur plusieurs domaines.

>[!TIP]
>
>**Même domaine de niveau supérieur - Bien ! Les cookies sont partagés**.<br/> **aller**.mycompany.com > **info**.mycompany.com
>
>**Différents domaines de niveau supérieur - Mauvais ! Les cookies ne sont _pas_ partagés**.<br/>.**mycompany**.com > aller.**mynewcompany**.com

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone **Admin**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Cliquez sur **Mon compte**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Faites défiler jusqu’à « Informations d’assistance » et copiez votre Munchkin ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Envoyer la demande au service informatique {#send-request-to-it}

1. Demandez à votre service informatique de configurer le CNAME suivant : (Remplacez le mot [CNAME] par le CNAME de votre choix et [l’ID Munchkin] par le texte de l’étape précédente).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Ajouter un nouveau CNAME {#add-a-new-cname}

1. Une fois que votre service informatique a créé le CNAME, accédez à la zone **Admin**.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Cliquez sur **Pages de destination**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Cliquez sur **[!UICONTROL Nouveau]** puis sélectionnez **[!UICONTROL Nouvel alias de domaine]**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Saisissez votre **[!UICONTROL alias de domaine].** La **[!UICONTROL Page par défaut]** s’affiche si le visiteur ne saisit pas d’URL. Dans ce cas, indiquez où ils doivent aller.

   >[!NOTE]
   >
   >Pour la [!UICONTROL Page par défaut], vous pouvez sélectionner une page de destination ou une URL externe, telle que votre site web public.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Saisissez votre **[!UICONTROL Page par défaut]** puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Joli ! Vous savez maintenant quoi faire si vous souhaitez ajouter un CNAME.
