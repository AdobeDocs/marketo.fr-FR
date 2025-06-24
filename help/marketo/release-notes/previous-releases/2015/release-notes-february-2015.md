---
unique-page-id: 6094890
description: Notes De Mise À Jour - Février 2015 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Février 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 13%

---

# Notes De Mise À Jour : Février 2015 {#release-notes-february}

Les fonctionnalités suivantes sont incluses dans la version de février 2015. Consultez votre édition Marketo pour connaître la disponibilité des fonctionnalités. Après la publication, veillez à revenir pour trouver des liens vers des articles détaillés pour chaque fonctionnalité. Rouleau de tambour...

## Améliorations de l’automatisation du marketing {#marketing-automation-enhancements}

**[Déplacer une campagne intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Hourra ! Vous pouvez désormais insérer ou extraire les campagnes intelligentes des programmes grâce à la fonction glisser-déposer ou Déplacer dans l’arborescence.

**[[!DNL Dynamics] 2015 (en ligne)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - pris en charge !

**Modifications du certificat HTTPS**

Afin de préserver la confidentialité et l’intégrité des données clients et des services SaaS, Marketo applique les bonnes pratiques du secteur SaaS

et remplacera les protocoles de sécurité actuellement utilisés (SHA-1 et SSL) par des versions plus sécurisées (SHA-2 (également appelées SHA-256) et TLS) pour les domaines suivants :

* marketo.net (trafic [!DNL Munchkin] chiffré)

* [marketo.com](https://marketo.com) (principales applications SaaS)

Cela se produira peu de temps après cette version. Le protocole SHA-1 sera temporairement pris en charge sur le domaine [mktoapi.com](https://mktoapi.com) jusqu&#39;en décembre 2015 pour permettre aux propriétaires de systèmes et d&#39;applications hérités de mettre à jour leurs systèmes avec la compatibilité SHA-2.

**[!DNL Munchkin]** sécurisé

Nous supprimons notre prise en charge de SSL3. Nous avons maintenu SSL3 jusqu’à présent pour maintenir la prise en charge des anciens navigateurs web, mais en 2015, nous ne voyons plus de trafic web important provenant de ces navigateurs. Cela n’affecte que les [!DNL Munchkin] lorsqu’elles sont utilisées sur des pages sécurisées et se déploie lentement après la version de février.

## Améliorations Du Personalization En Temps Réel {#real-time-personalization-enhancements}

**[URL cible pour les campagnes](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Sélectionnez les pages que votre campagne en temps réel doit afficher à l’aide de l’option Ajouter une URL Target . Cette fonctionnalité fonctionne avec tous les types de campagne (boîte de dialogue, dans la zone, widgets), mais elle est particulièrement utile pour les campagnes dans la zone, où une campagne s’affiche dans l’identifiant de zone pour l’URL cible sélectionnée uniquement. Elle prend en charge l’ajout de plusieurs URL pour cibler différentes pages web.

![](assets/image2015-2-19-11-3a0-3a30.png)

**Pays et état ajoutés au ciblage basé sur les comptes**

Les valeurs Pays et État peuvent désormais être ajoutées à vos Listes de comptes nommés. Cibler de futurs comptes clés à partir de lieux spécifiques.
