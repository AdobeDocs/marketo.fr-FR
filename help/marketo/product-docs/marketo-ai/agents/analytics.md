---
description: Discutez avec l’IA dédiée au Marketo des données de performances de Marketo Engage. Posez vos questions en langage simple et obtenez des réponses ancrées dans votre environnement Marketo.
title: Analytics
badge: Beta
hide: true
source-git-commit: 69749951d0397a837bee77d16baddc3342f68ec2
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# Analytics {#analytics}

Analytics vous permet d’avoir une conversation sur vos données de performances Marketo. Posez vos questions en langage simple et obtenez des réponses ancrées dans votre environnement Marketo.

>[!PREREQUISITES]
>
>* Pour utiliser cette fonctionnalité, vous devez d’abord accepter les termes [&#x200B; Core Gen-AI et les termes supplémentaires](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>
>* Vous devez avoir accès aux programmes et aux rapports sur lesquels vous vous renseignez.

>[!AVAILABILITY]
>
>Cette fonctionnalité est en version bêta fermée et fait actuellement l’objet d’un déploiement échelonné au cours des prochains mois. Vous saurez quand il a été activé pour votre abonnement lorsque la mosaïque _Créer avec l’IA_ s’affichera sur votre écran Mon Marketo.

## Utilisation {#how-to-use}

1. Dans Mon Marketo, cliquez sur la mosaïque **Créer avec l’IA**.

1. Dans la fenêtre d’invite, posez une question sur les performances. Précisez le calendrier ou le programme si vous en avez un en tête.

1. Consultez le résumé des retours de l’IA Marketo. Elle inclut des mesures clés telles que les taux d’ouverture, les taux de clics, les taux de conversion et le nombre de leads en fonction de ce que vous avez demandé.

1. Posez des questions de suivi pour explorer des domaines spécifiques (par exemple, « Quel e-mail de ce programme avait le taux de clic le plus élevé ? »). ou « Comment cela se compare-t-il au dernier trimestre ? »).

## Cas d’utilisation {#use-cases}

**Révision trimestrielle du programme** : un responsable de la génération de la demande se prépare pour une réunion de révision de la campagne. Ils demandent : « Comment mes programmes de formation au 2e trimestre se sont-ils comportés globalement ? » L’IA dédiée à Marketo renvoie les taux d’ouverture, les taux de clic sur l’ouverture, les taux de désabonnement et le nombre de personnes/prospects qui ont progressé vers MQL dans tous les programmes d’éducation du 2e trimestre, avec une note sur les programmes qui ont dépassé la moyenne du groupe.

**Comparaison de deux campagnes** : un responsable de campagne a exécuté deux versions d’une série d’invitations à un webinaire avec des objets différents. Ils demandent : «Comment le programme de webinaires d&#39;avril se compare-t-il au programme de mars en termes de taux d&#39;inscription ?» L’IA dédiée au Marketo renvoie les numéros d’enregistrement de chaque application et met en évidence la différence, afin que les utilisateurs puissent identifier l’approche qui a le mieux fonctionné.

**Recherche de contenu le plus performant** : un spécialiste des opérations marketing souhaite savoir quelles ressources d’e-mail ont généré le plus d’engagement le mois dernier. Ils demandent : « Quels emails ont eu les taux de clics les plus élevés en mai ? » L’IA dédiée aux Marketo renvoie une liste classée des ressources d’e-mail avec les taux de clics, afin qu’elles puissent identifier ce qui a résonné et informer les décisions de contenu futures.

## Éléments à noter {#things-to-note}

* Les réponses d’Analytics reposent sur les données disponibles dans votre instance Marketo. Si un programme n’est pas suivi ou si une mesure n’est pas capturée, l’IA dédiée au Marketo ne sera pas en mesure de créer des rapports à son sujet.
* Des périodes très longues ou des questions générales peuvent renvoyer des résumés de haut niveau plutôt que des détails précis. Par exemple : « Comment tous mes programmes se sont-ils comportés au cours des deux dernières années ? »
* L’IA dédiée aux Marketo peut faire apparaître des données, mais ne peut pas apporter de modifications à vos programmes ou rapports en fonction de ses découvertes.
* Pour des rapports personnalisés détaillés avec des filtres et des répartitions spécifiques, les outils de rapports intégrés de Marketo ou une intégration de BI peuvent être plus appropriés.
* L’attribution dans les campagnes multipoint nécessite une configuration de programme appropriée. L’IA dédiée au Marketo crée un rapport sur ce qui est suivi, et n’infère pas d’attribution qui n’a pas été configurée.
