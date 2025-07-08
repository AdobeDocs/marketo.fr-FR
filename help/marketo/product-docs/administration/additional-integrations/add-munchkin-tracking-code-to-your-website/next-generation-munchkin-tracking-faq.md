---
unique-page-id: 10096583
description: FAQ sur le suivi  [!DNL Munchkin]  nouvelle génération - Documents Marketo - Documentation du produit
title: FAQ sur le tracking  [!DNL Munchkin]  nouvelle génération
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: ea07c5c83c51fef4eb454562f041db685cf13775
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Questions fréquentes sur le suivi des [!DNL Munchkin] de nouvelle génération {#next-generation-munchkin-tracking-faq}

Nous sommes ravis d’annoncer que nous allons bientôt commencer le déploiement échelonné de notre technologie de suivi Web de prochaine génération.

Voici les informations les plus importantes à connaître :

* Nous supprimons le filtre de liste dynamique « Est anonyme » avec notre version du 1er trimestre (déjà terminé)
* Nous augmentons le nombre d’événements web (Page web de visite, Lien cliqué sur la page web) que nous pouvons ingérer
* Votre code [!DNL Munchkin] ne changera pas. Aucune mise à jour de votre site web n’est donc requise

## Quand mon abonnement Marketo sera-t-il disponible sur [!DNL Munchkin] V2 ? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Nous n&#39;avons pas encore de date exacte, mais veuillez vérifier ici pour les mises à jour.

## Vais-je devoir apporter des modifications à mon suivi des [!DNL Munchkin] sur mon site web ? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Non. Le code de suivi [!DNL Munchkin] reste le même. Aucune modification ne doit être apportée à votre site web.

>[!NOTE]
>
>Cette modification n’affecte pas Web Personalization (Real-Time Personalization). Il continue à identifier les visiteurs web anonymes et connus et à personnaliser le contenu en temps réel pour ces visiteurs.

## Pourquoi Marketo a-t-il supprimé le filtre « Est anonyme » des listes dynamiques ? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Nous avons modifié la manière dont les personnes anonymes interagissent avec les campagnes intelligentes. Auparavant, ils suivaient une campagne intelligente, tout comme les gens connus. Le filtre « Est anonyme » a été utilisé pour spécifier que seules des personnes connues ou anonymes circulent dans la campagne.

Avec [!DNL Munchkin] V2, nous continuerons à suivre toutes les activités anonymes. Cependant, vous ne pouvez plus appliquer de filtres aux personnes anonymes. Au moment de la conversion (lorsque la personne est connue dans Marketo), toutes les activités qui se sont produites lorsque la personne était anonyme sont ajoutées au journal des activités de la personne et, à ce stade, elles traversent les campagnes pour lesquelles elles sont qualifiées.

Si vous utilisez déjà ce filtre dans une liste dynamique (par exemple, dans une campagne dynamique ou un rapport), il n’est pas automatiquement supprimé de la liste dynamique. Voir ci-dessous pour plus de détails.

>[!NOTE]
>
>**Déclencheur** : page Web Visites, page Web est page de tarification\
>**Flux** : Modifier le score de +10 et le moment intéressant
>>**Web** : Page Tarification affichée
>
>Avec [!DNL Munchkin] V2, si une personne anonyme visite la page de tarification, elle ne participe pas immédiatement à la campagne. Au moment où la personne anonyme sera connue, nous lancerons cette campagne sur elle. Elle :
>
>* Obtenez un score de 10
>
>* Régler l’activité de la page web à la date correcte (date à laquelle elle s’est rendue)
>
>* Enregistrer un moment intéressant pour elle (avec la date à laquelle elle a réellement visité la page, et non pas la date à laquelle elle a été connue)
>
>* Avoir une activité « Nouvelle personne » consignée, telle qu’elle est aujourd’hui

## Qu’advient-il de mes listes dynamiques qui possèdent déjà le filtre « Est anonyme » ? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Après notre version d’hiver 16, si vous disposez d’anciennes campagnes intelligentes avec une liste dynamique comportant le filtre « Est anonyme », l’une des deux choses suivantes se produit :

1. Si la liste dynamique comporte le filtre « Est anonyme = Faux », alors rien ne se passera. On l&#39;ignorera.
1. Si la liste dynamique présente le filtre « Est anonyme = Vrai », cette campagne échoue et une notification vous est envoyée.

## J&#39;utilise Marketo depuis un moment. Comment savoir laquelle de mes campagnes utilise le filtre « Est anonyme » ? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Avant d’apporter cette modification, nous avons envoyé plusieurs notifications hebdomadaires à votre boîte de réception de notifications avec une liste de listes intelligentes, de campagnes intelligentes et de rapports qui utilisent le filtre « Est anonyme ». Ils peuvent vous aider à identifier l’endroit où vous utilisez actuellement ce filtre.

Passez-les en revue et identifiez les campagnes pour lesquelles l’option « Est anonyme » est définie sur « Vrai », car il s’agit des campagnes affectées. La plupart du temps, les clients utilisent ce paramètre pour un certain type de notation. Consultez l’exemple ci-dessus pour comprendre comment ces campagnes vont fonctionner maintenant.

## Je voudrais une documentation plus détaillée. Où puis-je le trouver ? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consultez ces liens :

[Présentation des mises à niveau de leads anonymes](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Mises à niveau de leads anonymes - Modifications dans l’interface utilisateur de Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Mises À Niveau De Prospects Anonymes - Action Du Client Nécessaire](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Mises à niveau de leads anonymes - Rapports Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Mises à niveau de leads anonymes - Calendrier des versions](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Mises à niveau de leads anonymes - Sous le capot](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promotion de lead anonyme vers un comportement de lead connu - [!DNL Munchkin] V2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## J&#39;ai d&#39;autres questions ! Comment puis-je obtenir des réponses ? {#i-have-more-questions-how-do-i-get-them-answered}

Contactez la [communauté](https://nation.marketo.com/){target="_blank"}. Vous pouvez également contacter le support technique de [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. Ils seront heureux de répondre à vos questions.
