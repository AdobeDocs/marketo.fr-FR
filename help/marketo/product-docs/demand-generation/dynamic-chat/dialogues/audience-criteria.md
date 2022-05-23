---
description: Critères d’audience - Documents Marketo - Documentation du produit
title: Critère d’audience
exl-id: 9b70b03e-229e-469e-bd65-07aaf2dcbec6
source-git-commit: 17f56a01096b1cc48a9df7a717145a00ef491dbd
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 2%

---

# Critère d’audience {#audience-criteria}

Tout comme les listes dynamiques Marketo, les attributs Critères d’audience vous permettent de définir votre audience cible. Vous pouvez cibler des personnes connues ou inconnues à l’aide d’attributs déduits, de personnes ou de société (ou d’une combinaison de ces attributs).

## Événements {#events}

![](assets/audience-criteria-0.png)

Les événements vous permettent de cibler les visiteurs en fonction de la durée de leur défilement ou de la durée pendant laquelle ils se trouvent sur votre page/site. Dans l’exemple ci-dessous, nous ciblons les visiteurs qui se trouvent sur une page spécifique depuis plus de 20 secondes.

1. Attrapez le **Durée sur la page** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-0a.png)

1. Définissez l’heure &quot;Supérieur à&quot; sur 20 secondes.

   ![](assets/audience-criteria-0b.png)

1. Ajoutez l’URL de la page souhaitée dans la [Cible](#target) .

   ![](assets/audience-criteria-0c.png)

## Attributs {#attributes}

![](assets/audience-criteria-0d.png)

**Personnes connues**

Il y a _many_ combinaisons d’attributs parmi lesquelles choisir. Dans l’exemple ci-dessous, nous ciblons tous les **personnes connues** en Californie, qui travaille dans une entreprise de plus de 50 employés.

1. Attrapez le **État de la personne** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-1.png)

1. _Is_ est défini par défaut. Dans le champ Sélectionner les valeurs , saisissez CA (vous pouvez également cliquer sur la liste déroulante et sélectionner dans la liste).

   ![](assets/audience-criteria-2.png)

1. Attrapez le **Taille de l’entreprise** Attribuez-le et faites-le glisser à l’endroit où il indique _faire glisser un attribut ici ;_.

   ![](assets/audience-criteria-3.png)

   >[!NOTE]
   >
   >Vous pouvez également choisir un attribut en cliquant sur son **+** icône .

1. Cliquez sur la liste déroulante des opérateurs et sélectionnez **Supérieur à**.

   ![](assets/audience-criteria-4.png)

1. Saisissez 50, puis cliquez ailleurs à l’écran pour enregistrer.

   ![](assets/audience-criteria-5.png)

Et voilà !

**Personnes anonymes**

Il existe un moyen simple de cibler spécifiquement les personnes qui ne se trouvent pas encore dans votre base de données. Dans cet exemple, nous ciblons tous les **anonymes** situé dans le quartier de New York.

1. Attrapez le **Adresse électronique de la personne** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-6.png)

1. Cliquez sur la liste déroulante des opérateurs et sélectionnez **Est vide**.

   ![](assets/audience-criteria-7.png)

1. Attrapez le **État déduit** Attribuez-le et faites-le glisser à l’endroit où il indique _faire glisser un attribut ici ;_.

   ![](assets/audience-criteria-8.png)

   >[!NOTE]
   >
   >Lorsqu’une personne visite votre site web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) les cookies et les place dans le système. Nous recherchons leur adresse IP dans une base de données spéciale et en déduisons toutes sortes de bonnes informations.

1. _Is_ est défini par défaut. Dans le champ Sélectionner les valeurs , saisissez NY (vous pouvez également cliquer sur la liste déroulante et effectuer une sélection dans la liste).

   ![](assets/audience-criteria-9.png)

## Ajout de groupes {#add-groups}

Vous avez également la possibilité de regrouper des attributs, au cas où vous souhaitez tous avoir certains attributs avec &quot;tous ou n’importe lequel&quot; d’un autre. Vous pouvez ajouter plusieurs groupes.

![](assets/audience-criteria-10.png)

![](assets/audience-criteria-11.png)

## Cible {#target}

C’est là que vous saisissez la ou les URL sur lesquelles vous souhaitez qu’un dialogue spécifique s’affiche. Vous avez également la possibilité d’ajouter des exclusions.

Formats acceptables :

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>L’utilisation d’un astérisque agit comme un caractère générique fourre-tout. Donc `https://*.website.com` placerait la boîte de dialogue sur chaque page du site, y compris les sous-domaines (par exemple : `support.website.com`). Et `https://website.com/folder/*` placerait la boîte de dialogue sur chaque page de HTML dans le dossier suivant (par exemple : dans ce cas, disons que le dossier est &quot;sports&quot;, donc : website.com/sports/baseball.html, website.com/sports/football.html, etc.).

**Exclusions**

Utilisez les exclusions pour vous assurer que votre dialogue fonctionne **not** s’affichent sur une page/zone spécifique de votre site. Les exclusions suivent le même format que les inclusions.

![](assets/audience-criteria-12.png)

>[!MORELIKETHIS]
>
>* [Créer un dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Concepteur de diffusion](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [Rapports](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

