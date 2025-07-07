---
solution: Marketo Engage
product: marketo
title: TITLE
description: Découvrez comment créer et gérer vos directives de marque.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: e0e739054c6389e0a3ab638097491e6c24f5e30c
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 87%

---

# Créer et gérer vos marques {#brands}

>[!AVAILABILITY]
>
>Vous devez accepter le [contrat d’utilisation](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} avant de pouvoir utiliser l’assistant AI dans Adobe Marketo Engage. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

Les consignes de marque sont un ensemble détaillé de règles et de normes qui établissent l’identité visuelle et verbale d’une marque. Elles servent de référence pour maintenir une représentation cohérente de la marque sur toutes les plateformes de marketing et de communication.

Dans [!DNL Marketo Engage], vous avez désormais la possibilité de saisir et d’organiser manuellement les détails de votre marque ou de charger des documents de directives pour une extraction automatique des informations.

## Accéder aux marques {#generative-access}

Pour accéder au menu **[!UICONTROL Marques]** dans [!DNL Adobe Marketo Engage], vous devez disposer des autorisations **[!UICONTROL Gérer le kit de marque]** ou **[!UICONTROL Activer l’Assistant IA]**. LIEN EN SAVOIR PLUS

+++  Découvrez comment attribuer des autorisations liées à la marque.

Pour attribuer des autorisations aux marques, procédez comme suit :

1. Dans le produit **Autorisations**, accédez à l’onglet **Rôles** et sélectionnez le **Rôle** de votre choix.

1. Cliquez sur **Modifier** pour modifier les autorisations.

1. Ajoutez la ressource **Assistant IA**, puis sélectionnez **Gérer le kit de marque** ou **[!UICONTROL Activer l’Assistant IA]** dans le menu déroulant.

   Notez que l’autorisation **[!UICONTROL Activer l’Assistant IA]** permet uniquement d’accéder en lecture seule au menu **[!UICONTROL Marques]**.

   CAPTURE D’ÉCRAN

1. Cliquez sur **Enregistrer** pour appliquer vos modifications.

   Les autorisations des personnes déjà affectées à ce rôle seront automatiquement mises à jour.

1. Pour attribuer ce rôle à de nouvelles personnes, accédez à l’onglet **Utilisateurs et utilisatrices** du tableau de bord **Rôles** et cliquez sur **Ajouter un utilisateur ou une utilisatrice**.

1. Saisissez le nom de la personne, son adresse e-mail ou choisissez dans la liste, puis cliquez sur **Enregistrer**.

