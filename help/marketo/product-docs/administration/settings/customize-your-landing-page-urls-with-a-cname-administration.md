---
unique-page-id: 2360189
description: Personnaliser vos URL de Landing page avec un CNAME (Administration) - Docs marketing - Documentation sur les produits
title: Personnaliser vos URL de Landing page avec un CNAME (Administration)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# Personnaliser vos URL de Landing page avec un CNAME (Administration) {#customize-your-landing-page-urls-with-a-cname-administration}

Même si Marketo héberge vos landings page, l’URL doit être personnalisée pour votre société.

>[!NOTE]
>
>Aucun CNAME :
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME de marque :
>
>https://go.**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Mettons-nous en place !

1. Sélectionnez un CNAME.

   C&#39;est la partie avant de l&#39;URL. Exemples :

   * **allez**&#x200B;à .YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **pages**.YourCompany.com/NameOfPage.html

   Le seul mot (plus YourCompany.com) est appelé CNAME. Vous en aurez besoin plus tard, alors prenez note.

1. Recherchez votre chaîne de compte.

1. Accédez à la zone **Admin** et cliquez sur **Landings page**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. Sous l’onglet **Landings page** , copiez la chaîne de compte dans la section Paramètres.

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. Vous en aurez également besoin plus tard, alors prenez note.

1. Envoyer la demande au service informatique.

1. Demandez à votre personnel informatique de configurer le CNAME suivant (remplacez le mot [CNAME] et la CHAÎNE [] DE COMPTE par le texte de l’étape précédente) :

   [CNAME].YourCompany.com > [ACCOUNT STRING].mktoweb.com

1. Effectuez la configuration CNAME.

1. Une fois que votre service informatique a créé le CNAME, accédez à **Admin** et cliquez sur **Landings page**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. Sous la section **Paramètres** , cliquez sur **Modifier**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Entrez votre CNAME dans le nom de **domaine pour les Landings page**, entrez votre page **de** secours, entrez votre **page d&#39;accueil**, puis cliquez sur **Enregistrer.**

   ![](assets/image2014-9-16-13-3a10-3a45.png)

Votre page de secours est celle où les visiteurs seront redirigés si votre landing page Marketo n’est pas disponible.

Beau boulot ! Vos landings page sont désormais marqués avec votre domaine de société.
