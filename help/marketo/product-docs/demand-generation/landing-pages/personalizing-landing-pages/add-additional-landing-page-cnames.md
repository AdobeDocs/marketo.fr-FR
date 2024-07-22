---
unique-page-id: 2359798
description: Ajout de CNAME de page d’entrée supplémentaires - Documents Marketo - Documentation du produit
title: Ajout de CNAME de page d’entrée supplémentaires
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Ajout de CNAME de page d’entrée supplémentaires {#add-additional-landing-page-cnames}

Vous pouvez ajouter des CNAME de landing page pour permettre à différentes URL de pointer vers vos landing pages Marketo. Suivez les étapes ci-dessous pour gérer plusieurs domaines.

>[!CAUTION]
>
>Les cookies ne peuvent pas être partagés entre les domaines.

>[!TIP]
>
>**Même domaine de niveau supérieur - Bon ! Les cookies sont partagés**.<br/> **go**.mycompany.com > **info**.mycompany.com
>
>**Domaines de niveau supérieur différents - Mauvais ! Les cookies sont _not_ shared**.<br/> go.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone **Admin**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Cliquez sur **Mon compte**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Faites défiler l’écran jusqu’à &quot;Informations sur l’assistance&quot; et copiez votre Munchkin ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Envoyer la demande au service informatique {#send-request-to-it}

1. Demandez à votre service informatique de configurer le CNAME suivant : (remplacez le mot [CNAME] par le CNAME de votre choix et [Munchkin ID] par le texte de l’étape précédente).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Ajout d’un nouveau CNAME {#add-a-new-cname}

1. Une fois que votre service informatique a créé le CNAME, accédez à la zone **Admin** .

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Cliquez sur **Landing Pages**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Cliquez sur **New** , puis sélectionnez **New Domain Alias**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Saisissez votre **Alias de domaine.** La **page par défaut** s’affiche si le visiteur ne place pas d’URL. Entrez où ils doivent aller dans ce cas.

   >[!NOTE]
   >
   >Pour la page par défaut, vous pouvez sélectionner une landing page ou une URL externe, telle que votre site web public.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Saisissez votre **page par défaut** et cliquez sur **Créer**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Beau ! Vous savez maintenant quoi faire si vous souhaitez ajouter un CNAME.
