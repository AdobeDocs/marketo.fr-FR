---
unique-page-id: 1147108
description: Importation d’un programme - Documents Marketo - Documentation du produit
title: Importation d’un programme
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Importation d’un programme {#import-a-program}

Un programme peut être importé d&#39;un abonnement Marketo vers un autre. Par exemple, vous pouvez créer un programme dans un environnement de test, puis l’importer dans votre abonnement en direct. En outre, vous pouvez importer un programme prédéfini à partir du [Bibliothèque de programmes Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

## Importation d’un programme {#importing-a-program}

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/import-a-program-1.png)

1. Cliquez sur le bouton **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Programme d’importation]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >L’importation de programme n’est disponible que pour les utilisateurs pour lesquels l’autorisation Importer un programme est activée. En savoir plus sur [gestion des rôles utilisateur et des autorisations](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >Pour connecter un compte sandbox à votre abonnement en direct, contactez [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Sélection d’une Marketo **[!UICONTROL Abonnement]** et un programme à importer. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-program-3.png)

1. Spécifiez un **[!UICONTROL Dossier Campaign]** pour le programme importé. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Assurez-vous de **[!UICONTROL Utiliser le conflit par défaut]** règles est sélectionnée. Des règles de conflit sont nécessaires lorsque vous importez des programmes dans une instance dont les ressources portent le même nom.

1. Sélectionnez les détails de conflit de votre choix, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Si vous importez un programme qui utilise des étapes de flux personnalisées ou des règles de liste dynamique dérivées d’un service d’étape de flux dans une instance de destination où il existe plusieurs fournisseurs de services compatibles, l’utilisateur importateur sera invité à affecter des étapes ou des règles au bon fournisseur dans l’instance de destination.

1. Aperçu des détails et **[!UICONTROL Importer]** le programme.

   ![](assets/import-a-program-6.png)

Une fois l&#39;import terminé, vous recevrez une confirmation par email.

>[!NOTE]
>
>Vous devrez replanifier les campagnes par lots importées et activer les campagnes de déclenchement. Le système désactive automatiquement les plannings de campagne et déclenche les campagnes dans le programme importé.

## Impact sur les ressources externes lors des importations de programme {#impact-on-external-assets-during-program-imports}

Les programmes utilisent des ressources externes telles que des modèles de courrier électronique, des modèles de page d’entrée, des images, des formulaires, des jetons et des balises de programme. Vous pouvez configurer la manière dont les modèles de page d’entrée et les balises de programme sont traités, et Marketo gère automatiquement le reste.

**Modèles de courrier électronique/page d’entrée :** Les modèles Email/Landing Page sont importés dans Design Studio. Vous pouvez utiliser des règles de conflit pour configurer le comportement lorsqu’il existe un modèle portant le même nom. Avec la règle par défaut, un nombre sera ajouté à un modèle s’il existe un modèle portant le même nom. Par exemple, si vous disposez déjà d’un modèle nommé &quot;Modèle standard&quot;, le nouveau modèle s’intitule &quot;Modèle standard - 1&quot;.

**Pages d’entrée/Forms :** S’il existe un formulaire ou une page d’entrée portant le même nom dans Design Studio, ils seront toujours importés, mais un numéro sera ajouté à leur nom (ex : Page d’entrée - 1).

**Images :** Les images utilisées par les landing pages sont importées dans l’atelier de conception, sauf si elles portent le même nom.

**Jetons :** Les jetons qui se trouvent en dehors d’un programme sont convertis en jetons locaux lors du processus d’importation.

>[!CAUTION]
>
>Le type d’image que mes jetons ne sont pas pris en charge pour les importations de programme. Si un programme de type image mes jetons est importé, _non_ les jetons passeront.

**Balises de programme :** Vous pouvez utiliser des règles de conflit pour contrôler la manière dont les balises de programme qui n’existent pas dans le compte de destination seront traitées. L’utilisation de la règle par défaut crée les balises de programme ou vous pouvez choisir d’ignorer les balises.

>[!CAUTION]
>
>Lors de l&#39;import d&#39;un programme, les emails/landing pages contenant [contenu dynamique](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} sera ignorée.
