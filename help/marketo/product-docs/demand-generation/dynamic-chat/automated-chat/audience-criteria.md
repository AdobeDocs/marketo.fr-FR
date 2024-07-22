---
description: Critères d’audience - Documents Marketo - Documentation du produit
title: Critère d’audience
feature: Dynamic Chat
exl-id: 95c4558e-0c0c-4623-bb7d-b6ac2f455c01
source-git-commit: f5f93a993d5b13c1fda0b31172393eff0bc65fd4
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# Critère d’audience {#audience-criteria}

Tout comme les listes dynamiques de Marketo Engage, les attributs de critères d’audience vous permettent de définir votre audience cible. Vous pouvez cibler des personnes connues ou inconnues à l’aide d’attributs déduits, de personnes ou de société (ou d’une combinaison de ces attributs).

## Priorité {#priority}

La priorité détermine le dialogue qu’un prospect reçoit lorsqu’il remplit les conditions requises pour plus d’un. Elle est établie lorsque vous [créez votre dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"} pour la première fois. Vous pouvez modifier la priorité d’un dialogue existant en l’ouvrant et en accédant à **[!UICONTROL Détails du dialogue]** dans l’onglet Critères d’audience.

![](assets/audience-criteria-1.png)

## Événements {#events}

Les événements vous permettent de cibler les visiteurs en fonction de la durée de leur défilement ou de la durée pendant laquelle ils se trouvent sur votre page/site. Dans l’exemple ci-dessous, nous ciblons les visiteurs qui se trouvent sur une page spécifique depuis plus de 20 secondes.

1. Prenez l’événement **[!UICONTROL Time on Page]** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-3.png)

1. Définissez l’heure &quot;Supérieur à&quot; sur 20 secondes.

   ![](assets/audience-criteria-4.png)

1. Ajoutez l’URL de la page souhaitée dans la section [Target](#target) .

   ![](assets/audience-criteria-5.png)

## Attributs {#attributes}

**Personnes connues**

Il existe plusieurs combinaisons d’attributs _many_ parmi lesquelles choisir. Dans l’exemple ci-dessous, nous ciblons toutes les personnes connues en Californie qui travaillent dans une entreprise de plus de 50 employés.

1. Saisissez l’attribut **[!UICONTROL Person State]** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-7.png)

1. _Is_ est défini par défaut. Dans le champ Sélectionner des valeurs , saisissez CA (vous pouvez également cliquer sur la liste déroulante et sélectionner dans la liste).

   ![](assets/audience-criteria-8.png)

1. Saisissez l’attribut **[!UICONTROL Taille de la société]** et faites-le glisser jusqu’à l’endroit où il est indiqué _Faites glisser un attribut ici_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >Vous pouvez également choisir un attribut en cliquant sur son icône **+** .

1. Cliquez sur la liste déroulante des opérateurs et sélectionnez **[!UICONTROL Supérieur à]**.

   ![](assets/audience-criteria-10.png)

1. Saisissez 50, puis cliquez ailleurs à l’écran pour enregistrer.

   ![](assets/audience-criteria-11.png)

Et c&#39;est tout !

**Personnes anonymes**

Il existe un moyen simple de cibler spécifiquement les personnes qui ne se trouvent pas encore dans votre base de données. Dans cet exemple, nous ciblons toutes les personnes anonymes situées dans la région de New York.

1. Saisissez l’attribut **[!UICONTROL Person Email]** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-12.png)

1. Cliquez sur la liste déroulante des opérateurs et sélectionnez **[!UICONTROL Est vide]**.

   ![](assets/audience-criteria-13.png)

1. Saisissez l’attribut **[!UICONTROL État déduit]** et faites-le glisser jusqu’à l’endroit où il est indiqué _faites glisser un attribut ici_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >Lorsqu’un visiteur se rend sur votre site Web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} les cookies et les met dans le système. Nous recherchons leur adresse IP dans une base de données spéciale et en déduisons toutes sortes de bonnes informations.

1. _Is_ est défini par défaut. Dans le champ Sélectionner les valeurs , saisissez NY (vous pouvez également cliquer sur la liste déroulante et effectuer une sélection dans la liste).

   ![](assets/audience-criteria-15.png)

## Adhésion {#membership}

Utilisez des listes dynamiques Marketo Engage pour l’audience cible de votre dialogue.

>[!AVAILABILITY]
>
>Un membre de la liste dynamique ou un membre de la liste nécessite Dynamic Chat. Pour plus d’informations, contactez l’équipe de compte d’Adobe (votre gestionnaire de compte).

1. Sous Adhésion, accédez à **[!UICONTROL Membre de la liste dynamique]** et déposez-le sur la zone de travail.

   ![](assets/audience-criteria-15a.png)

1. Sélectionnez la liste dynamique de votre choix.

   ![](assets/audience-criteria-15b.png)

## Ajout de groupes {#add-groups}

Vous avez également la possibilité de regrouper des attributs, au cas où vous souhaitez tous avoir certains attributs avec &quot;tous ou n’importe lequel&quot; d’un autre. Vous pouvez ajouter plusieurs groupes.

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Target {#target}

C’est là que vous saisissez la ou les URL sur lesquelles vous souhaitez afficher un dialogue spécifique. Vous avez également la possibilité d’ajouter des exclusions.

Formats acceptables :

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>L’utilisation d’un astérisque agit comme un caractère générique fourre-tout. Par conséquent, `https://*.website.com` placerait la boîte de dialogue sur chaque page du site, y compris les sous-domaines (ex : `support.website.com`). Et `https://website.com/folder/*` placerait la boîte de dialogue sur chaque page d’HTML dans le dossier suivant (par exemple, supposons que le dossier soit &quot;sports&quot;, donc : website.com/sports/baseball.html, website.com/sports/football.html, etc.).

**Exclusions**

Utilisez les exclusions pour vous assurer que votre dialogue n’apparaît _pas_ sur une page/zone spécifique de votre site. Les exclusions suivent le même format que les inclusions.

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [Créer un dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [Stream Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}
