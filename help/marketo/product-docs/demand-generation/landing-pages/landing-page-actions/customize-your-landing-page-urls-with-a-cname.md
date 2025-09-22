---
unique-page-id: 2359746
description: Personnaliser vos URL de page de destination avec un CNAME - Documents Marketo - Documentation du produit
title: Personnaliser vos URL de page de destination avec un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 7%

---

# Personnaliser vos URL de page de destination avec un CNAME {#customize-your-landing-page-urls-with-a-cname}

Même si Marketo héberge vos pages de destination, l’URL peut être entièrement personnalisée. À quoi cela ressemble sans CNAME :

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

L’apparence souhaitée :

`https://go.YourCompany.com/UnsubscribePage.html`

## Choisir un CNAME {#choose-a-cname}

Choisissez un mot à placer au début de l’URL de vos pages de destination. Ce n&#39;est qu&#39;un mot et il devrait être relativement court. Exemples :

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

Le seul mot (plus YourCompany.com) est appelé CNAME. Vous en aurez besoin plus tard, prenez-en note.

## Recherche de votre Munchkin ID {#find-your-munchkin-id}

1. Accédez à la zone **Admin**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Cliquez sur **Mon compte**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Autorisations d’administrateur requises**

1. Faites défiler jusqu’à « Informations d’assistance » et copiez votre Munchkin ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Envoyer la demande au service informatique {#send-request-to-it}

Demandez à votre personnel informatique de configurer le CNAME suivant : (Remplacez le mot [CNAME] et [Munchkin ID] par le texte de l’étape précédente.)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Terminer la configuration CNAME {#complete-cname-setup}

1. Une fois que votre service informatique a créé le CNAME, accédez à la zone **Admin**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Cliquez sur **Pages de destination**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Dans la section **Paramètres**, cliquez sur **Modifier**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Saisissez votre CNAME dans **[!UICONTROL Nom de domaine pour les pages de destination]**, saisissez votre **[!UICONTROL page de secours]**, saisissez votre **[!UICONTROL page d’accueil]** et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Votre page de secours sera la page vers laquelle les prospects seront redirigés si votre page de destination Marketo n’est pas disponible.

Joli travail ! Vos pages de destination sont désormais marquées avec le domaine de votre société.
