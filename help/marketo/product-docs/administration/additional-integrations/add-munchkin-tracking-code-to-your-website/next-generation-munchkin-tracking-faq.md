---
unique-page-id: 10096583
description: FAQ about the next-generation [!DNL Munchkin] tracking rollout and the Is Anonymous filter change.
title: Next Generation [!DNL Munchkin] Tracking FAQ
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Next Generation [!DNL Munchkin] Tracking FAQ {#next-generation-munchkin-tracking-faq}

Marketo is rolling out next-generation web tracking technology in phases.

Here are the most important things to know:

* The &quot;Is Anonymous&quot; Smart List filter has been removed
* The number of web events (Visit Web Page, Clicked Link on Web Page) Marketo can ingest is increasing
* Your [!DNL Munchkin] code will not change, so no updates on your website are required

## When will my Marketo subscription be on [!DNL Munchkin] V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

An exact date is not yet available. Check this page for updates.

## Will I need to make any changes to my [!DNL Munchkin] tracking on my website? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Non. The [!DNL Munchkin] tracking code remains the same. No changes need to be made to your website.

>[!NOTE]
>
>This change does not affect Web Personalization (Real-Time Personalization). It continues to identify anonymous and known web visitors and personalize content in real time to these visitors.

## Why did Marketo remove the &quot;Is Anonymous&quot; filter from Smart Lists? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Marketo changed how anonymous people interact with Smart Campaigns. Before, they flowed through a smart campaign, just like known people. The &quot;Is Anonymous&quot; filter was used to specify that only known or only anonymous people flow through the campaign.

With [!DNL Munchkin] V2, Marketo will continue to track all anonymous activities; however, you are no longer able to apply filters to anonymous people. At the point of conversion (when the person becomes known in Marketo), all activities that occurred when the person was anonymous are appended to the person activity log and at this time they flow through the campaigns they qualify for.

If you are already using this filter in a Smart List (for example, in a Smart Campaign or a Report), it is not automatically removed from the Smart List. See below for more details.

>[!NOTE]
>
>**Trigger**: Visits Web Page, Web Page is Pricing Page >**Flux** : Modifier le score de +10 et le moment intéressant >**Web** : Page Tarification affichée
>
>Avec [!DNL Munchkin] V2, si une personne anonyme visite la page de tarification, elle ne participe pas immédiatement à la campagne. Au moment où la personne anonyme est connue, Marketo exécute cette campagne sur elle. Ils :
>
>* Obtenez un score de 10
>
>* Définissez l’activité Page web sur la date appropriée (date à laquelle ils se sont réellement rendus).
>
>* enregistrer un moment intéressant pour eux (avec la date à laquelle ils ont réellement visité la page, et non pas la date à laquelle ils se sont fait connaître) ;
>
>* Avoir une activité « Nouvelle personne » consignée, telle qu’elle est aujourd’hui

## Qu’advient-il de mes listes dynamiques qui possèdent déjà le filtre « Est anonyme » ? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Après la version d’hiver 16, si vous disposez d’anciennes campagnes intelligentes avec une liste dynamique comportant le filtre « Est anonyme », l’une des deux choses suivantes se produit :

1. Si la liste dynamique comporte le filtre « Est anonyme = Faux », alors rien ne se passera. Il est ignoré.
1. Si la liste dynamique présente le filtre « Est anonyme = Vrai », cette campagne échoue et une notification est envoyée.

## J’utilise Marketo depuis un certain temps. Comment savoir laquelle de mes campagnes utilise le filtre « Est anonyme » ? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Avant cette modification, Marketo a envoyé plusieurs notifications hebdomadaires à votre boîte de réception de notifications avec une liste de listes intelligentes, de campagnes intelligentes et de rapports qui utilisent le filtre « Est anonyme ». Ils peuvent vous aider à identifier l’endroit où vous utilisez actuellement ce filtre.

Passez-les en revue et identifiez l’emplacement où la valeur de « Est anonyme » est définie sur « Vrai », car il s’agit des campagnes affectées. La plupart du temps, ce paramètre est utilisé pour un type de notation. Consultez l’exemple ci-dessus pour comprendre comment ces campagnes vont fonctionner maintenant.

## Je voudrais une documentation plus détaillée. Où puis-je le trouver ? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consultez ces liens :

[Présentation des mises à niveau des leads anonymes](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Anonymous Lead Upgrades - Changes Inside Marketo UI](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Anonymous Lead Upgrades - Customer Action Needed](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Anonymous Lead Upgrades - Analytics Reports](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Anonymous Lead Upgrades - Release Schedule](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Anonymous Lead Upgrades - Under The Hood](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Anonymous Lead Promotion to Known Lead - [!DNL Munchkin] V2 Behavior](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## I have more questions! How do I get them answered? {#i-have-more-questions-how-do-i-get-them-answered}

Visit the [Marketo Community](https://experienceleaguecommunities.adobe.com/?profile.language=fr){target="_blank"}. You can also contact Marketo Support. They are happy to answer your questions.
