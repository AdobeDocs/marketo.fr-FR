---
description: Comment bloquer les envois de formulaires indésirables - Documents Marketo - Documentation du produit
title: Comment bloquer les envois de formulaires indésirables
translation-type: tm+mt
source-git-commit: 35ab8d353a2518a1603cb508a6f8c0ea650483e4
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Comment bloquer les envois de formulaires indésirables {#how-to-block-spam-form-submissions}

Souvent, les envois de formulaires avec une somme de contrôle non valide ou manquante (généralement à partir de robots) peuvent produire de fausses statistiques. Voici comment éviter cela.

>[!CAUTION]
>
>Cette fonctionnalité rejette les soumissions de formulaires effectuées à l’aide de POST programmatiques au point de terminaison leadCapture/save2. Si votre entreprise utilise une intégration qui envoie des formulaires à Marketo avec cette méthode, l’activation de cette fonctionnalité bloquera ces envois. L’utilisation de leadCapture/save2 en tant qu’API ou l’exécution directe d’envois de formulaire par programmation n’est pas prise en charge et est interdite. Assurez-vous que votre entreprise n&#39;envoie que les formulaires à l&#39;aide de : Ressources de formulaire, code de formulaires incorporés, API Forms2.js ou API REST de formulaire d’envoi.

1. Cliquez sur **Admin**.

   ![](assets/how-to-block-spam-form-submissions-1.png)

1. Cliquez sur **Poitrine de trésor**.

   ![](assets/how-to-block-spam-form-submissions-2.png)

1. En regard de **Capture de personne - Rejeter les valeurs de somme de contrôle non valides**, cliquez sur **Modifier**.

   ![](assets/how-to-block-spam-form-submissions-3.png)

1. Cochez la case **Activé** et cliquez sur **Enregistrer**.

   ![](assets/how-to-block-spam-form-submissions-4.png)

>[!NOTE]
>
>Lors de l’activation de cette fonctionnalité, vous pouvez voir une baisse de l’activité du formulaire lorsque les faux nombres sont filtrés.
