---
unique-page-id: 1147108
description: Importer un Programme - Documents marketing - Documentation du produit
title: Importer un Programme
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---


# Importer un Programme {#import-a-program}

Un programme peut être importé d&#39;un abonnement de marché à un autre. Par exemple, vous pouvez créer un programme dans un sandbox, puis l’importer dans votre abonnement actif. En outre, vous pouvez importer un programme préconstruit à partir de la bibliothèque de Programmes Marketo.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Importer un Programme {#import-a-program-1}

1. Accédez à Activités **marketing.**

   ![](assets/ma.png)

1. Cliquez sur **Nouvelle **liste déroulante. Sélectionnez **Importer le Programme**.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >L’importation de programme n’est disponible que pour les utilisateurs pour lesquels l’autorisation d’importation de Programme est activée. En savoir plus sur la [gestion des rôles utilisateur et des autorisations](../../../../product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >
   >Pour connecter un compte sandbox à votre abonnement actif, contactez l’assistance [](http://www.marketo.com/services/support/)marketing.

1. Sélectionnez un **Abonnement** marketing et un programme à importer. Cliquez sur **Suivant**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Spécifiez un dossier **** Campaign pour le programme importé. Cliquez sur **Suivant.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Assurez-vous que** ****Utiliser les règles de conflit** par défaut est sélectionné. Des règles de conflit sont nécessaires lorsque vous importez des programmes dans une instance dont les actifs portent le même nom.

1. Détails de la prévisualisation et **Importer** le programme.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   Une boîte de dialogue affiche la progression de l&#39;importation du programme.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Vous recevrez une confirmation par courrier électronique une fois l&#39;importation terminée.

>[!NOTE]
>
>Vous devez replanifier des campagnes par lots importées et activer des campagnes de déclenchement. Le système désactive automatiquement les planifications de campagne et déclenche les campagnes dans le programme importé.

## Identification des Programmes prédéveloppés dans la bibliothèque de Programmes de marketing {#identify-pre-built-programs-in-the-marketo-program-library}

La bibliothèque de Programmes Marketo contient des programmes pré-créés et testés que vous pouvez importer dans votre abonnement. Les programmes disponibles sont les suivants :

1. **Infirmière de base.** Envoie une série de courriers électroniques séparés par des étapes d’attente.
1. **data Management.** Préserve l’intégrité des données à l’aide de campagnes intelligentes.
1. **Courriel avec Landing page.** Envoie un premier courrier électronique avec une offre, telle que &quot;Télécharger ce livre blanc&quot;. Suit un message de confirmation ou de rappel. Inclut un landing page avec un formulaire.
1. **Courrier électronique avec états de progression.** Envoie une explosion de courrier avec un lien pouvant faire l’objet d’un suivi pour la personne sur laquelle cliquer. Met à jour l’état de progression de chaque personne - Envoyé, Ouvert, Cliqué, etc.
1. **Moments intéressants.** Crée des moments intéressants pour que votre équipe commerciale les garde dans la boucle.
1. **landing page avec la réponse automatique.** Utilisez le contenu téléchargeable pour attirer de nouvelles personnes et les nourrir. Inclut des landings page et des formulaires.
1. **Cycle de vie 2.** Utilise le score pour déplacer une personne du nouveau au marketing qualifié.
1. **Modèle de courrier électronique mobile.** Modèle de courrier électronique réactif testé sur iPhone et Android. Certaines versions des applications Android, MS Outlook, Exchange et tierces, telles que Gmail et Yahoo ! Les applications mobiles par courrier électronique ne prennent pas en charge la page CSS requise pour les modèles réactifs. Nous vous recommandons de tester avant d&#39;envoyer des courriers électroniques.
1. **Tirage d’importation de programme.** Tirage programme pour ceux qui essaient la Programme Library ! Approuvez simplement les courriels et le landing page et activez la campagne intelligente. Ensuite, vue le landing page approuvé, remplissez le formulaire, et vous êtes inscrit !
1. **Campagnes disponibles sur les ventes.** Donne à vos commerciaux un moyen d’exécuter des campagnes marketing intelligentes à partir d’un Tableau de bord de votre gestion de la relation client.
1. **Scoring - Spark Edition.** Score démographique et comportemental capturé dans un seul champ de score. Inclut plus de deux douzaines de campagnes liées au score.
1. **Scoring - Standard &amp; Select Editions.** Score démographique et comportemental capturé dans des champs de score distincts. Inclut plus de deux douzaines de campagnes liées au score.
1. **Synchroniser les nouvelles personnes avec CRM.** Campagne qui synchronise les nouvelles personnes sur votre système de gestion de la relation client. Il attribue un statut à une personne de telle sorte qu&#39;elle soit reconnue comme n&#39;étant pas prête pour les ventes.
1. **Webinaire avec adaptateur de Événement.** Un ensemble complet de courriels - tels que des invitations et des rappels - plus des landings page avec des formulaires et des campagnes pour déplacer les personnes à travers le programme. Ce programme reçoit des mises à jour sur l&#39;inscription, la présence, etc. provenant de fournisseurs de événements en ligne tels que WebEx.
1. **Webinaire sans adaptateur de Événement.** Comme ci-dessus, mais avec des processus manuels pour enregistrer l&#39;inscription, la présence, etc.
1. **Programme** de score des décisions Sirius. Ce programme est conçu pour prendre en charge le modèle standard de notation des décisions Sirius, y compris les règles de notation implicites et explicites et l&#39;affectation de personnes matriquées. Vue [de ce](http://docs.marketo.com/display/docs/assets/sirius-decisions-scoring-program-overview.pdf)PDF pour plus d’informations.

>[!CAUTION]
>
>Vous devez créer deux champs personnalisés (&quot;Score démographique&quot; et &quot;Score comportemental&quot;) avant d’importer le programme Scoring - Standard &amp; Select Editions.

## Impact sur les actifs externes lors des importations de Programme {#impact-on-external-assets-during-program-imports}

Les programmes utilisent des ressources externes telles que des modèles de courrier électronique, des modèles de landing page, des images, des formulaires, des jetons et des balises de programme. Vous pouvez configurer la manière dont les modèles de landing page et les balises de programme sont traités et Marketo gère automatiquement le reste.

**Modèles de courrier électronique : **Les modèles de courrier électronique sont automatiquement importés et créés, sauf s’il en existe un portant le même nom.

**Modèles de Landing page : **Les modèles de Landing page sont importés dans le studio de création. Vous pouvez utiliser des règles de conflit pour configurer le comportement lorsqu’un modèle portant le même nom existe. La règle par défaut permet d’ajouter un nombre à un modèle de landing page s’il en existe un portant le même nom. Par exemple, un modèle de landing page nommé Modèle standard 1 est créé s’il en existe un nommé Modèle standard.

**Images : **Les images utilisées par les landings page sont importées dans le studio de création, sauf si elles portent le même nom.

**Jetons : **Les jetons qui résident en dehors d’un programme seront convertis en jetons locaux pendant le processus d’importation.

>[!CAUTION]
>
>Les types d’image que mes jetons ne sont pas pris en charge pour les importations de programme. Si un programme avec un type d&#39;image mes jetons est importé, **no **tokens va passer.

**Balises de Programme : **Vous pouvez utiliser des règles de conflit pour contrôler le traitement des balises de programme qui n’existent pas dans le compte de destination. L’utilisation de la règle par défaut crée les balises de programme ou vous pouvez choisir d’ignorer les balises.  **Forms : **Les formulaires externes seront automatiquement importés dans le studio de création, sauf s’il en existe un portant le même nom.

>[!CAUTION]
>
>Lors de l’importation d’un programme, les landings page/courriers électroniques contenant du contenu [](http://docs.marketo.com/x/yRAt) dynamique sont ignorés.

## Regarder une vidéo {#watch-a-video}

`<iframe width="630" height="470" src="//play.vidyard.com/KgvZssZ9WRkZgDsY1yZfms.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`