1. Si le profil de l’utilisateur ou de l’utilisatrice n’a pas été créé auparavant, consultez cette [documentation](https://experienceleague.adobe.com/fr/docs/experience-platform/access-control/abac/permissions-ui/users).

+++

## Créer et gérer votre marque {#create-brand-kit}

Pour créer et gérer vos directives de marque, vous pouvez saisir vous-même les détails ou charger votre document de directives de marque pour que les informations soient extraites automatiquement :

1. Dans le menu **[!UICONTROL Marques]**, cliquez sur **[!UICONTROL Créer une marque]**.

   CAPTURE D’ÉCRAN

1. Saisissez le **[!UICONTROL Nom]** de votre marque.

1. Effectuez un glisser-déposer ou sélectionnez votre fichier pour charger vos directives de marque et extraire automatiquement les informations pertinentes sur la marque. Cliquez sur **[!UICONTROL Créer une marque]**.

   Le processus d’extraction des informations commence maintenant. Notez que l’opération peut prendre plusieurs minutes.

   CAPTURE D’ÉCRAN

1. Vos standards de création visuelle et de contenu sont désormais automatiquement renseignés. Parcourez les différents onglets pour adapter les informations selon vos besoins. [En savoir plus](#personalize)

1. Dans le menu avancé de chaque section ou catégorie, vous pouvez ajouter des références pour extraire automatiquement les informations de marque pertinentes.

   Pour supprimer du contenu existant, utilisez les options **[!UICONTROL Effacer la section]** ou **[!UICONTROL Effacer la catégorie]**.

   CAPTURE D’ÉCRAN

1. Une fois la configuration effectuée, cliquez sur **[!UICONTROL Enregistrer]**, puis sur **[!UICONTROL Publier]** pour rendre les consignes de votre marque disponibles dans l’Assistant IA.

1. Pour apporter des modifications à votre marque publiée, cliquez sur **[!UICONTROL Modifier la marque]**.

   >[!NOTE]
   >
   >Cette opération crée une copie temporaire en mode d’édition, qui remplace la version active une fois publiée.

   CAPTURE D’ÉCRAN

1. Dans le tableau de bord **[!UICONTROL Marques]**, ouvrez le menu avancé en cliquant sur l’icône VIDE pour :

   * Afficher la marque
   * Modifier
   * Dupliquer
   * Publier
   * Dépublier
   * Supprimer

   CAPTURE D’ÉCRAN

Les consignes de votre marque sont désormais accessibles à partir de la liste déroulante **[!UICONTROL Marque]** du menu de l’Assistant IA, ce qui lui permet de générer du contenu et des ressources dans le ton de votre marque. En savoir plus sur l’assistant AI - LINK

CAPTURE D’ÉCRAN

### Définir une marque par défaut {#default-brand}

Vous pouvez désigner une marque par défaut qui sera appliquée automatiquement lors de la génération du contenu et du calcul des scores d’alignement pendant la création des campagnes.

Pour définir une marque par défaut, accédez au tableau de bord **[!UICONTROL Marques]**. Ouvrez le menu avancé en cliquant sur l’icône ![](assets/do-not-localize/Smock_More_18_N.svg) et sélectionnez **[!UICONTROL Marquer comme marque par défaut]**.

CAPTURE D’ÉCRAN

## Personnaliser votre marque {#personalize}

### À propos de la marque {#about-brand}

Dans l’onglet **[!UICONTROL À propos de la marque]**, vous pouvez définir l’identité principale de votre marque en décrivant son objectif, sa personnalité, son slogan et d’autres attributs déterminants.

1. Commencez par renseigner les informations de base de votre marque dans la catégorie **[!UICONTROL Détails clés]** :

   * **[!UICONTROL Nom du kit de marque]** : saisissez le nom du kit de marque.

   * **[!UICONTROL Quand l’utiliser]** : spécifiez les scénarios ou les contextes dans lesquels ce kit de marque doit être appliqué.

   * **[!UICONTROL Nom de la marque]** : saisissez le nom officiel de la marque.

   * **[!UICONTROL Description de la marque]** : présentez ce que représente cette marque.

   * **[!UICONTROL Slogan par défaut]** : ajoutez le slogan principal de la marque.

   CAPTURE D’ÉCRAN

1. Dans la catégorie **[!UICONTROL Principes directeurs]**, clarifiez l’orientation principale et la philosophie de votre marque :

   * **[!UICONTROL Mission]** : détaillez l’objectif de votre marque.

   * **[!UICONTROL Vision]** : décrivez votre objectif à long terme ou la situation future visée.

   * **[!UICONTROL Positionnement sur le marché]** : expliquez comment votre marque se positionne sur le marché.

   CAPTURE D’ÉCRAN

1. Dans la catégorie **[!UICONTROL Valeurs de marque principales]**, cliquez sur « Ajouter une icône » pour ajouter les valeurs de base de la marque et renseigner les détails :

   * **[!UICONTROL Valeur]** : attribuez un nom à une valeur fondamentale de la marque.

   * **[!UICONTROL Description]** : expliquez ce que cette valeur signifie pour votre marque.

   * **[!UICONTROL Comportements]** : décrivez les actions ou attitudes qui reflètent cette valeur dans la pratique.

   * **[!UICONTROL Manifestations]** : donnez des exemples de la manière dont cette valeur s’exprime dans le branding réel.

   CAPTURE D’ÉCRAN

1. Si nécessaire, cliquez sur l’icône « Modifier » pour mettre à jour ou supprimer l’une des valeurs principales de votre marque.

   CAPTURE D’ÉCRAN

Vous pouvez maintenant [publier votre marque](#create-brand-kit) ou continuer à la personnaliser.

### Règle de style {#writing-style}

La section **[!UICONTROL Style d’écriture]** décrit les normes d’écriture du contenu et expose en détail comment la langue, la mise en forme et la structure doivent être utilisés pour garantir la clarté, la cohérence et l’homogénéité de l’ensemble des ressources.

+++ Catégories et exemples disponibles

<table>
  <thead>
    <tr>
      <th>Catégorie</th>
      <th>Sous-catégorie</th>
      <th>Exemple de directives</th>
      <th>Exemple d’exclusions</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Normes de création de contenu</td>
      <td>Normes des messages de la marque</td>
      <td>Mettez l’accent sur l’innovation et orientez les messages sur la clientèle.</td>
      <td>Ne faites pas de promesses irréalistes sur les capacités du produit.</td>
    </tr>
    <tr>
      <td>Utilisation du slogan</td>
      <td>Placez le slogan sous le logo sur toutes les ressources marketing numériques.</td>
      <td>Ne modifiez ni ne traduisez le slogan.</td>
    </tr>
    <tr>
      <td>Messages principaux</td>
      <td>Insistez sur l’énoncé des principaux avantages, comme l’amélioration de la productivité.</td>
      <td>N’utilisez pas des propositions de valeur sans rapport.</td>
    </tr>
    <tr>
      <td>Normes de nommage</td>
      <td>Utilisez des noms simples et descriptifs tels que « ProScheduler ».</td>
      <td>N’utilisez ni des termes complexes ni des caractères spéciaux.</td>
    </tr>
    <tr>
      <td rowspan="5">Style de communication de la marque</td>
      <td>Caractéristiques de la marque</td>
      <td>Amical et accessible.</td>
      <td>Ne soyez pas défaitiste.</td>
    </tr>
    <tr>
      <td>Règles d’écriture</td>
      <td>Gardez les phrases courtes et percutantes.</td>
      <td>N’utilisez pas trop de jargon.</td>
    </tr>
    <tr>
      <td>Ton situationnel</td>
      <td>Maintenez un ton professionnel dans les communications de crise.</td>
      <td>Ne soyez pas dédaigneux dans les communications d’assistance.</td>
    </tr>
    <tr>
      <td>Consignes relatives aux choix des mots</td>
      <td>Utilisez des mots comme « innovant » et « intelligent ».</td>
      <td>Évitez les mots tels que « bon marché » ou « hack ».</td>
    </tr>
    <tr>
      <td>Normes linguistiques</td>
      <td>Respectez les conventions françaises.</td>
      <td>Faites attention à l’orthographe.</td>
    </tr>
    <tr>
      <td rowspan="3">Normes de conformité légale</td>
      <td>Normes de marque commerciale</td>
      <td>Utilisez toujours le symbole ™ ou ®.</td>
      <td>N’omettez pas les symboles légaux si nécessaire.</td>
    </tr>
    <tr>
      <td>Normes de copyright</td>
      <td>Incluez les avis de copyright sur les supports marketing.</td>
      <td>N’utilisez pas de contenu tiers sans autorisation.</td>
    </tr>
    <tr>
      <td>Normes de mentions légales</td>
      <td>Affichez clairement les mentions légales sur les ressources numériques.</td>
      <td>Ne masquez pas les mentions légales dans des zones non visibles.</td>
    </tr>
</table>

+++

</br>

Pour personnaliser votre **[!UICONTROL style d’écriture]** :

1. Dans l’onglet **[!UICONTROL Style d’écriture]**, cliquez sur ![](assets/do-not-localize/Smock_Add_18_N.svg) pour ajouter une directive, une exception ou une exclusion.

1. Saisissez votre directive, votre exception ou votre exclusion, puis cliquez sur **[!UICONTROL Ajouter]**.

   CAPTURE D’ÉCRAN

1. Sélectionnez l’une des directives ou exclusions à mettre à jour ou à supprimer.

1. Cliquez sur le bouton « Modifier » pour modifier votre exemple ou sur l’icône « Supprimer » pour le supprimer.

   CAPTURE D’ÉCRAN

Vous pouvez désormais personnaliser davantage votre marque ou [la publier](#create-brand-kit).

### Contenu visuel {#visual-content}

La section **[!UICONTROL Contenu visuel]** définit les normes en matière d’imagerie et de conception, en détaillant les spécifications nécessaires pour conserver une apparence de marque unifiée et cohérente.

+++ Catégories et exemples disponibles

<table>
  <thead>
    <tr>
      <th>Catégorie</th>
      <th>Exemple de directives</th>
      <th>Exemple d’exclusions</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Normes de photographie</td>
      <td>Utilisez l’éclairage naturel pour les prises de vue extérieures.</td>
      <td>Évitez les images trop modifiées ou pixellisées.</td>
    </tr>
    <tr>
      <td>Normes d’illustration</td>
      <td>Utilisez des styles épurés et minimalistes.</td>
      <td>Optez pour la simplicité.</td>
    </tr>
    <tr>
      <td>Normes d’icône</td>
      <td>Utilisez un système de grille cohérent de 24 px.</td>
      <td>Ne mélangez pas les dimensions des icônes, n’utilisez pas d’épaisseurs de trait incohérentes et ne vous écartez pas des règles de grille.</td>
    </tr>
    <tr>
      <td>Consignes d’utilisation</td>
      <td>Choisissez des images de style de vie qui représentent des clientes et clients réels utilisant le produit dans des environnements professionnels.</td>
      <td>N’utilisez pas d’images qui contredisent le ton de la marque ou semblent hors contexte.</td>
    </tr>
</table>

+++

</br>

Pour personnaliser votre **[!UICONTROL contenu visuel]** :

1. Dans l’onglet **[!UICONTROL Contenu visuel]**, cliquez sur VIERGE pour ajouter une directive, une exclusion ou un exemple.

1. Saisissez votre directive, exclusion ou exemple et cliquez sur **[!UICONTROL Ajouter]**.

   CAPTURE D’ÉCRAN

1. Pour ajouter une image attestant d’une utilisation correcte, sélectionnez **[!UICONTROL Exemple]** et cliquez sur **[!UICONTROL Sélectionner une image]**. Vous pouvez également ajouter une image montrant une utilisation incorrecte comme exemple d’exclusion.

   CAPTURE D’ÉCRAN

1. Sélectionnez l’une des directives ou exclusions à mettre à jour ou à supprimer.

1. Sélectionnez l’une de vos directives ou exclusions pour la mettre à jour. Cliquez sur l’icône « Supprimer » pour la supprimer.

   CAPTURE D’ÉCRAN

Vous pouvez maintenant [publier votre marque](#create-brand-kit) ou continuer à la personnaliser.
