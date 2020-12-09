---
unique-page-id: 10098812
description: Configurer l'attribution des recettes pour les campagnes de publicité numérique - Documents marketing - Documentation du produit
title: Configurer l’attribution des recettes pour les campagnes de publicité numérique
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---


# Configurer l’attribution des recettes pour les campagnes de publicité numérique {#set-up-revenue-attribution-for-digital-advertising-campaigns}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Voici comment configurer l’attribution des recettes pour les canaux et campagnes de publicité numérique. Après l’avoir configuré, vous pouvez attribuer des recettes Première touche et Multipoint aux annonces numériques de la même manière que dans les autres programmes du marché.

Après avoir configuré votre premier programme publicitaire dans Marketo, vous pouvez le cloner et le mettre à jour pour d’autres canaux. Par exemple, cloner un programme LinkedIn sur un  Facebook.

Avec des programmes distincts, vous pouvez ensuite effectuer le suivi du nombre de conversions à partir de chacun d’eux et afficher vos programmes dans l’analyseur de Programme, l’analyseur d’influence d’opportunité et d’autres fonctionnalités d’analyse de marché.

>[!PREREQUISITES]
>
>* Configuration d’une balise de canal avec des valeurs d’état et un programme réussi (Digital Advertising ou Social Paid et PPC, par exemple)
>* Créer ou modifier un formulaire pour transmettre une chaîne de requête à la personne
>* Assurez-vous d’avoir accès à certaines fonctionnalités d’analyse du cycle des recettes pour générer des rapports sur vos canaux publicitaires et campagnes.

>



## Créer un Programme par défaut {#create-a-default-program}

Contrairement à certains programmes (tels que le courriel) qui peuvent s’exécuter périodiquement pendant une période donnée, les programmes par défaut sont toujours activés.

1. Accédez à Activités **** marketing.

   ![](assets/login-marketing-activities-5.png)

1. Cliquez sur **Nouveau** et sélectionnez **Nouveau Programme**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Si vous avez déjà un programme en place, vous pouvez le [cloner](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Chaque fois que vous clonez un programme, veillez à remplacer les noms dans les champs de chaîne de requête des listes dynamiques.

1. Une fois le programme initial défini, placez le nouveau programme dans un dossier de campagne spécifique.

   >[!NOTE]
   >
   >**Exemple**
   >
   >
   >Une chaîne de requête transmise par l’URL permet à Marketing Cloud de savoir sur quelle campagne publicitaire un visiteur a cliqué lorsqu’il est devenu une personne dans Marketing Cloud.
   >
   >
   >Vous pouvez créer une méthodologie de chaîne de requête qui inclut toutes les variables à mesurer. Marketo utilise ces variables pour ajouter des personnes à vos différents programmes.
   >
   >
   >Par exemple, vous pouvez utiliser le Canal type_Canal__Asset__Region. Cela pourrait ressembler à ceci : SP_FB_NewGuide_US. **Remarque**: les abréviations économisent de l’espace.
   >
   >
   >Ou, configurez-le en tant que Canal_Adsource_AssetName_Region_UniqueIdNumber. Cela pourrait ressembler à ceci : Social-Paid_Facebook_NewGuide_NA_123.

## Créer une Campaign intelligente pour de nouveaux noms {#create-a-smart-campaign-for-new-names}

1. Dans la campagne intelligente, créez une liste intelligente qui contient deux déclencheurs et deux filtres, comme indiqué.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >La chaîne de requête utilisée dans les deux déclencheurs et le filtre Nom **capturé du** Programme vous est propre. Les chaînes de requête affichées ici sont par exemple uniquement. Si vous avez cloné le champ, remplacez simplement ces champs.

1. Créez une étape de flux pour modifier l’attribut en Programme **d’** acquisition et définissez la nouvelle valeur sur la valeur que vous avez définie pour les campagnes sociales payantes.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Planifiez et activez la campagne.

## Créer une Campaign intelligente pour un état/un Programme réussi {#create-a-smart-campaign-for-status-program-success}

Vous avez besoin d’une seconde campagne intelligente pour modifier l’état des personnes, afin qu’elles puissent réussir sur le Programme et être incluses dans les calculs d’attribution des recettes.

1. Dans le déclencheur **Remplit le formulaire** , saisissez le nom du programme dans la chaîne de requête. Si vous clonez le programme, remplacez simplement l’ancien nom de chaîne de requête par le nouveau.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Créez des étapes de flux pour remplacer l’état par un état associé à la réussite du programme.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >L&#39;exemple ci-dessus montre **Converted, **mais cela dépend de votre état/valeur de réussite.

1. Planifiez et activez la campagne.

## Créer votre publicité {#create-your-ad}

Après avoir configuré le programme et les campagnes, créez la nouvelle publicité.

1. Aller au canal ; Par exemple, LinkedIn ou Facebook.
1. Créez une publicité.
1. Sélectionnez un landing page Marketo comme destination de l’appel à l’action dans la campagne.
1. Ajoutez la chaîne de requête sur l’URL.

   >[!NOTE]
   >
   >**Exemple**
   >
   >
   >Voici comment ajouter toutes les informations que vous avez configurées dans une URL réelle. Les éléments sont séparés par une esperluette (&amp;) :
   >
   >
   >[www.marketo.com ?**source**=Social-Paid&amp;**comment**=Social-Paid_Facebook_NewGuide_NA&amp;**camp**=abc&amp;**kk=**xyz](http://www.marketo.com?source=Social-Paid&amp;comment=Social-Paid_Facebook_NewGUide_NA&amp;camp=abc&amp;kk+xyz)
   >
   >    
   >    
   >    * **source** est la source de la personne utilisée comme identifiant de canal
   >    * **commentaire** est l&#39;identifiant unique créé pour chaque programme
   >    * **camp** est la campagne dans Facebook, LinkedIn ou Google
   >    * **kk** est le mot-clé ou le nom de fichier à capturer

   >    
   >    
   >**Ces quatre termes doivent être en minuscules et l’URL ne peut contenir aucun espace pour que ces informations soient capturées.**

## Bonnes pratiques {#best-practices}

Utilisez une balise de canal unique pour représenter l’ensemble de Digital Advertising ou utilisez plusieurs balises de canal si vous souhaitez effectuer des comparaisons plus granulaires par rapport à vos autres canaux marketing (par exemple, Social-Payé, Search-Paid, Display, Retargeting).

Ensuite, configurez différents programmes pour chaque vue de rapports dont vous avez besoin. Utilisez un ID commun comme paramètre dans l’URL (BC, par exemple) dans la chaîne de requête si 10 régions lancent ensemble un &quot;Big Campaign&quot; et que vous souhaitez pouvoir vue des résultats entre les régions.

Si vous souhaitez rapporter sur chaque région et les résultats collectifs du Big Campaign, créez 11 programmes : un pour chaque région et un pour le Big Campaign. Chaque programme référence uniquement les caractères appropriés de la chaîne de requête (comme BC).

Il y a un chevauchement intentionnel dans le nombre de personnes entre le Big Campaign et les programmes de la région, donc vous ne voudriez pas rapporter le nombre total de personnes sur les 11 programmes, comme certaines personnes sont à la fois dans le Big Campaign et un des programmes de la région.
