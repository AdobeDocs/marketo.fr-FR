---
unique-page-id: 10096583
description: "Génération suivante [!DNL Munchkin] FAQ sur le suivi - Documents Marketo - Documentation du produit"
title: "Génération suivante [!DNL Munchkin] FAQ sur le suivi"
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 1a6f029b8c9665ecd7fcc066004d88ee6c915505
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# Génération suivante [!DNL Munchkin] FAQ sur le suivi {#next-generation-munchkin-tracking-faq}

Nous sommes ravis d’annoncer que nous allons bientôt lancer un déploiement progressif de notre nouvelle technologie de tracking Web.

Voici les éléments les plus importants à savoir :

* Nous supprimons le filtre Liste dynamique &quot;Is Anonymous&quot; avec notre version du 1er trimestre (déjà terminée).
* Nous augmentons le nombre d’événements web (Page web de la visite, Lien cliqué sur la page web) que nous pouvons ingérer.
* Votre [!DNL Munchkin] Le code ne change pas. Aucune mise à jour n’est donc requise sur votre site web.

## Quand mon abonnement Marketo sera-t-il activé ? [!DNL Munchkin] V2 ? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Nous n&#39;avons pas encore de date exacte, mais veuillez consulter les mises à jour ici.

## Dois-je apporter des modifications à mon [!DNL Munchkin] suivi sur mon site web ? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Nombre Le [!DNL Munchkin] le code de suivi reste le même. Aucune modification ne doit être apportée à votre site web.

>[!NOTE]
>
>Cette modification n’a aucune incidence sur la personnalisation web (personnalisation en temps réel). Il continue à identifier les visiteurs anonymes et connus et à personnaliser le contenu en temps réel pour ces visiteurs.

## Pourquoi Marketo a-t-il supprimé le filtre &quot;Is Anonymous&quot; des listes dynamiques ? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Nous avons modifié la manière dont les personnes anonymes interagissent avec les campagnes intelligentes. Avant, ils ont traversé une campagne intelligente, tout comme les gens connus. Le filtre &quot;Est anonyme&quot; a été utilisé pour indiquer que seules les personnes connues ou anonymes circulent dans la campagne.

Avec [!DNL Munchkin] V2, nous poursuivrons le suivi de toutes les activités anonymes ; cependant, vous ne pouvez plus appliquer de filtres aux personnes anonymes. Au point de conversion (lorsque la personne est connue dans Marketo), toutes les activités survenues lorsque la personne était anonyme sont ajoutées au journal d’activité de la personne et, à ce moment, elles transitent par les campagnes pour lesquelles elles remplissent les critères.

Si vous utilisez déjà ce filtre dans une liste dynamique (par exemple, dans une campagne dynamique ou un rapport), il n’est pas automatiquement supprimé de la liste dynamique. Voir ci-dessous pour plus de détails.

>[!NOTE]
>
>**Déclencheur**: Page web Visites, page web = page des tarifs\
>**Flux**: Score de changement +10 et moment intéressant
>**Web**: Page de tarification consultée
>
>Avec [!DNL Munchkin] V2, si une personne anonyme consulte la page des tarifs, elle ne rentre pas immédiatement dans l&#39;opération. Au moment où la personne anonyme sera connue, nous lui lancerons cette campagne. Elle :
>
>* Obtenir un score de 10
>
>* Définissez l’activité Page Web à la date appropriée (date à laquelle elle a réellement visité le site).
>
>* Ayez un moment intéressant consigné pour elle (avec la date à laquelle elle a réellement visité la page, et non quand elle a été connue)
>
>* Consignez une activité &quot;Nouvelle personne&quot; comme aujourd’hui


## Qu’advient-il de mes listes dynamiques qui disposent déjà du filtre &quot;Est-ce anonyme&quot; ? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Après notre version de l’hiver 16, si vous disposez d’anciennes campagnes dynamiques avec une liste dynamique qui contient le filtre &quot;Is Anonymous&quot;, deux choses se produiront :

1. Si le filtre &quot;Is Anonymous = False&quot; est appliqué à la liste dynamique, rien ne se produit. Nous l&#39;ignorerons.
1. Si le filtre &quot;Is Anonymous = True&quot; est appliqué à la liste dynamique, cette campagne échoue et vous recevez une notification.

## J&#39;utilise Marketo depuis un moment. Comment savoir laquelle de mes campagnes utilise le filtre &quot;Est anonyme&quot; ? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Avant d’apporter cette modification, nous avons envoyé plusieurs notifications hebdomadaires à votre boîte de réception de notifications avec une liste de listes dynamiques, de campagnes dynamiques et de rapports qui utilisent le filtre &quot;Est anonyme&quot;. Ils peuvent vous aider à identifier où vous utilisez actuellement ce filtre.

Consultez-les et identifiez l’emplacement où &quot;Est anonyme&quot; est défini sur True, car il s’agit des campagnes affectées. La plupart du temps, les clients utilisent ce paramètre pour une sorte de notation. Consultez l’exemple ci-dessus pour comprendre comment ces campagnes fonctionneront désormais.

## Je voudrais une documentation plus détaillée. Où puis-je le trouver ? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consultez les liens suivants :

[Présentation des mises à niveau de pistes anonymes](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Mises à niveau de pistes anonymes - Modifications dans l’interface utilisateur de Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Mises à niveau de pistes anonymes - Action client requise](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Mises à niveau des pistes anonymes - Rapports Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Mises à niveau de piste anonymes - Calendrier des versions](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Mises À Niveau Des Pistes Anonymes - Sous Le Bois](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promotion de piste anonyme vers piste connue - [!DNL Munchkin] Comportement V2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## J&#39;ai plus de questions ! Comment puis-je leur faire répondre ? {#i-have-more-questions-how-do-i-get-them-answered}

Veuillez contacter le [communauté](https://nation.marketo.com/){target="_blank"}. You can also contact [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. Ils seront heureux de répondre à vos questions.
