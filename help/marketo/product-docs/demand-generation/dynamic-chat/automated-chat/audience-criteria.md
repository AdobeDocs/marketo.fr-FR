---
description: Découvrez les Critères d’audience pour le ciblage des personnes qui voient vos boîtes de dialogue Dynamic Chat. Définissez des audiences à l’aide d’événements, des attributs de personne et d’entreprise et de la priorité.
title: Critère d’audience
feature: Dynamic Chat
exl-id: 95c4558e-0c0c-4623-bb7d-b6ac2f455c01
TQID: https://experienceleague.adobe.com/1h0-iXYpK53V4jUIZVM-T3TJkxhbaWvmZrb4er1vW18
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240e
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 624
ht-degree: 1%

---

# Critère d’audience {#audience-criteria}

Tout comme les listes dynamiques Marketo Engage, les attributs des critères d’audience vous permettent de définir votre audience cible. Vous pouvez cibler des personnes connues ou inconnues à l’aide d’attributs déduits, de personne ou d’entreprise (ou d’une combinaison de ces attributs).

## Priorité {#priority}

La priorité détermine la boîte de dialogue qu’un prospect reçoit s’il répond aux critères de plusieurs d’entre elles. Il est établi lorsque vous [créez votre boîte de dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"} pour la première fois. Vous pouvez modifier la priorité d’une boîte de dialogue existante en l’ouvrant et en accédant à **[!UICONTROL Détails de la boîte de dialogue]** dans l’onglet Critères d’audience.

![](assets/audience-criteria-1.png)

## Événements {#events}

Les événements vous permettent de cibler les visiteurs et visiteuses en fonction de leur niveau de défilement ou de la durée pendant laquelle ils se trouvent sur votre page ou site. Dans l’exemple ci-dessous, la configuration cible les visiteurs et visiteuses qui se trouvent sur une page spécifique depuis plus de 20 secondes.

1. Saisissez l’événement **[!UICONTROL Temps passé sur la page]** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-3.png)

1. Définissez l’heure « [!UICONTROL  supérieure à ] » sur 20 secondes.

   ![](assets/audience-criteria-4.png)

1. Ajoutez l’URL de la page souhaitée dans la section [[!UICONTROL Target]](#target).

   ![](assets/audience-criteria-5.png)

## Attributs {#attributes}

**Personnes connues**

Vous pouvez choisir parmi de _nombreuses_ combinaisons d’attributs. Dans l’exemple ci-dessous, la configuration cible toutes les personnes connues en Californie qui travaillent dans une entreprise de plus de 50 employés.

1. Saisissez l’attribut **[!UICONTROL État de la personne]** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-7.png)

1. _[!UICONTROL Est]_ est défini par défaut. Dans le champ Sélectionner des valeurs , saisissez dans l’autorité de certification (vous pouvez également cliquer sur la liste déroulante et effectuer une sélection dans la liste).

   ![](assets/audience-criteria-8.png)

1. Saisissez l’attribut **[!UICONTROL Taille de l’entreprise]** et faites-le glisser à l’emplacement indiqué _faites glisser un attribut ici_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >Vous pouvez également choisir un attribut en cliquant sur son icône **+**.

1. Cliquez sur la liste déroulante des opérateurs et sélectionnez **[!UICONTROL Supérieur à]**.

   ![](assets/audience-criteria-10.png)

1. Tapez 50 et cliquez ailleurs sur l&#39;écran pour enregistrer.

   ![](assets/audience-criteria-11.png)

**Personnes anonymes**

Le code suivant cible les personnes qui ne figurent pas encore dans votre base de données. Dans cet exemple, la configuration cible toutes les personnes anonymes situées dans la région de New York.

1. Saisissez l’attribut **[!UICONTROL E-mail de la personne]** et faites-le glisser vers la droite.

   ![](assets/audience-criteria-12.png)

1. Cliquez sur la liste déroulante des opérateurs et sélectionnez **[!UICONTROL Est vide]**.

   ![](assets/audience-criteria-13.png)

1. Saisissez l’attribut **[!UICONTROL État déduit]** et faites-le glisser à l’emplacement indiqué _faites glisser un attribut ici_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >Lorsqu&#39;une personne visite votre site web, [](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} crée un cookie et le place dans le système. L’adresse IP est recherchée dans une base de données spéciale pour déduire l’emplacement et d’autres informations.

1. _[!UICONTROL Est]_ est défini par défaut. Dans le champ Sélectionner des valeurs , saisissez NY (vous pouvez également cliquer sur la liste déroulante et effectuer une sélection dans la liste).

   ![](assets/audience-criteria-15.png)

## Adhésion {#membership}

Utilisez les listes dynamiques Marketo Engage pour l’audience cible de votre boîte de dialogue.

>[!AVAILABILITY]
>
>Le membre de la liste dynamique ou le membre des critères de liste nécessite Dynamic Chat Prime. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

1. Sous Abonnement, accédez à **[!UICONTROL Membre de la liste dynamique]** et déposez-la sur la zone de travail.

   ![](assets/audience-criteria-15a.png)

1. Sélectionnez la liste dynamique de votre choix.

   ![](assets/audience-criteria-15b.png)

## Ajouter des groupes {#add-groups}

Vous avez également la possibilité de regrouper les attributs si vous souhaitez que certains attributs soient associés à « tout ou partie » d’un autre. Vous pouvez ajouter plusieurs groupes.

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Cible {#target}

C’est là que vous saisissez la ou les URL pour lesquelles vous souhaitez afficher une boîte de dialogue spécifique. Vous pouvez également ajouter des exclusions.

Formats acceptables :

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>* L’utilisation d’un astérisque agit comme un caractère générique fourre-tout. Ainsi, `https://*.website.com` placez la boîte de dialogue sur chaque page du site, y compris les sous-domaines (par exemple : `support.website.com`). De plus, `https://website.com/folder/*` placerait la boîte de dialogue sur chaque page HTML dans le dossier suivant (par exemple, dans ce cas, disons que le dossier est « sports », donc : website.com/sports/baseball.html, website.com/sports/football.html, etc.).
>
>* Les paramètres d’URL ne sont pas pris en charge pour le moment.

**Exclusions**

Utilisez des exclusions pour vous assurer que votre boîte de dialogue n’apparaît _pas_ sur une page ou une zone spécifique de votre site. Les exclusions suivent le même format que les inclusions.

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [Créer une boîte de dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [Stream Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}
