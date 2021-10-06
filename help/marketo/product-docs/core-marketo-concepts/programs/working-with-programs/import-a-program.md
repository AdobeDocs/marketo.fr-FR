---
unique-page-id: 1147108
description: Importation d’un programme - Documents Marketo - Documentation du produit
title: Importation d’un programme
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
source-git-commit: 1b37a750c5e609b9e43e942df752305d85153989
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Importation d’un programme {#import-a-program}

Un programme peut être importé d&#39;un abonnement Marketo vers un autre. Par exemple, vous pouvez créer un programme dans un environnement de test, puis l’importer dans votre abonnement en direct. Vous pouvez également importer un programme prédéfini à partir de la bibliothèque de programmes Marketo.

## Importation d’un programme {#import-a-program-1}

1. Accédez à **Activités marketing.**

   ![](assets/ma.png)

1. Cliquez sur la liste déroulante **Nouvelle** . Sélectionnez **Programme d’importation**.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >L’importation de programme n’est disponible que pour les utilisateurs pour lesquels l’autorisation Importer un programme est activée. En savoir plus sur la [gestion des rôles et des autorisations des utilisateurs](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Pour connecter un compte sandbox à votre abonnement en direct, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Sélectionnez une Marketo **Abonnement** et un programme à importer. Cliquez sur **Suivant**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Spécifiez un **dossier Campaign** pour le programme importé. Cliquez sur **Suivant.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Assurez-vous que les **règles Utiliser le conflit par défaut** sont sélectionnées. Des règles de conflit sont nécessaires lorsque vous importez des programmes dans une instance dont les ressources portent le même nom.

1. Prévisualisez les détails et **importez** le programme.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   Une boîte de dialogue affiche la progression de l’importation du programme.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Une fois l&#39;import terminé, vous recevrez une confirmation par email.

>[!NOTE]
>
>Vous devrez replanifier les campagnes par lots importées et activer les campagnes de déclenchement. Le système désactive automatiquement les plannings de campagne et déclenche les campagnes dans le programme importé.

## Identification des programmes prédéveloppés dans la bibliothèque de programmes Marketo {#identify-pre-built-programs-in-the-marketo-program-library}

La bibliothèque de programmes Marketo contient des programmes prédéfinis et testés que vous pouvez importer dans votre abonnement. Les programmes disponibles incluent :

1. **Des soins de base.** Envoie une série d’emails séparés par des étapes d’attente.
1. **Gestion des données.** Maintient l’intégrité des données à l’aide de campagnes intelligentes.
1. **Courrier électronique avec page d’entrée.** Envoie un premier courrier électronique avec une offre, par exemple &quot;Téléchargez ce livre blanc&quot;. Suit un email de confirmation ou de rappel. Inclut une landing page avec un formulaire.
1. **Courrier électronique avec états de progression.** Envoie un message avec un lien pouvant faire l’objet d’un suivi que la personne à cliquer. Met à jour l’état de progression de chaque personne (Envoyé, Ouvert, Cliqué, etc.).
1. **Moments significatifs.** Crée des moments intéressants pour que votre équipe de vente les conserve dans la boucle.
1. **Page d’entrée avec la réponse automatique.** Utilisez du contenu téléchargeable pour obtenir de nouvelles personnes et les nourrir. Inclut des landing pages et des formulaires.
1. **Cycle de vie 2.** Utilise la notation pour faire passer une personne du nouveau au marketing qualifié.
1. **Modèle de courrier électronique mobile.** Modèle de courrier électronique réactif testé par rapport à iPhone et Android. Certaines versions d’Android, MS Outlook, Exchange et d’applications tierces telles que Gmail et Yahoo! Les applications mobiles de messagerie ne prennent pas en charge le code CSS requis pour les modèles réactifs. Nous vous recommandons de tester avant d’envoyer des emails.
1. **Tirage d’importation de programme.** Programme Tirage pour ceux qui essaient la bibliothèque du programme ! Validez simplement les emails et la landing page et activez la campagne dynamique. Visualisez ensuite la landing page validée, remplissez le formulaire, et vous êtes alors inscrit !
1. **Campagnes disponibles des ventes.** Donne à vos commerciaux le moyen d’exécuter des campagnes dynamiques Marketo à partir d’un tableau de bord dans votre gestion de la relation client.
1. **Notation - Édition Spark.** Score démographique et comportemental capturé dans un champ de notation unique. Inclut plus de deux douzaines de campagnes liées à la notation.
1. **Notation - Éditions Standard et Sélectionner .** Score démographique et comportemental capturé dans des champs de notation distincts. Inclut plus de deux douzaines de campagnes liées à la notation.
1. **Synchroniser les nouvelles personnes avec le CRM.** La campagne qui synchronise les nouvelles personnes dans votre système CRM. Il attribue un statut de personne de sorte qu’il soit reconnu comme n’étant pas prêt pour les ventes.
1. **Webinaire avec adaptateur d’événement.** Un ensemble complet d’emails (ex. : invitations et rappels) ainsi que des landing pages avec des formulaires et des campagnes pour déplacer des personnes dans le programme. Ce programme reçoit des mises à jour sur l&#39;inscription, l&#39;assiduité, etc. des fournisseurs d’événements en ligne tels que WebEx.
1. **Webinaire sans adaptateur d’événement.** Comme ci-dessus, mais avec des processus manuels d&#39;enregistrement, de présence, etc.
1. **Programme de notation des décisions Sirius**. Ce programme est conçu pour prendre en charge le modèle de notation standard des décisions Sirius, y compris les règles de notation implicites et explicites et l’affectation de personne matrifiée.

>[!CAUTION]
>
>Vous devez créer deux champs personnalisés (&quot;Score démographique&quot; et &quot;Score comportemental&quot;) avant d’importer le programme Scoring - Standard &amp; Select Editions .

## Impact sur les ressources externes lors des importations de programme {#impact-on-external-assets-during-program-imports}

Les programmes utilisent des ressources externes telles que des modèles d’email, des modèles de landing page, des images, des formulaires, des jetons et des balises de programme. Vous pouvez configurer la manière dont les modèles de landing page et les balises de programme sont traités, et Marketo gère automatiquement le reste.

**Modèles de courrier électronique :** les modèles de courrier électronique sont automatiquement importés et créés, sauf s’il en existe un portant le même nom.

**Modèles de page d’entrée :** les modèles de page d’entrée sont importés dans le studio de conception. Vous pouvez utiliser des règles de conflit pour configurer le comportement lorsqu’il existe un modèle portant le même nom. En utilisant la règle par défaut, un nombre sera ajouté à un modèle de landing page s&#39;il en existe un portant le même nom. Par exemple, un modèle de page d’entrée nommé Modèle standard 1 sera créé s’il existe un modèle standard.

**Images :**  les images utilisées par les landing pages sont importées dans l’atelier de conception, sauf si elles portent le même nom.

**Jetons :** les jetons situés en dehors d’un programme seront convertis en jetons locaux au cours du processus d’importation.

>[!CAUTION]
>
>Le type d’image que mes jetons ne sont pas pris en charge pour les importations de programme. Si un programme avec un type d’image mes jetons est importé, les jetons **no** passeront.

**Balises de programme :** vous pouvez utiliser des règles de conflit pour contrôler la manière dont seront traitées les balises de programme qui n’existent pas dans le compte de destination. L’utilisation de la règle par défaut crée les balises de programme ou vous pouvez choisir d’ignorer les balises.

**Forms :** les formulaires externes seront automatiquement importés dans l’atelier de conception, sauf s’il en existe un portant le même nom.

>[!CAUTION]
>
>Lors de l&#39;import d&#39;un programme, les landing pages/emails contenant [contenu dynamique](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) seront ignorés.
