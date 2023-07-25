---
unique-page-id: 2360189
description: Personnalisation des URL de votre page d’entrée avec un CNAME (Administration) - Documents Marketo - Documentation du produit
title: Personnalisation des URL de votre page d’entrée avec un CNAME (Administration)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 6%

---

# Personnalisation des URL de votre page d’entrée avec un CNAME  {#customize-your-landing-page-urls-with-a-cname}

Même si Marketo héberge vos landing pages, l’URL doit être personnalisée pour votre entreprise.

>[!NOTE]
>
>No CNAME :
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

   C&#39;est la partie avant de l&#39;URL. Exemples:

   * **go**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **pages**.YourCompany.com/NameOfPage.html

   Le seul mot (plus YourCompany.com) est appelé CNAME. Vous en aurez besoin plus tard alors prenez note.

1. Recherchez votre chaîne de compte.

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Cliquez sur **[!UICONTROL Pages de destination]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. Sous , **[!UICONTROL Pages d’entrée]** copiez la chaîne de compte dans la section Paramètres .

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. Vous en aurez également besoin plus tard, alors prenez note.

1. Envoyez une demande au service informatique.

1. Demandez à votre personnel informatique de configurer le CNAME suivant (remplacez le mot [CNAME] et [CHAÎNE DE COMPTE] avec le texte de l’étape précédente) :

   [CNAME].YourCompany.com > [CHAÎNE DE COMPTE].mktoweb.com

1. Terminez la configuration CNAME.

1. Une fois que votre service informatique a créé le CNAME, revenez à la **[!UICONTROL Administration]** zone.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Cliquez sur **[!UICONTROL Pages de destination]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Sous , **[!UICONTROL Paramètres]** , cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Saisissez votre CNAME dans **[!UICONTROL Nom de domaine pour les pages d’entrée]**, saisissez votre **[!UICONTROL Page de secours]**, saisissez votre **[!UICONTROL Page d’accueil]**, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

Votre page de secours est l’endroit où les visiteurs seront redirigés si votre page d’entrée Marketo n’est pas disponible.

Beau boulot ! Vos landing pages sont maintenant marquées avec le domaine de votre entreprise.
