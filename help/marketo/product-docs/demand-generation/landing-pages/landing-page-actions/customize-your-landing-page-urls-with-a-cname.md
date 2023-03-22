---
unique-page-id: 2359746
description: Personnalisation des URL de votre page d’entrée avec un CNAME - Documents Marketo - Documentation du produit
title: Personnalisation des URL de votre page d’entrée avec un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 3%

---

# Personnalisation des URL de votre page d’entrée avec un CNAME {#customize-your-landing-page-urls-with-a-cname}

Même si Marketo héberge vos landing pages, l&#39;URL peut être entièrement personnalisée. À quoi cela ressemble sans CNAME :

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

À quoi il doit ressembler :

`https://go.YourCompany.com/UnsubscribePage.html`

## Choisir un CNAME {#choose-a-cname}

Sélectionnez un mot pour accéder au début de l’URL de vos landing pages. Ce n&#39;est qu&#39;un mot et devrait être relativement court. Exemples:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

Le seul mot (plus YourCompany.com) est appelé CNAME. Vous en aurez besoin plus tard alors prenez note.

## Trouvez votre Munchkin ID {#find-your-munchkin-id}

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Cliquez sur **Mon compte**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Autorisations d’administrateur requises**

1. Faites défiler l’écran jusqu’à &quot;Informations sur l’assistance&quot; et copiez votre Munchkin ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Envoyer la demande au service informatique {#send-request-to-it}

Demandez à votre personnel informatique de configurer le CNAME suivant : (Remplacer le mot [CNAME] et [Munchkin ID] avec le texte de l’étape précédente.)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Configuration CNAME terminée {#complete-cname-setup}

1. Une fois que le service informatique a créé le CNAME, accédez à la **Administration** zone.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Cliquez sur **Pages de destination**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Sous , **Paramètres** , cliquez sur **Modifier**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Saisissez votre CNAME dans **Nom de domaine pour les pages d’entrée**, saisissez votre **Page de secours**, saisissez votre **Page d’accueil** et cliquez sur **Enregistrer**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Votre page de secours sera alors redirigée vers les pistes de page si votre page d’entrée Marketo n’est pas disponible.

Beau boulot ! Vos landing pages sont maintenant marquées avec le domaine de votre entreprise.
