---
unique-page-id: 6094890
description: Notes de mise à jour - Février 2015 - Documents marketing - Documentation du produit
title: Notes de mise à jour - Février 2015
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---


# Notes de mise à jour : Février 2015 {#release-notes-february}

Les fonctionnalités suivantes sont incluses dans la version de février 2015. Veuillez vérifier la disponibilité des fonctionnalités de votre édition Marketing. Après la publication, n&#39;oubliez pas de revenir pour trouver des liens vers des articles détaillés pour chaque fonction. Lancement de tambour...

## Améliorations de l’automatisation du marketing {#marketing-automation-enhancements}

** [Move Smart Campaign](../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Réjouissez-vous ! Désormais, vous pouvez déplacer des campagnes intelligentes dans et hors des programmes à l’aide de la fonction glisser-déposer ou Déplacer dans l’arborescence.

** [Dynamics 2015 (Online)](http://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises) **- pris en charge !

**Modifications des certificats HTTPS**

Pour protéger la confidentialité et l’intégrité des données client et des services SaaS, Marketo suit les meilleures pratiques du secteur SaaS

et remplacera les protocoles de sécurité actuellement utilisés (SHA-1 et SSL) par des versions plus sécurisées (SHA-2 (ou SHA-256) et TLS) pour les domaines suivants :

`·` [marketo.net](http://marketo.net) (trafic Munchkin chiffré)

`·` [marketo.com](http://marketo.com) (applications SaaS principales)

Cela se produira peu après cette version. Le protocole SHA-1 sera temporairement pris en charge sur le domaine [mktoapi.com](http://mktoapi.com) jusqu&#39;en décembre 2015 pour permettre aux propriétaires de systèmes et d&#39;applications hérités de mettre à jour leurs systèmes avec la compatibilité SHA-2.

**Munchkin sécurisé**

Nous supprimons la prise en charge de SSL3. Jusqu&#39;à présent, nous avons maintenu SSL3 pour maintenir la prise en charge des anciens navigateurs Web, mais en 2015, nous ne voyons plus de trafic Web significatif de ces navigateurs. Cela n&#39;affecterait Munchkin que lorsqu&#39;il est utilisé sur des pages sécurisées et se déploiera lentement après la publication de février.

## Améliorations de la personnalisation en temps réel {#real-time-personalization-enhancements}

** URL [de Cible pour les campagnes](../../product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Sélectionnez les pages sur lesquelles votre campagne en temps réel doit s&#39;afficher à l&#39;aide de l&#39;option &quot;Ajouter une URL de Cible&quot;. Cette fonctionnalité fonctionne avec tous les types de campagne (Boîte de dialogue, Zone, Widgets), mais elle s’avère particulièrement utile pour les campagnes en zone dans lesquelles une campagne s’affichera dans l’identifiant de zone pour l’URL de cible sélectionnée uniquement. Il prend en charge l’ajout de plusieurs URL à la cible de différentes pages Web.

![](assets/image2015-2-19-11-3a0-3a30.png)

** [Pays et État Ajoutés au ciblage](https://docs.marketo.com/display/DOCS/View+a+Named+Account+List)basé sur les comptes**

Le pays et l’état peuvent désormais être ajoutés à vos Listes de compte nommé. Prospects de compte clés de cible à partir d’emplacements spécifiques.
