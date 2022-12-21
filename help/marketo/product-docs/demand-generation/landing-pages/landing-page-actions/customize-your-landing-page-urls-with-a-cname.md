---
unique-page-id: 2359746
description: Personnalisation des URL de votre page d’entrée avec un CNAME - Documents Marketo - Documentation du produit
title: Personnalisation des URL de votre page d’entrée avec un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

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

## Rechercher votre chaîne de compte {#find-your-account-string}

1. Accédez au **Administration** et cliquez sur **Pages d’entrée**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Autorisations d’administrateur requises**

1. Sous , **Landing** **Pages** , copiez la variable **Compte** **Chaîne** de la **Paramètres** .

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Vous en aurez également besoin plus tard, alors prenez-en note.

## Envoyer la demande au service informatique {#send-request-to-it}

Demandez à votre personnel informatique de configurer le CNAME suivant : (Remplacer le mot [CNAME] et [CHAÎNE DE COMPTE] avec le texte de l’étape précédente.)

[CNAME].YourCompany.com > [CHAÎNE DE COMPTE].mktoweb.com

## Configuration CNAME terminée {#complete-cname-setup}

1. Une fois que le service informatique a créé le CNAME, accédez à **Administration** et cliquez sur **Pages d’entrée**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Sous , **Paramètres** , cliquez sur **Modifier**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Saisissez votre CNAME dans **Nom de domaine pour les pages d’entrée**, saisissez votre **Page de secours**, saisissez votre **Page d’accueil** et cliquez sur **Enregistrer**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Votre page de secours sera alors redirigée vers les pistes de page si votre page d’entrée Marketo n’est pas disponible.

Beau boulot ! Vos landing pages sont maintenant marquées avec le domaine de votre entreprise.
