---
unique-page-id: 10098812
description: Configuration de l’attribution des recettes pour les campagnes Digital Advertising - Documents Marketo - Documentation du produit
title: Configuration de l’attribution des recettes pour les campagnes Digital Advertising
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Configuration de l’attribution des recettes pour les campagnes Digital Advertising {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Voici comment configurer l’attribution des recettes pour les canaux et campagnes publicitaires numériques. Une fois que vous l’avez configuré, vous pouvez effectuer l’attribution des recettes Première touche et multipoint pour les publicités numériques de la même manière que dans d’autres programmes Marketo.

>[!IMPORTANT]
>
>Le 31 juillet 2024, nous avons commencé à abandonner cette fonctionnalité. Il n’est plus possible de créer de nouvelles ressources. Les ressources existantes continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Après avoir configuré votre premier programme publicitaire dans Marketo, vous pouvez le cloner et le mettre à jour pour d’autres canaux. Par exemple, clonez un programme LinkedIn à un programme Facebook.

Avec des programmes distincts, vous pouvez ensuite suivre le nombre de conversions de chacun et afficher vos programmes dans l’analyseur de programme, l’analyseur d’influence d’opportunité et d’autres fonctionnalités Marketo Analytics.

>[!PREREQUISITES]
>
>* Configuration d’une balise de canal avec des valeurs d’état et la réussite du programme (par exemple, Digital Advertising ou Social Payé et PPC)
>* Créer ou modifier un formulaire pour transmettre une chaîne de requête à la personne
>* Assurez-vous d’avoir accès à certaines fonctionnalités de Revenu Cycle Analytics pour créer des rapports sur vos canaux publicitaires et campagnes.

## Création d’un programme par défaut {#create-a-default-program}

Contrairement à certains programmes (tels que les courriers électroniques) qui peuvent s’exécuter périodiquement pendant une période spécifique, les programmes par défaut sont toujours activés.

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Cliquez sur **New** et sélectionnez **New Program**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Si vous avez déjà un programme en place, vous pouvez [le cloner](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Chaque fois que vous clonez un programme, veillez à remplacer les noms dans les champs de chaîne de requête des listes dynamiques.

1. Placez le nouveau programme dans un dossier de campagne spécifique, une fois le programme initial défini.

   >[!NOTE]
   >
   >**Exemple**
   >
   >Une chaîne de requête transmise par l’URL permet à Marketo de déterminer la campagne publicitaire sur laquelle un visiteur a cliqué lorsqu’il est devenu une personne dans Marketo.
   >
   >Vous pouvez créer une méthodologie de chaîne de requête qui inclut toutes les variables que vous souhaitez mesurer. Marketo utilise ces variables pour ajouter des personnes à vos différents programmes.
   >
   >Par exemple, vous pouvez utiliser Canal type_Channel__Asset__Region. Cela peut se présenter comme suit : SP_FB_NewGuide_US. **Remarque** : les abréviations économisent de l’espace.
   >
   >Vous pouvez également le configurer en tant que Channel_Adsource_AssetName_Region_UniqueIdNumber. Cela peut se présenter comme suit : Social-Paid_Facebook_NewGuide_NA_123.

## Création d’une campagne dynamique pour les nouveaux noms {#create-a-smart-campaign-for-new-names}

1. Dans la campagne dynamique, créez une liste dynamique qui contient deux déclencheurs et deux filtres, comme indiqué.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >La chaîne de requête utilisée dans les deux déclencheurs et le filtre **Program That Captured Name** est votre propre nom. Les chaînes de requête affichées ici sont par exemple uniquement. Si vous avez cloné le champ, remplacez simplement ces champs.

1. Créez une étape de flux pour modifier l’attribut en **Programme d’acquisition** et définissez la Nouvelle valeur sur la valeur que vous avez définie pour les campagnes sociales payantes.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Planifiez et activez la campagne.

## Création d’une campagne dynamique pour un état/un programme réussi {#create-a-smart-campaign-for-status-program-success}

Vous avez besoin d’une seconde campagne intelligente pour modifier l’état des personnes, de sorte qu’elles puissent réaliser le succès du programme et être incluses dans les calculs d’attribution des recettes.

1. Dans le déclencheur **Remplit le formulaire**, saisissez le nom du programme dans la chaîne de requête. Si vous clonez le programme, remplacez simplement l’ancien nom de chaîne de requête par le nouveau.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Créez des étapes de flux pour définir l’état associé à la réussite du programme.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >L’exemple ci-dessus montre **Converted**, mais cela dépend de votre état/valeur de succès.

1. Planifiez et activez la campagne.

## Créer votre publicité {#create-your-ad}

Après avoir configuré le programme et les campagnes, créez la nouvelle publicité.

1. Accédez au canal, par exemple LinkedIn ou Facebook.
1. Créez une publicité.
1. Sélectionnez une landing page Marketo comme destination de l’appel à l’action dans la campagne.
1. Ajoutez la chaîne de requête à l’URL.

   >[!NOTE]
   >
   >**Exemple**
   >
   >Voici comment ajouter toutes les informations que vous configurez dans une URL réelle. Les éléments sont séparés par une esperluette (&amp;) :
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** est la Source de personne utilisée comme identifiant de canal
   >* **comment** est l’identifiant unique créé pour chaque programme
   >* **camp** correspond à la campagne dans Facebook, LinkedIn ou Google
   >* **kk** est le mot-clé ou le nom de ressource que vous souhaitez capturer
   >
   >**Ces quatre termes doivent être en minuscules et il ne peut y avoir aucun espace dans l’URL pour que ces informations soient capturées.**

## Meilleures pratiques {#best-practices}

Utilisez une balise de canal unique pour représenter l’ensemble de Digital Advertising ou plusieurs balises de canal si vous souhaitez des comparaisons plus granulaires par rapport à vos autres canaux marketing (par exemple, Social-Payé, Recherche-Payée, Affichage, Reciblage).

Ensuite, configurez différents programmes pour chaque vue de rapport dont vous avez besoin. Utilisez un ID commun comme paramètre dans l’URL (BC, par exemple) dans la chaîne de requête si 10 régions lancent ensemble une &quot;Big Campaign&quot; et que vous souhaitez pouvoir afficher les résultats entre les régions.

Si vous souhaitez rendre compte de chaque région et des résultats collectifs de la Big Campaign, créez 11 programmes : un pour chaque région et un pour la Big Campaign. Chaque programme ne référence que les caractères appropriés de la chaîne de requête (comme BC).

Il y a un chevauchement intentionnel entre le nombre de personnes dans la Big Campaign et les programmes de la région, donc vous ne voudriez pas rapporter le nombre total de personnes dans les 11 programmes, comme certaines personnes sont à la fois dans la Big Campaign et dans l&#39;un des programmes de la région.
