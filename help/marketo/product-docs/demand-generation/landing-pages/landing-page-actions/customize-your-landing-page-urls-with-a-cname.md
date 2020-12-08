---
unique-page-id: 2359746
description: Personnaliser vos URL de Landing page avec un CNAME - Docs marketing - Documentation du produit
title: Personnaliser vos URL de Landing page avec un CNAME
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Personnaliser vos URL de Landing page avec un CNAME {#customize-your-landing-page-urls-with-a-cname}

Même si Marketo héberge vos landings page, l’URL peut être totalement personnalisée. A quoi ressemble un CNAME :
`<pre data-theme="Confluence">http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html</pre>` Il devrait se présenter ainsi :
`<pre data-theme="Confluence"> http://go.YourCompany.com/UnsubscribePage.html</pre>`

## Choisir un CNAME {#choose-a-cname}

Choisissez un mot à insérer au début de l’URL de vos landings page. Ce n&#39;est qu&#39;un mot et devrait être relativement court. Exemples :

* allez-y. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* info. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* pages. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)

Le seul mot (plus [YourCompany.com](http://YourCompany.com)) est appelé CNAME. Vous en aurez besoin plus tard, alors prenez note.

## Rechercher votre chaîne de compte {#find-your-account-string}

1. Accédez à la zone **Admin** et cliquez sur **Landings page.**

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Autorisations d’administrateur requises**

1. Sous l’onglet **Pages d’entrée****, copiez la** chaîne du **compte** **depuis la section Paramètres.******

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Vous en aurez également besoin plus tard, alors prenez note.

## Envoyer la demande au service informatique {#send-request-to-it}

Demandez à votre personnel informatique de configurer le CNAME suivant : (Remplacez le mot [CNAME] et CHAÎNE [] DE COMPTE par le texte de l’étape précédente.)

[CNAME]. [YourCompany.com](http://yourcompany.com/) > [ACCOUNT STRING]. [mktoweb.com](http://mktoweb.com/)

## Configuration CNAME complète {#complete-cname-setup}

1. Une fois que votre service informatique a créé le CNAME, accédez à **Admin** et cliquez sur **Pages d’entrée** ****.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Sous la section **Paramètres** , cliquez sur **Modifier**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Entrez votre CNAME dans le **nom** de **domaine** **pour** **Landing Pages, entrez votre  de , entrez votre  de page d&#39;accueil et cliquez sur Enregistrer.**********************

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Votre page de secours sera la page vers laquelle les pistes seront redirigées si votre Landing page Marketo n&#39;est pas disponible.

Beau boulot ! Vos landings page sont désormais marqués avec votre domaine de société.