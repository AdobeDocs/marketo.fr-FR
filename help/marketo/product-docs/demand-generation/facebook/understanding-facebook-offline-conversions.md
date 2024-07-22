---
unique-page-id: 11383945
description: Présentation des conversions hors ligne Facebook - Documents Marketo - Documentation du produit
title: Présentation des conversions hors ligne de Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Présentation des conversions hors ligne de Facebook {#understanding-facebook-offline-conversions}

Les campagnes facebook Lead Ads génèrent des pistes et les envoient à Marketo pour les utiliser dans les campagnes marketing. Toutefois, sans visibilité sur les conversions hors ligne, l’annonceur Facebook ne peut pas savoir quelles publicités sont les plus efficaces. Voici un exemple.

>[!NOTE]
>
>**Exemple**
>
>Facebook Lead Ads exécute trois publicités.
>
>* La publicité 1 génère 20 pistes
>* La publicité 2 génère 30 pistes
>* La publicité 3 génère 50 pistes
>
>Sur la seule base de ces chiffres, Ad 3 semble le plus efficace.
>
>Cependant, lorsque vous examinez les données du côté Marketo, un autre article se développe.
>
>* La publicité 1 génère 10 ventes
>* La publicité 3 génère 2 ventes
>
>Cela signifie que la publicité 1, bien que générant moins de pistes, avait un taux de succès de 50 %, alors que la publicité 3 était à peine efficace du tout.
>
>Sans conversions hors ligne, l’annonceur investirait probablement plus d’argent dans la publicité 3. Avec les données de conversion hors ligne, l’annonceur investira plus probablement dans la publicité 1.

Vous pouvez [configurer les conversions hors ligne de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) pour envoyer les performances des publicités hors ligne à Facebook.

1. Assurez-vous que votre [intégration Facebook LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) est à jour.
1. Faites correspondre les étapes de votre modèle de cycle de revenu aux étapes de conversion hors ligne sur Facebook.
1. Lorsqu’une piste Facebook est générée à partir d’une annonce de piste Facebook et atteint une étape mappée, Marketo renvoie les données de conversion hors ligne à Facebook plusieurs fois par jour via une API sécurisée et automatisée. Les données s’affichent dans le rapport Gestionnaire de publicités Facebook .

>[!MORELIKETHIS]
>
>[ Configuration de conversions hors ligne Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
