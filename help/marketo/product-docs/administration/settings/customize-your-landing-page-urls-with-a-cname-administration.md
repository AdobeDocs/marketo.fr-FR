---
unique-page-id: 2360189
description: Personnaliser vos URL de Landing page avec un CNAME (Administration) - Docs Marketo - Documentation du produit
title: Personnaliser vos URL de Landing page avec un CNAME (Administration)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 2%

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

Procédons à la configuration!

1. Sélectionnez un CNAME.

   C&#39;est la partie avant de l&#39;URL. Exemples :

   * **allez** à .YourCompany.com/NameOfPage.html
   * **info** .YourCompany.com/NameOfPage.html
   * **pages** .YourCompany.com/NameOfPage.html

   Le seul mot (plus YourCompany.com) est appelé CNAME. Vous en aurez besoin plus tard, alors prenez note.

1. Recherchez votre chaîne de compte.

1. Accédez à la zone **Admin** et cliquez sur **Landings page**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. Sous l&#39;onglet **Landings page**, copiez la chaîne de compte dans la section Paramètres.

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. Vous en aurez également besoin plus tard, alors prenez note.

1. Envoyer la demande au service informatique.

1. Demandez à votre personnel informatique de configurer le CNAME suivant (remplacez le mot [CNAME] et [CHAÎNE DE COMPTE] par le texte de l’étape précédente) :

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

1. Effectuez la configuration CNAME.

1. Une fois que votre service informatique a créé le CNAME, accédez à **Admin** et cliquez sur **Landings page**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. Sous la section **Paramètres**, cliquez sur **Modifier**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Entrez votre CNAME dans **nom de domaine pour les Landings page**, entrez votre **page de secours**, entrez votre **page d&#39;accueil**, puis cliquez sur **Enregistrer**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

Votre page de secours est celle où les utilisateurs seront redirigés si votre landing page Marketo n’est pas disponible.

Beau boulot ! Vos landings page sont désormais marqués avec votre domaine de société.
