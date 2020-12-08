---
unique-page-id: 10096583
description: FAQ sur le suivi de Munchkin de nouvelle génération - Docs marketing - Documentation du produit
title: FAQ sur le suivi de Munchkin de nouvelle génération
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# FAQ sur le suivi de Munchkin de nouvelle génération {#next-generation-munchkin-tracking-faq}

Nous sommes heureux d&#39;annoncer que nous allons bientôt commencer un déploiement progressif de notre technologie de suivi Web de prochaine génération.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Voici les éléments les plus importants à savoir :

* Nous supprimons le filtre de Liste dynamique &quot;Is Anonymous&quot; avec notre version du 1er trimestre (déjà terminée).
* Nous augmentons le nombre de événements Web (Page Web de visite, Lien cliqué sur la page Web) que nous pouvons ingérer
* Votre code Munchkin ne changera pas. Aucune mise à jour de votre site Web n’est donc requise.

## Quand mon abonnement Marketo sera-t-il sur Munchkin V2 ? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Nous n&#39;avons pas encore de date exacte, mais veuillez revenir ici pour les mises à jour.

## Dois-je apporter des modifications au suivi de ma serviette Munchkin sur mon site Web ? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Non. Le code de suivi de Munchkin reste le même. Aucune modification n’est nécessaire pour votre site Web.

>[!NOTE]
>
>Cette modification n’a aucune incidence sur la personnalisation Web (personnalisation en temps réel). Il continue à identifier des visiteurs web anonymes et connus et à personnaliser le contenu en temps réel pour ces visiteurs.

## Pourquoi Marketo a-t-il supprimé le filtre &quot;Is Anonymous&quot; des Listes dynamiques ? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Nous avons changé la façon dont les personnes anonymes interagissent avec les campagnes intelligentes. Avant, ils passaient par une campagne intelligente, tout comme les gens connus. Le filtre &quot;Est anonyme&quot; a été utilisé pour spécifier que seules les personnes connues ou anonymes circulent dans la campagne.

Avec Munchkin V2, nous continuerons à suivre toutes les activités anonymes ; cependant, vous ne pouvez plus appliquer des filtres à des personnes anonymes. Au moment de la conversion (lorsque la personne est connue dans Marketo), toutes les activités survenues lorsque la personne était anonyme sont ajoutées au journal des activités de la personne et, à ce moment, elles passent par les campagnes pour lesquelles elles remplissent les conditions requises.

Si vous utilisez déjà ce filtre dans une Liste dynamique (par exemple, dans une Campaign dynamique ou un rapport), il n’est pas automatiquement supprimé de la Liste dynamique. Voir ci-dessous pour plus de détails.

>[!NOTE]
>
>**Exemple**
>
>**Déclencheur**: Page Web Visites, page Web est la page Tarification\
>**Flux**: Changer de note +10 et moment intéressant, **Web**: Page Tarifs affichés
>
>Avec Munchkin V2, si une personne anonyme visite la page de tarification, elle n&#39;entre pas immédiatement dans la campagne. Au moment où la personne anonyme sera connue, nous lui lancerons cette campagne. Elle :
>
>* Obtenez un score de 10
   >
   >
* L&#39;activité de la page Web est-elle définie à la date appropriée (date à laquelle elle s&#39;est effectivement rendue) ?
   >
   >
* Ayez un moment intéressant consigné pour elle (avec la date à laquelle elle a réellement visité la page, et non quand elle a été connue)
   >
   >
* Ayez une activité &quot;Nouvelle personne&quot; enregistrée, telle qu’elle est actuellement

>



## Qu’advient-il de mes Listes dynamiques qui disposent déjà du filtre &quot;Est-ce anonyme&quot; ? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Après notre version de l’hiver 16, si vous avez d’anciennes campagnes dynamiques avec une Liste dynamique qui comporte le filtre &quot;Est anonyme&quot;, une des deux choses se produit :

1. Si la Liste dynamique comporte le filtre &quot;Est anonyme = False&quot;, rien ne se passera. Nous l&#39;ignorerons.
1. Si la Liste dynamique comporte le filtre &quot;Est anonyme = True&quot;, cette campagne échoue et vous recevrez une notification.

## J&#39;utilise Marketo depuis un moment. Comment savoir laquelle de mes campagnes utilise le filtre &quot;Est anonyme&quot; ? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Avant de procéder à cette modification, nous avons envoyé plusieurs notifications hebdomadaires à votre boîte de réception Notifications avec une liste de Listes dynamiques, de campagnes dynamiques et de rapports qui utilisent le filtre &quot;Est anonyme&quot;. Elles peuvent vous aider à déterminer où vous utilisez actuellement ce filtre.

Vérifiez-les et identifiez l’emplacement où l’option &quot;Est anonyme&quot; est définie sur True, car il s’agit des campagnes qui sont affectées. La plupart du temps, les clients utilisent ce paramètre pour obtenir un certain score. Consultez l&#39;exemple ci-dessus pour comprendre comment ces campagnes vont fonctionner maintenant.

## Je voudrais une documentation plus détaillée. Où puis-je le trouver ? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consultez ces liens :

[Présentation des mises à niveau des pistes anonymes](https://nation.marketo.com/docs/DOC-2937)

[Mises à niveau des pistes anonymes - Modifications dans l’interface utilisateur de Marketing Cloud](https://nation.marketo.com/docs/DOC-2938)

[Mises à niveau des pistes anonymes - Action client requise](https://nation.marketo.com/docs/DOC-2939)

[Mises à niveau des pistes anonymes - Rapports Analytics](https://nation.marketo.com/docs/DOC-2940)

[Mises à niveau des pistes anonymes - Calendrier de publication](https://nation.marketo.com/docs/DOC-2961)

[Mises à niveau des pistes anonymes - Sous la houe](https://nation.marketo.com/docs/DOC-2962)

[Promotion anonyme de pistes vers le comportement connu - Munchkin V2](https://nation.marketo.com/docs/DOC-2963)

## J&#39;ai plus de questions ! Comment puis-je leur faire répondre ? {#i-have-more-questions-how-do-i-get-them-answered}

Veuillez contacter la [communauté](https://nation.marketo.com/welcome). Vous pouvez également envoyer un courriel à [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#4c3f393c3c233e380c212d3e27293823622f232162) Ils seront heureux de répondre à vos questions.
