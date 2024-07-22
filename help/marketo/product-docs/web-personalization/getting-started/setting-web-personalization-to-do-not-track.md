---
unique-page-id: 11382593
description: Définition de Web Personalization sur lequel ne pas effectuer de suivi - Documents Marketo - Documentation du produit
title: Configuration de Web Personalization pour un suivi incorrect
exl-id: 9c60cd6b-4244-4472-90fa-4ba9fa9a4f34
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Configuration de Web Personalization pour un suivi incorrect {#setting-web-personalization-to-do-not-track}

Les visiteurs web peuvent configurer leur navigateur pour empêcher le suivi par n’importe quel site web, en choisissant &quot;Ne pas suivre&quot; (DNT). Cela empêche le suivi pour ce navigateur et cet appareil particulier.

Dans Personalization web et contenu prédictif, un marketeur peut définir une bascule pour indiquer s’il faut prendre en charge ou ignorer le paramètre Ne pas suivre (DNT) du navigateur. Le basculement pour les comptes est désactivé par défaut, ce qui signifie que le DNT n’est pas honoré par l’application.

## Activation ou désactivation du basculement {#enable-or-disable-the-toggle}

1. Accédez à **Paramètres du compte**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. Dans Configuration du domaine et du domaine, sélectionnez **On** pour activer le bouton d’activation/désactivation du DNT d’honneur.

   ![](assets/two-1.png)

   Lorsque le bouton bascule est activé, Web Personalization prend en charge le paramètre Ne pas suivre (DNT) du navigateur et ne suit aucune activité web ni n’exécute de campagnes ou de recommandations de contenu sur votre site web.

   >[!NOTE]
   >
   >La définition du bouton bascule sur Activé peut affecter la valeur et la fonctionnalité de Marketo dans des zones spécifiques.

1. Pour désactiver le bouton Honor DNT et ignorer le paramètre Do No Track (DNT) du navigateur, sélectionnez **Off** sous Honor DNT.
