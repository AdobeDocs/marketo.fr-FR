---
unique-page-id: 37355534
description: Notes de mise à jour - Jan 2020 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Jan 2020
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 1%

---

# Notes de mise à jour : janvier 2020 {#release-notes-jan}

Les fonctionnalités suivantes sont incluses dans la version du 20 janvier. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile ( ![(star)](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **17 janvier 2020**.

## Adobe Marketo Engage principal {#core-marketo-engage-adobe-application}

* [Sélecteur de ressources Adobe Experience Manager](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md) : accédez rapidement aux ressources qui correspondent à votre marque avec les ressources AEM disponibles directement dans Marketo Engage. Remarque : Bien que cette fonctionnalité soit disponible dans nos expériences Marketo Sky et classique, les fonctionnalités d’administration se trouvent dans notre expérience classique. Vous devez être client d’AEM Assets et disposer de la version 6.5 ou supérieure.

>[!NOTE]
>
>Actuellement, le sélecteur de ressources AEM n’est entièrement pris en charge que dans Firefox. Elle n’est pas prise en charge dans Safari et peut ne pas fonctionner dans la dernière version de Chrome (v. 80), selon vos paramètres de cookie SameSite.

* **Microsoft Dynamics - piste de synchronisation vers CRM en temps réel** : synchronisation en temps réel des pistes et des contacts entre Marketo Engage et Microsoft Dynamics. Créez des pistes ou des contacts et affichez-les immédiatement dans Microsoft Dynamics avec l’action de flux &quot;Synchroniser la personne avec Microsoft&quot;.
* **Mappage de champ supplémentaire de LinkedIn Lead Gen Forms** : capture des données de piste de LinkedIn Lead Gen Forms afin de créer des expériences plus pertinentes pour les points de contact marketing et de vente. Extrayez les champs masqués, les champs de consentement et le champ de piste de test dans Marketo Engage.
* **API Dépendances des modèles d’email** : obtenir une liste des ressources qui dépendent d’un modèle d’email pour comprendre la portée des modifications potentielles et résoudre plus rapidement les dépendances des modèles qui peuvent être modifiées et supprimées.
* **Améliorations de la gestion multi-instances** : accédez à l’instance dont vous avez besoin rapidement à l’aide d’un menu déroulant alphabétique et défilable de vos abonnements.

## Account-Based Marketing {#account-based-marketing}

![(star)](assets/yellow-star.png)

* **[New Account Discovery (BETA)](https://docs.marketo.com/x/WQA6Ag) ![(star)](assets/yellow-star.png)** : utilisez le profilage de compte pour découvrir de nouveaux comptes cibles pour votre stratégie ABM en fonction de votre modèle de profil client idéal optimisé par l’IA. Affichez, sélectionnez et importez les nouveaux comptes recommandés, ainsi que leurs indicateurs de données d’ajustement et d’intention basés sur l’IA, qui n’existent pas déjà dans votre base de données de piste et de compte de Marketo Engage pour le ciblage ABM. Immédiatement disponible pour les clients de profilage de compte admissibles.

<br> 

**_Mise à jour tout au long du trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Bizible {#bizible}

![(star)](assets/yellow-star.png)

* **Intégration des pistes de Marketo Engage** : rassemblez les ventes et le marketing avec une vue unifiée des pistes sur Bizible et Marketo Engage. Grâce à cette mise à jour, Marketo Engage peut désormais être utilisé comme source de données de piste supplémentaire. Il n’est donc plus nécessaire d’attendre que les pistes soient synchronisées avec le CRM pour générer des rapports sur la génération de pistes.
* **Améliorations de Discover** : tirez davantage parti de nos panoramas Discover dans Bizible grâce aux améliorations apportées aux commentaires des clients, telles que la possibilité d’accéder aux enregistrements transactionnels à partir de mosaïques et d’attributs, d’ajouter des nombres d’enregistrements essentiels et les mesures de coût correspondantes, et d’ajouter/supprimer des filtres de tableau de bord pour plusieurs tableaux de bord. Vous accédez également directement au tableau de bord par défaut à la connexion.

## Marketo Sky {#marketo-sky}

* [Modification d’images](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio) : accédez aux fonctionnalités d’édition de l’Adobe sans avoir à quitter Marketo Engage. Cette nouvelle fonctionnalité vous permet d’améliorer, de recadrer et d’ajouter facilement du texte aux images directement dans Design Studio.

## Sales Insight {#sales-insight}

* **Actions en masse d’éclairs Salesforce** : améliorez l’efficacité des ventes et maintenez les acheteurs impliqués dans la possibilité d’ajouter jusqu’à 200 contacts/prospects aux campagnes et de leur envoyer des emails Marketo Engage en masse avec Salesforce Lightning.
* **Prise en charge mobile de Salesforce1** : vous disposez désormais d’un accès mobile en continu à toutes les fonctionnalités d’aperçu des ventes, comme Moments intéressants et Activités web et e-mails, directement dans l’application Salesforce1.
* **Améliorations de l’interface utilisateur** : mise à jour de l’interface avec des améliorations de la lisibilité et une conception cohérente avec notre expérience de Marketo Sky.

## Sales Connect {#sales-connect}

* **Composants de grille** : optimisez votre instance Sales Connect avec de nouvelles fonctionnalités de personnalisation de grille. Choisissez les colonnes à afficher, recherchez des colonnes, sélectionnez/désélectionnez toutes les colonnes et déterminez le nombre de lignes de données à afficher sur chaque page.
* **[Verrouillage de contenu](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)** : optimise l’alignement de la marque avec un paramètre à l’échelle de l’abonnement qui contrôle si les non-administrateurs ont la possibilité de créer et de modifier des modèles et des campagnes.

>[!NOTE]
>
>* **Dépréciation de TLS 1.0 et 1.1** : dans un effort continu d’intégration à la structure de version d’Adobe, nous transférons l’obsolescence de TLS 1.0 et TLS 1.1 au 13 janvier 2020. Vous trouverez de plus amples informations [ici](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **Mise à jour ITP 2.1+ Munchkin** : en raison de modifications apportées à la politique des cookies pour Safari, la capacité de Munchkin à effectuer le suivi des utilisateurs entre les sessions sur le même domaine sera limitée par ITP à 1 ou 7 jours en fonction de la version du navigateur et de la version du navigateur utilisée par le visiteur. Pour ce faire, nous mettons en oeuvre un nouveau service Web pour permettre aux cookies Munchkin d’être définis avec un en-tête Set-Cookie via une réponse HTTP. Vous trouverez plus d&#39;informations sur la mise en oeuvre de ce nouveau service [ici](https://nation.marketo.com/docs/DOC-7351).

**__** [Rejoignez-nous](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) le 3 mars à 11h00 PT/14 h ET pour un webinaire en direct hébergé par notre équipe produit et découvrez les fonctionnalités incluses dans cette version.
