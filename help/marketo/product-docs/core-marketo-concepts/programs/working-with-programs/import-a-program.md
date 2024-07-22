---
unique-page-id: 1147108
description: Importation d’un programme - Documents Marketo - Documentation du produit
title: Importation d’un programme
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 0adb780ea1622d12b8daafc502fd6a9151757ad3
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Importation d’un programme {#import-a-program}

Un programme peut être importé d&#39;un abonnement Marketo Engage à un autre. Par exemple, vous pouvez créer un programme dans un environnement de test, puis l’importer dans votre abonnement en direct. Vous pouvez également importer un programme prédéfini à partir de la [bibliothèque de programmes Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

>[!CAUTION]
>
>Les programmes dont les listes dynamiques contiennent un déclencheur &quot;Objet personnalisé mis à jour&quot; entraînent l’échec de l’importation. Supprimez ce déclencheur de toutes les listes dynamiques avant de suivre les étapes décrites ci-dessous.

## Importation d’un programme {#importing-a-program}

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/import-a-program-1.png)

1. Cliquez sur la liste déroulante **[!UICONTROL New]** et sélectionnez **[!UICONTROL Import Program]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* L’importation de programme n’est disponible que pour les utilisateurs pour lesquels l’autorisation Importer un programme est activée. En savoir plus sur la [gestion des rôles et des autorisations utilisateur](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >* Pour connecter un compte sandbox à votre abonnement en direct, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Sélectionnez un **[!UICONTROL abonnement]** Marketo et un programme à importer. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-program-3.png)

1. Spécifiez un **[!UICONTROL dossier Campaign]** pour le programme importé. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Assurez-vous que les règles **[!UICONTROL Utiliser le conflit par défaut]** sont sélectionnées. Des règles de conflit sont nécessaires lorsque vous importez des programmes dans une instance dont les ressources portent le même nom.

1. Sélectionnez les détails de conflit de votre choix et cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Si vous importez un programme qui utilise des étapes de flux personnalisées ou des règles de liste dynamique dérivées d’un service d’étape de flux dans une instance de destination où il existe plusieurs fournisseurs de services compatibles, l’utilisateur importateur sera invité à affecter des étapes ou des règles au bon fournisseur dans l’instance de destination.

1. Prévisualisez les détails et **[!UICONTROL importez]** le programme.

   ![](assets/import-a-program-6.png)

Une fois l&#39;import terminé, vous recevrez une confirmation par email.

>[!NOTE]
>
>Vous devrez replanifier les campagnes par lots importées et activer les campagnes de déclenchement. Le système désactive automatiquement les plannings de campagne et déclenche les campagnes dans le programme importé.

## Impact sur Assets externe lors des importations de programme {#impact-on-external-assets-during-program-imports}

Les programmes utilisent des ressources externes telles que des modèles de courrier électronique, des modèles de page d’entrée, des images, des formulaires, des jetons et des balises de programme. Vous pouvez configurer la manière dont les modèles de page d’entrée et les balises de programme sont traités, et Marketo gère automatiquement le reste.

**Modèles de courrier électronique/page d’entrée :** Les modèles de courrier électronique/page d’entrée sont importés dans Design Studio. Vous pouvez utiliser des règles de conflit pour configurer le comportement lorsqu’il existe un modèle portant le même nom. Avec la règle par défaut, un nombre sera ajouté à un modèle s’il existe un modèle portant le même nom. Par exemple, si vous disposez déjà d’un modèle nommé &quot;Modèle standard&quot;, le nouveau modèle s’intitule &quot;Modèle standard - 1&quot;.

**Pages d’entrée/Forms :** Si un formulaire ou une page d’entrée portant le même nom existe dans Design Studio, ils seront toujours importés, mais avec un numéro ajouté à leur nom (ex : Page d’entrée - 1).

**Images :** Les images utilisées par les pages d’entrée sont importées dans le studio de conception, sauf si elles portent le même nom.

**Jetons :** Les jetons qui se trouvent en dehors d’un programme sont convertis en jetons locaux pendant le processus d’importation.

>[!CAUTION]
>
>Le type d’image que mes jetons ne sont pas pris en charge pour les importations de programme. Si un programme avec un type d&#39;image mes jetons est importé, des jetons _no_ seront disponibles.

**Balises du programme :** Vous pouvez utiliser des règles de conflit pour contrôler la manière dont seront traitées les balises du programme qui n’existent pas dans le compte de destination. L’utilisation de la règle par défaut crée les balises de programme ou vous pouvez choisir d’ignorer les balises.

>[!CAUTION]
>
>Lors de l&#39;import d&#39;un programme, les emails/landing pages contenant le [contenu dynamique](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} seront ignorés.
