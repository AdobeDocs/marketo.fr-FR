---
unique-page-id: 10096583
description: Questions fréquentes sur le déploiement du suivi  [!DNL Munchkin]  nouvelle génération et le changement de filtre Est anonyme.
title: FAQ sur le tracking  [!DNL Munchkin]  nouvelle génération
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
source-git-commit: 689773f0d6f87b65d5299ecc11f3de11f7e66775
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Questions fréquentes sur le suivi des [!DNL Munchkin] de nouvelle génération {#next-generation-munchkin-tracking-faq}

Marketo déploie la technologie de tracking web de nouvelle génération par phases.

Voici les informations les plus importantes à connaître :

* Le filtre de liste dynamique « Est anonyme » a été supprimé
* Le nombre d’événements web (Visiter une page web, Lien cliqué sur la page web) que Marketo peut ingérer augmente
* Votre code [!DNL Munchkin] ne changera pas. Aucune mise à jour de votre site web n’est donc requise

## Quand mon abonnement Marketo sera-t-il disponible sur [!DNL Munchkin] V2 ? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Aucune date exacte n’est encore disponible. Consultez cette page pour connaître les mises à jour.

## Vais-je devoir apporter des modifications à mon suivi des [!DNL Munchkin] sur mon site web ? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Non. Le code de suivi [!DNL Munchkin] reste le même. Aucune modification ne doit être apportée à votre site web.

>[!NOTE]
>
>Cette modification n’affecte pas Web Personalization (Real-Time Personalization). Il continue à identifier les visiteurs web anonymes et connus et à personnaliser le contenu en temps réel pour ces visiteurs.

## Pourquoi Marketo a-t-il supprimé le filtre « Est anonyme » des listes dynamiques ? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Marketo a modifié la manière dont les personnes anonymes interagissent avec les campagnes intelligentes. Auparavant, ils suivaient une campagne intelligente, tout comme les gens connus. Le filtre « Est anonyme » a été utilisé pour spécifier que seules des personnes connues ou anonymes circulent dans la campagne.

Avec [!DNL Munchkin] V2, Marketo continuera à suivre toutes les activités anonymes ; cependant, vous ne pouvez plus appliquer de filtres aux personnes anonymes. Au moment de la conversion (lorsque la personne est connue dans Marketo), toutes les activités qui se sont produites lorsque la personne était anonyme sont ajoutées au journal des activités de la personne et, à ce stade, elles traversent les campagnes pour lesquelles elles sont qualifiées.

Si vous utilisez déjà ce filtre dans une liste dynamique (par exemple, dans une campagne dynamique ou un rapport), il n’est pas automatiquement supprimé de la liste dynamique. Voir ci-dessous pour plus de détails.

>[!NOTE]
>
>**Déclencheur** : page Web Visites, page Web est page de tarification >**Flux** : Modifier le score de +10 et le moment intéressant >**Web** : Page Tarification affichée
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

[Mises à niveau de leads anonymes - Modifications dans l’interface utilisateur de Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Mises à niveau de leads anonymes - Action du client nécessaire](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Mises à niveau de leads anonymes - Rapports Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Mises à niveau de leads anonymes - Calendrier des versions](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Mises à niveau de leads anonymes - En cours](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promotion de lead anonyme vers un comportement de lead connu - [!DNL Munchkin] V2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## J&#39;ai d&#39;autres questions ! Comment puis-je obtenir des réponses ? {#i-have-more-questions-how-do-i-get-them-answered}

Visitez la [Communauté &#x200B;](https://experienceleaguecommunities.adobe.com/?profile.language=fr){target="_blank"}. Vous pouvez également contacter le support technique de Marketo. Ils se feront un plaisir de répondre à vos questions.
