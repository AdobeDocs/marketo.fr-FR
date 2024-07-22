---
unique-page-id: 2951056
description: Notes de mise à jour - Septembre 2013 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Septembre 2013
exl-id: 43428813-0405-4c35-9165-f189fbb5ffb7
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 11%

---

# Notes de mise à jour : septembre 2013 {#release-notes-september}

Les fonctionnalités suivantes sont incluses dans la version de septembre.

## URL courtes {#shorter-urls}

Les URL des e-mails sont désormais plus courtes et plus agréables pour le destinataire, mais elles conservent leur fonctionnalité de suivi.

>[!CAUTION]
>
>Lorsque nous passons aux URL courtes, les liens contenus dans les emails envoyés avant la version de septembre expirent 90 jours après cette version.

Utilisez des données provenant d’objets personnalisés Marketo ou ajoutez une logique conditionnelle au contenu de votre email à l’aide du langage de modèle Velocity.

![](assets/image2014-9-22-17-3a10-3a56.png)

## Modifier Envoyer un test pour envoyer un exemple {#change-send-test-to-send-sample}

Nous avons renommé l’action Envoyer le test pour envoyer un exemple

## Exemple d’envoi personnalisé {#personalized-send-sample-email}

Lorsque vous envoyez un exemple d&#39;email, vous pouvez sélectionner le nom d&#39;un prospect pour personnaliser l&#39;exemple d&#39;email.

![](assets/image2014-9-22-17-3a11-3a22.png)

## Nouveau champ de synchronisation pour GoToWebinar {#additional-field-sync-for-gotowebinar}

Vous pouvez synchroniser le nom de l’entreprise et le titre de la tâche de votre formulaire Marketo dans GoToWebinar. Pour activer ces champs supplémentaires, accédez à Partenaires d’événements et cochez &quot;Activer les champs supplémentaires&quot;.

![](assets/image2014-9-22-17-3a11-3a53.png)

## Limiter la connexion de l’utilisateur à SSO uniquement {#restrict-user-login-to-sso-only}

Configurez les abonnements pour permettre uniquement aux utilisateurs de Marketo de se connecter via SSO et non via l’écran de connexion normal.

## Recherche des virus dans les fichiers téléchargés {#virus-scan-of-uploaded-files}

Les fichiers téléchargés dans Design Studio sont automatiquement scannés et bloqués s&#39;ils contiennent des virus.

## Exporter l&#39;analyseur d&#39;influence sur l&#39;opportunité {#export-opportunity-influence-analyzer}

Vous pouvez désormais exporter les données dans l’analyseur d’influence d’opportunité vers Excel. Chaque fichier Excel exporté contient toutes les interactions marketing pour toutes les pistes (y compris celles qui n’ont pas de rôle dans l’opportunité) ainsi que toutes les opportunités sous le compte sélectionné dans l’analyseur. Les lignes d’opportunité sont mises en surbrillance en vert. Vous pouvez utiliser les fonctionnalités natives de filtrage des données d’Excel si vous devez vous concentrer sur des pistes spécifiques ou des activités marketing.

![](assets/image2014-9-22-17-3a12-3a23.png)

## Paramètres d&#39;attribution du programme {#program-attribution-settings}

Vous pouvez modifier la manière dont Marketo associe les contacts et les opportunités pour les mesures d’attribution Première touche et multipoint, y compris la possibilité d’effectuer une attribution basée sur le compte. Ces paramètres auront un impact sur les mesures d’attribution dans les rapports de l’Explorateur de recettes sous la zone Analyse des opportunités du programme et la zone Analyse des opportunités . Cela aura également une incidence sur les mesures d’attribution dans Program Analyzer.

Vous pouvez définir les paramètres d’attribution du programme sur l’un des trois choix. La modification de ce paramètre ne modifie aucune donnée de Marketo ou de gestion de la relation client ; elle modifie simplement l’exécution des rapports et peut être annulée à tout moment.

Le paramètre Explicite n’examine que les contacts avec des rôles (comportement actuel). Implicit examine tous les contacts associés au compte, quel que soit leur rôle. Si possible, nous vous recommandons vivement d&#39;utiliser le mode Explicite . L’utilisation d’Implicit peut créer des faux positifs, des personnes qui ont le crédit d’une opportunité malgré l’absence d’une réelle influence sur l’opportunité.

![](assets/image2014-9-22-17-3a12-3a43.png)

## Sales Insight disponible en français et en allemand (Salesforce uniquement) {#sales-insight-available-in-french-and-german-salesforce-only}

Téléchargez la dernière version de Marketo Lead Management et de Marketo Sales Insight depuis AppExchange afin que vos vendeurs français et allemands puissent consulter le contenu de Sales Insight dans la langue de leur choix.

![](assets/image2014-9-22-17-3a13-3a12.png)

## Interface utilisateur cobalt {#cobalt-user-interface}

Au cours des prochains mois, un nouveau thème est en cours de déploiement dans différentes parties de l’application. Ce mois-ci, vous remarquerez peut-être de nouvelles fenêtres modales bleues.
