---
description: Exécuter Campaign - Documents Marketo - Documentation du produit
title: Lancer la campagne
exl-id: d550cf08-b295-4289-9bb0-79d81cabc245
feature: Smart Campaigns
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Lancer la campagne {#execute-campaign}

Une campagne exécutable, comme d’autres campagnes, contient une liste dynamique, un flux et une planification. Contrairement à d’autres campagnes, vous ne le planifiez pas ou ne l’activez pas. Elle ne peut être appelée que par une autre opération via l&#39;étape de flux Exécuter la campagne . Les étapes de flux dans la campagne exécutable sont exécutées en série avec la campagne parente (contrairement à la campagne de requête qui s’exécute en parallèle dans une campagne de déclenchement distincte).

>[!NOTE]
>
>Les campagnes exécutables sont toujours des enfants de la campagne (parent) qui les appelle.

## Quand utiliser Exécuter une campagne {#when-to-use-execute-campaign}

Vous pouvez réaliser de nombreuses actions avec une campagne exécutable. Ils sont conçus pour faciliter les tâches opérationnelles courantes, telles que le routage des pistes, la gestion du cycle de vie et la notation (entre autres), et peuvent être utilisés pour exécuter le même workflow à partir des campagnes par lots ou déclenchées.

Vous pouvez également les utiliser lorsque vous devez exécuter un flux distinct, mais vous devez dépendre des résultats de ce flux dans les choix d’étapes de flux suivants (c’est-à-dire, si cela est le cas).

L’option Exécuter la campagne est une amélioration de la fonction [Demander la campagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md), car elle peut s’exécuter en série, tandis que la dernière ne s’exécute qu’en parallèle.

>[!NOTE]
>
>Les étapes d’attente et les webhooks ne seront jamais compatibles avec les campagnes exécutables. Pour ce faire, vous devrez utiliser plutôt Demander la campagne .

## Création d’une campagne exécutable {#how-to-create-an-executable-campaign}

1. Cliquez avec le bouton droit de la souris sur le programme de votre choix et sélectionnez **[!UICONTROL Nouvelle campagne dynamique]**.

   ![](assets/execute-campaign-1.png)

1. Donnez-lui un nom, cochez la case **[!UICONTROL Exécutable]**, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/execute-campaign-2.png)

1. Définissez la liste dynamique et le flux, comme toute autre campagne dynamique.

Vous pouvez également cloner une campagne dynamique existante. Si vous clonez une campagne exécutable existante, vous devrez toujours cocher la case **[!UICONTROL Exécutable]** après l’avoir nommée.

>[!NOTE]
>
>Vous ne pouvez pas cloner une campagne qui contient des déclencheurs.

## Utiliser le contexte de jeton de la campagne parente {#use-parent-campaign-token-context}

Lorsque la valeur est définie sur true, les contextes de jeton suivants sont envoyés dans la campagne enfant (celle en cours d’exécution) :

* Mes jetons
* Jetons de campagne
* Jetons de programme
* Jetons de membre
* [Trigger Tokens](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) (s’il est appelé à partir d’une campagne déclenchée)

**Interaction API**

Lors de l’utilisation de Schedule ou Request Campaign [ dans l’API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/assets/smart-campaigns#batch), les deux permettent de transmettre des valeurs pour My Tokens, qui remplace les valeurs définies pour ces jetons dans la campagne que vous appelez. Si cette campagne exécute ensuite une autre campagne et définit &quot;Utiliser le contexte parent sur True&quot;, elle utilisera les valeurs transmises par le biais de l’API, plutôt que les valeurs définies dans l’application.

## Informations à noter {#things-to-note}

* La liste dynamique exclut toute personne qui ne remplit pas les critères. Si une personne est admissible, l’enregistrement de l’activité de campagne exécutée qui en résulte la liste est &quot;Qualifiée : TRUE&quot; (et FALSE dans le cas contraire).
* Les règles de qualification de la campagne de planification s’appliquent (Paramètres de campagne dynamique sous l’onglet Planning)
* Les campagnes exécutables ne peuvent pas être appelées dans les espaces de travail.
* Si vous utilisez l’action de flux [Supprimer du flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) ciblant une campagne exécutable, elle cible à la fois l’enfant et le parent.
* Tirer parti de l’héritage des jetons : si, par exemple, vous disposez d’un seul flux de notation commun déclenché par plusieurs ressources différentes, vous pouvez définir un score Mon jeton par défaut dans la campagne enfant et dans la campagne parente, de sorte que vous puissiez remplacer la valeur de la campagne Score enfant pour vos campagnes parentes (voir l’exemple ci-dessous).
* Les campagnes exécutables peuvent être appelées jusqu’à trois niveaux de profondeur (par exemple, Campagne parent > Enfant > Enfant).

>[!CAUTION]
>
>Ne laissez jamais vos listes dynamiques pour les campagnes exécutables non valides, sinon _personne_ ne sera admissible pour cette opération. La bonne pratique consiste à créer des ressources de liste dynamique distinctes, à les définir complètement et à s’assurer qu’elles sont valides. Ensuite, utilisez le filtre &quot;Membre de la liste dynamique&quot; dans la campagne exécutable afin de pouvoir échanger votre définition de liste dynamique.

## Exemple d’héritage du jeton {#token-inheritance-example}

Vous trouverez ci-dessous un exemple visuel de l’héritage du jeton dans une campagne exécutable et deux campagnes parents : l’une avec le contexte du jeton défini sur **[!UICONTROL True]**, l’autre sur **[!UICONTROL False]**.

Campagne enfant avec une note de changement symbolique.

![](assets/execute-campaign-3.png)

La campagne enfant est Mes jetons.

![](assets/execute-campaign-4.png)

### Exemple 1 - Vrai {#example-one-true}

À l’étape du flux Exécuter la campagne de la première campagne parente, le paramètre &quot;Utiliser le contexte du jeton de campagne parent&quot; est défini sur **True**.

![](assets/execute-campaign-5.png)

Mes jetons de la campagne parente.

![](assets/execute-campaign-6.png)

Résultats : le score a changé de +10.

![](assets/execute-campaign-7.png)

### Exemple 2 : False {#example-two-false}

À l’étape du flux Exécuter la campagne de la seconde campagne parente, le paramètre &quot;Utiliser le contexte du jeton de campagne parent&quot; est défini sur **False**.

![](assets/execute-campaign-8.png)

Mes jetons de la campagne parente.

![](assets/execute-campaign-9.png)

Résultats : le score reste inchangé, car la valeur de score de la campagne enfant, +0, a été utilisée.

![](assets/execute-campaign-10.png)
