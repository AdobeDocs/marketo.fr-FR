---
description: Exécuter Campaign - Documents Marketo - Documentation du produit
title: Lancer la campagne
translation-type: tm+mt
source-git-commit: 20a3bee9973340d7b772532d1be31fe745e5ffd7
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---

# Lancer la campagne {#execute-campaign}

Un Campaign exécutable, comme d&#39;autres campagnes, contient une Liste intelligente, un flux et une planification. Contrairement à d’autres campagnes, vous ne planifiez pas ou n’activez pas ce type de campagne. Elle ne peut être appelée que par une autre campagne via l’étape de flux Exécuter Campaign. Les étapes de flux dans le Campaign exécutable sont exécutées en série avec la campagne parent (contrairement à Request Campaign, qui s’exécute en parallèle dans un Campaign Trigger distinct).

>[!NOTE]
>
>Les campagnes exécutables sont toujours des enfants de la campagne (parent) qui les appelle.

## Quand utiliser Exécuter Campaign {#when-to-use-execute-campaign}

Il y a beaucoup de choses que vous pouvez faire avec une Campaign Exécutable. Elles sont conçues pour faciliter les tâches opérationnelles communes, telles que le routage de piste, la gestion du cycle de vie et la notation (entre autres), et peuvent être utilisées pour exécuter le même flux de travail depuis les campagnes par lot ou déclenchées.

Vous pouvez également les utiliser lorsque vous devez exécuter un flux distinct, mais vous devez dépendre des résultats de ce flux dans les choix d’étapes de flux suivants (c.-à-d., si cela est le cas, faites-le).

Exécuter Campaign est une amélioration sur [Request Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md), car il peut s&#39;exécuter en série ou en parallèle, alors que ce dernier s&#39;exécute uniquement en parallèle.

>[!NOTE]
>
>Les étapes d’attente et les crochets Web ne seront jamais compatibles avec les campagnes exécutables. Pour ceux-ci, vous devrez utiliser Request Campaign à la place.

## Création d&#39;une Campaign exécutable {#how-to-create-an-executable-campaign}

1. Cliquez avec le bouton droit de la souris sur votre programme et sélectionnez **Nouvelle Campaign intelligente**.

   ![](assets/execute-campaign-1.png)

1. Attribuez-lui un nom, cochez la case **Exécutable**, puis cliquez sur **Créer**.

   ![](assets/execute-campaign-2.png)

1. Définissez la Liste et le flux dynamiques, comme tout autre Campaign dynamique.

Vous pouvez également cloner une Campaign dynamique existante. Si vous clonez un Campaign exécutable existant, vous devrez toujours cocher la case **Executable** après l&#39;avoir nommé.

>[!NOTE]
>
>Vous ne pouvez pas cloner une campagne qui contient des déclencheurs.

## Utiliser le contexte du jeton Campaign parent {#use-parent-campaign-token-context}

Lorsqu’elle est définie sur true, les contextes de jeton suivants sont envoyés dans la campagne enfant (celle en cours d’exécution) :

* Mes jetons
* Jetons Campaign
* Jetons de programme
* Jetons de membre
* [Jetons](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)  de déclenchement (s’ils sont appelés à partir d’une Campaign déclenchée)

**Interaction API**

Lors de l’utilisation de l’option Planifier ou Demander Campaign [dans l’API](https://developers.marketo.com/rest-api/assets/smart-campaigns/#batch), les deux options vous permettent de transmettre des valeurs pour Mes jetons, ce qui remplace les valeurs définies pour ces jetons dans la campagne que vous appelez. Si ce Campaign exécute ensuite une autre campagne et définit &quot;Utiliser le contexte parent avec la valeur True&quot;, il utilisera les valeurs transmises par le biais de l’API, plutôt que celles définies dans l’application.

## Éléments à noter {#things-to-note}

* La Liste intelligente filtrera tous ceux qui ne sont pas admissibles. Si une personne est admissible, l&#39;enregistrement d&#39;activité Campaign exécuté qui en résulte les liste comme &quot;Qualifié : TRUE&quot; (et FALSE dans le cas contraire)
* Les règles de qualification Planifier Campaign s’appliquent (Paramètres de Campaign intelligent sous l’onglet Planifier).
* Les campagnes exécutables ne peuvent pas être appelées dans les espaces de travail.
* Si vous utilisez l&#39;action de flux [Supprimer du flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) ciblant une Campaign exécutable, elle cible à la fois l&#39;enfant et le parent.
* Profiter de l’héritage des jetons - Par exemple, si vous avez un seul flux de score commun déclenché par plusieurs ressources différentes, vous pouvez définir un score par défaut Mon jeton dans la campagne enfant et dans la campagne parente afin de remplacer la valeur de campagne de score enfant pour vos campagnes parentes (voir l’exemple visuel ci-dessous).
* L&#39;imbrication de campagnes exécutables n&#39;est pas disponible pour l&#39;instant, mais sera dans une prochaine version

>[!CAUTION]
>
>Ne laissez jamais vos listes intelligentes pour les campagnes exécutables non valides, sinon **personne** n&#39;y aura droit. Il est recommandé de créer des ressources de liste intelligentes distinctes, de les définir complètement et de s’assurer qu’elles sont valides. Ensuite, utilisez le filtre &quot;Membre de la Liste intelligente&quot; dans le Campaign exécutable pour que vous puissiez permuter votre définition de liste intelligente.

## Exemple d&#39;héritage de jeton {#token-inheritance-example}

Vous trouverez ci-dessous un exemple visuel de l&#39;héritage des jetons dans une Campaign exécutable et deux campagnes parents : l’un avec un contexte de jeton défini sur **True**, l’autre sur **False**.

Campagne enfant avec un score de changement symbolique.

![](assets/execute-campaign-3.png)

Les jetons de la campagne enfant.

![](assets/execute-campaign-4.png)

**Exemple 1 - Vrai**

À l’étape Exécuter le flux Campaign de la première campagne parent, le paramètre &quot;Utiliser le contexte du jeton Parent Campaign&quot; est défini sur **True**.

![](assets/execute-campaign-5.png)

Mes jetons de la campagne parent.

![](assets/execute-campaign-6.png)

Les résultats : note modifiée par +10.

![](assets/execute-campaign-7.png)

**Exemple 2 : False**

Dans le filtre Exécuter Campaign de la seconde campagne parent, le paramètre &quot;Utiliser le contexte du jeton Parent Campaign&quot; est défini sur **False**.

![](assets/execute-campaign-8.png)

Mes jetons de la campagne parent.

![](assets/execute-campaign-9.png)

Les résultats : score inchangé, car la valeur de score de la campagne enfant, +0, a été utilisée.

![](assets/execute-campaign-10.png)
