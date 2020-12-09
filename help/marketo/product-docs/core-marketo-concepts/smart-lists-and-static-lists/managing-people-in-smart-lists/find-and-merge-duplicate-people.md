---
unique-page-id: 557339
description: Rechercher et fusionner des personnes Duplicata - Documents marketing - Documentation sur les produits
title: Rechercher et fusionner des personnes de Duplicata
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---


# Rechercher et fusionner des personnes de Duplicata {#find-and-merge-duplicate-people}

Marketo annule automatiquement les duplicata lorsque de nouvelles personnes entrent dans le système. Cependant, votre service de gestion de la relation client a peut-être initialement envoyé des duplicata à Marketing Cloud. Voici comment les fusionner.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Marketo ne dédupliquera pas automatiquement une synchronisation Salesforce ou Microsoft Dynamics, ni lorsque vous saisirez manuellement des personnes.

>[!PREREQUISITES]
>
>La recherche et la fusion de duplicata impliqueront l&#39;utilisation de listes [intelligentes](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md)intégrées/système.

## Rechercher des Duplicata {#find-duplicates}

1. Accédez à la zone **Base de données** .

   ![](assets/db.png)

   >[!CAUTION]
   >
   >La fusion de personnes dans Marketo peut ne pas fonctionner si vous utilisez un compte de personne Salesforce. Si possible, fusionnez les enregistrements dans Salesforce.

1. Sélectionnez la liste intelligente **Possible** **Duplicata** du système et cliquez sur l’onglet **Personnes** .

   ![](assets/two.png)

   >[!NOTE]
   >
   >Vous pouvez également [rechercher des personnes Duplicata avec une logique](find-duplicate-people-with-custom-logic.md)personnalisée.

## Fusionner les personnes manuellement {#merge-people-manually}

>[!CAUTION]
>
>Lors de la fusion de personnes, si la personne perdante a un objet personnalisé Marketo, il **ne sera pas** réassocié à la personne gagnante. Reparent l&#39;objet personnalisé avant d&#39;effectuer la fusion.

Sélectionnez les duplicata en maintenant la touche Ctrl/Cmd enfoncée et en cliquant sur, puis cliquez sur Fusionner les personnes.
![](assets/three.png)

>[!TIP]
>
>Vous pouvez avoir deux ou plusieurs duplicata pour la même personne - sélectionnez-les tous en même temps.

1. Vous verrez les valeurs entre les enregistrements qui *ne correspondent pas* . Sélectionnez la valeur à conserver pour chaque champ. Lorsque vous avez terminé, cliquez sur **Fusionner** . Si vous ne souhaitez aucune des deux valeurs, vous pouvez cocher **Personnalisé** et saisir la valeur de votre choix.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Lors de la fusion manuelle de personnes, la première personne sélectionnée sera la &quot;gagnante&quot;. Dans l&#39;onglet Personnes, si vous fusionnez des ID d&#39;enregistrement 198 et 199, et que vous cliquez d&#39;abord sur 199, 199 sera l&#39;ID d&#39;enregistrement des personnes fusionnées. Cela s&#39;applique également si plus de deux enregistrements sont fusionnés.

   >[!TIP]
   >
   >La fusion est préférable à la suppression. Vous conserverez tout l’historique (visites de page, clics sur les liens, ouvertures de courriel, remplissages de formulaires, etc.).

## Effet dans Salesforce {#effect-in-salesforce}

Si vous avez intégré Salesforce, vous trouverez quelques remarques sur l&#39;effet de Fusionner les pistes dans Salesforce.

    * Lorsque vous fusionnez uniquement des Pistes ou des Contacts, ils fusionnent selon les règles Salesforce normales.
    * Lors de la fusion des Pistes et Contacts, toutes les Pistes sont converties en Contacts avant la fusion selon les règles Salesforce normales.

Pour connaître le comportement de Salesforce lors de la fusion de pistes ou de contacts, consultez les documents Salesforce suivants :

    * [Fusionner les pistes de Duplicata](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
    * [Fusionner les contacts de Duplicata](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Fusion en masse {#bulk-merging}

Si vous avez trop de duplicata à fusionner manuellement, contactez votre responsable de succès client pour discuter de vos options.

Super ! Si vous êtes connecté à un CRM, les enregistrements y fusionnent selon les règles ci-dessous.