---
unique-page-id: 6094890
description: Notes de mise à jour - Février 2015 - Marketo Docs - Documentation du produit
title: Notes de mise à jour - Février 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 21%

---

# Notes de mise à jour : Février 2015 {#release-notes-february}

Les fonctionnalités suivantes sont incluses dans la version de février 2015. Veuillez vérifier la disponibilité des fonctionnalités de Marketo Edition. Après la publication, n&#39;oubliez pas de revenir pour trouver des liens vers des articles détaillés pour chaque fonction. Lancement de tambour...

## Améliorations de l&#39;automatisation du marketing {#marketing-automation-enhancements}

**[Déplacer une campagne intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Hourra ! Vous pouvez désormais insérer ou extraire les campagnes intelligentes des programmes grâce à la fonction glisser-déposer ou Déplacer dans l’arborescence.

**[Dynamics 2015 (En ligne)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - pris en charge !

**Modifications des certificats HTTPS**

Pour protéger la confidentialité et l’intégrité des données client et des services SaaS, Marketo suit les meilleures pratiques du secteur SaaS

et remplacera les protocoles de sécurité actuellement utilisés (SHA-1 et SSL) par des versions plus sécurisées (SHA-2 (ou SHA-256) et TLS) pour les domaines suivants :

* [marketo.net](https://marketo.net)  (trafic Munchkin chiffré)

* [marketo.com](https://marketo.com)  (applications SaaS principales)

Cela se produira peu après cette version. Le protocole SHA-1 sera temporairement pris en charge sur le domaine [mktoapi.com](https://mktoapi.com) jusqu&#39;en décembre 2015 pour permettre aux propriétaires de systèmes et d&#39;applications hérités de mettre à jour leurs systèmes avec la compatibilité SHA-2.

**Munchkin sécurisé**

Nous supprimons la prise en charge de SSL3. Jusqu&#39;à présent, nous avons maintenu SSL3 pour maintenir la prise en charge des anciens navigateurs Web, mais en 2015, nous ne voyons plus de trafic Web significatif de ces navigateurs. Cela n&#39;affecterait Munchkin que lorsqu&#39;il est utilisé sur des pages sécurisées et se déploiera lentement après la publication de février.

## Améliorations de la personnalisation en temps réel {#real-time-personalization-enhancements}

**[URL de cible pour les campagnes](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Sélectionnez les pages que votre campagne en temps réel affichera en utilisant « Ajouter une URL cible ». Cette fonctionnalité fonctionne avec tous les types de campagne (Boîte de dialogue, Zone, Widgets), mais elle s’avère particulièrement utile pour les campagnes en zone dans lesquelles une campagne s’affichera dans l’identifiant de zone pour l’URL de cible sélectionnée uniquement. Il prend en charge l’ajout de plusieurs URL à la cible de différentes pages Web.

![](assets/image2015-2-19-11-3a0-3a30.png)

**Pays et État ajoutés au ciblage basé sur le compte**

Les valeurs Pays et État peuvent désormais être ajoutées à vos Listes de comptes nommés. Cibler de futurs comptes clés à partir de lieux spécifiques.
