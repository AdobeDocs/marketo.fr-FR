---
unique-page-id: 10912085
description: Adresses IP partagées et dédiées - Documents Marketo - Documentation du produit
title: Adresses IP partagées et dédiées
exl-id: 3d7a78f4-531a-4ad7-a20b-1385bd62d1d9
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 3%

---

# Adresses IP partagées et dédiées {#shared-and-dedicated-ip-addresses}

## Qu’est-ce qu’une adresse IP ? {#what-is-an-ip-address}

Libellé numérique indiquant l’adresse d’un ordinateur connecté à Internet.

## Que sont les adresses IP partagées ? {#what-are-shared-ip-addresses}

Cela se rapporte au cas où plusieurs expéditeurs utilisent les mêmes adresses IP pour lancer des campagnes par e-mail. Ils partagent tous les mêmes adresses IP d’envoi.

## Qu’est-ce qu’une adresse IP dédiée ? {#what-is-a-dedicated-ip-address}

Adresse IP spécifique à l’utilisateur à partir de laquelle un seul expéditeur effectue l’envoi.

## Qu’est-ce qui est préférable : partagé ou dédié ? {#which-is-better-shared-or-dedicated}

Comme d’habitude, il y a des avantages et des inconvénients aux deux options.

**Avantages et inconvénients d’une adresse IP dédiée**

_Avantages_

**Réputation** - Vous êtes propriétaire de votre réputation et de votre délivrabilité.
**Surveillance** - La surveillance de vos rapports de délivrabilité vous permet de répondre rapidement aux modifications de vos mesures de diffusion.
**Résolution de problèmes** - Il est plus facile de rechercher, de comprendre et de résoudre les problèmes de diffusion.

_Inconvénients_

**Modifications de volume** - Les pics de volume peuvent avoir une incidence négative sur votre réputation et doivent être gérés.
**Processus de préchauffage d’IP** - La réputation s’établit au fil du temps. Certains fournisseurs d’accès à Internet (FAI) limitent les adresses IP sans historique de volume, vous devrez donc établir une réputation au cours des premières semaines (Marketo peut vous guider).
**Coût** - L’envoi de messages depuis une adresse IP dédiée auprès d’un fournisseur entraîne généralement des frais supplémentaires.

**Avantages et inconvénients d’une adresse IP partagée**

_Avantages_

**Bons colocataires** - Si les personnes avec lesquelles vous partagez votre adresse IP suivent les bonnes pratiques d’envoi, vous en bénéficierez.
**Fréquence de publipostage** - Il n’existe pas de fréquence de publipostage minimale nécessaire pour être éligible à une adresse IP partagée, contrairement aux adresses IP dédiées.
**Coût** - Il n’y a jamais de frais supplémentaires à envoyer à partir d’une adresse IP partagée.

_Inconvénients_

**Mauvais colocataires** - Si les personnes avec lesquelles vous partagez votre adresse IP adoptent de mauvaises pratiques d’envoi, vos campagnes par e-mail pourraient être affectées.
**Contrôle** - Vous avez beaucoup moins de contrôle sur la réputation de votre expéditeur.
**Résolution des problèmes** - Il peut souvent être plus difficile de résoudre un problème lors de l’envoi de messages à partir d’adresses IP partagées.

>[!NOTE]
>
>Lors de la prise de décision, il y a un autre facteur important à prendre en compte : le volume d’envoi. Si vous prévoyez d’envoyer moins de 100 000 e-mails par mois, ou moins de deux mailings par mois, vous ne bénéficierez probablement pas d’une adresse IP dédiée. Des numéros d’envoi comme celui-ci sont considérés comme faibles et il serait difficile de garder votre adresse IP dédiée suffisamment « chaude » pour être considérée comme sûre par les principaux FAI. En gros, si vous ne publiez pas assez souvent, les FAI verront un publipostage comme une « augmentation » soudaine de l&#39;activité, et pourraient finir par le bloquer comme spam présumé.

Si vous avez des questions ou si vous souhaitez configurer une adresse IP dédiée, contactez votre représentant commercial Marketo.
