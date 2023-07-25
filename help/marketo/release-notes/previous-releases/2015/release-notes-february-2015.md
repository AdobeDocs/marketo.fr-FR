---
unique-page-id: 6094890
description: Notes de mise à jour - Février 2015 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Février 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 21%

---

# Notes de mise à jour : Février 2015 {#release-notes-february}

Les fonctionnalités suivantes sont incluses dans la version de février 2015. Vérifiez la disponibilité de vos fonctionnalités dans Marketo Edition. Après la version, veillez à revenir à la page pour trouver des liens vers des articles détaillés pour chaque fonctionnalité. Dum roll...

## Améliorations de l’automatisation du marketing {#marketing-automation-enhancements}

**[Déplacer une campagne intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Hourra ! Vous pouvez désormais insérer ou extraire les campagnes intelligentes des programmes grâce à la fonction glisser-déposer ou Déplacer dans l’arborescence.

**[Dynamics 2015 (En ligne)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - pris en charge !

**Modifications des certificats HTTPS**

Pour protéger la confidentialité et l’intégrité des données client et des services SaaS, Marketo suit les bonnes pratiques du secteur SaaS.

et remplaceront les protocoles de sécurité actuellement utilisés (SHA-1 et SSL) par des versions plus sécurisées (SHA-2 (ou SHA-256) et TLS) pour les domaines suivants :

* marketo.net (trafic Munchkin chiffré)

* [marketo.com](https://marketo.com) (applications SaaS principales)

Cela se produira peu après cette version. Le protocole SHA-1 sera temporairement pris en charge sur [mktoapi.com](https://mktoapi.com) d’ici décembre 2015 pour permettre aux propriétaires des systèmes et applications hérités de mettre à jour leurs systèmes avec la compatibilité SHA-2.

**Secure Munchkin**

Nous supprimons la prise en charge de SSL3. Jusqu’à présent, SSL3 était pris en charge pour les anciens navigateurs Web, mais en 2015, ces navigateurs n’affichaient plus de trafic Web important. Cela affecterait uniquement Munchkin lorsqu’il est utilisé sur des pages sécurisées et se déploie lentement après la publication de février.

## Améliorations de la personnalisation en temps réel {#real-time-personalization-enhancements}

**[URL cible pour les campagnes](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Sélectionnez les pages que votre campagne en temps réel affichera en utilisant « Ajouter une URL cible ». Cette fonctionnalité fonctionne avec tous les types de campagne (Boîte de dialogue, Dans la zone, Widgets), mais elle est particulièrement utile pour les campagnes Dans la zone où une campagne s’affichera dans l’identifiant de zone pour l’URL cible sélectionnée uniquement. Il prend en charge l’ajout de plusieurs URL pour cibler différentes pages web.

![](assets/image2015-2-19-11-3a0-3a30.png)

**Pays et État ajoutés au ciblage basé sur le compte**

Les valeurs Pays et État peuvent désormais être ajoutées à vos Listes de comptes nommés. Cibler de futurs comptes clés à partir de lieux spécifiques.
