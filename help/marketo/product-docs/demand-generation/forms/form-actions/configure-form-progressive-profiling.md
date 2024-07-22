---
unique-page-id: 2359646
description: Configurer le profilage progressif de formulaire - Documents Marketo - Documentation du produit
title: Configurer le profilage progressif du formulaire
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Configurer le profilage progressif du formulaire {#configure-form-progressive-profiling}

Les formulaires courts sont bons ! Lorsqu’une personne revient à un formulaire, vous pouvez présenter de nouveaux champs et remplir progressivement le profil du visiteur. Voici comment.

>[!NOTE]
>
>Pour que cette fonction fonctionne correctement, assurez-vous que l’option Form Pre-Fill (Préremplissage de formulaire) est activée pour les champs visibles et que l’option [disabled](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) pour les champs masqués.

1. Accédez à **Activités marketing**.

   ![](assets/ma-1.png)

1. Sélectionnez votre formulaire et cliquez sur **Modifier le formulaire**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Sous **Paramètres de formulaire**, cliquez sur **Paramètres**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Définissez **Profilage progressif** sur **Activé**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Ok, maintenant, on le configure. Accédez à **Field Details**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Faites glisser et déposez tous les champs qui font partie du jeu de profils progressifs.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Lorsque vous avez terminé de déplacer tous les champs, cela doit ressembler à ceci :

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Les champs situés en dehors de la zone **Profilage progressif** s’affichent toujours dans le formulaire, même s’ils sont remplis.

1. Sélectionnez la zone **Profilage progressif** .

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Soyez prudent lorsque vous utilisez les champs requis dans le Profilage progressif. Ces champs peuvent toujours être laissés vides si le visiteur saisit une nouvelle adresse électronique (qui créerait une nouvelle personne) après avoir précédemment soumis des données pour les autres champs, car ils seront supprimés dans le dernier formulaire.

1. Sélectionnez maintenant le nombre de champs vierges à afficher dans la zone **Profilage progressif** à un moment donné.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Si vous choisissez **Number** **of** **Blank** **Fields** comme 1, le visiteur verra la première fois qu’il verra ce formulaire :
   >
   >* Prénom (vide)
   >* Nom (vide)
   >* Adresse électronique (vide)
   >* Numéro de téléphone (vide)
   >
   >En supposant qu’ils remplissent chaque champ, la deuxième fois qu’ils le visitent, ils verront :
   >
   >* Prénom (prérempli)
   >* Nom (prérempli)
   >* Adresse électronique (préremplie)
   >* Numéro de téléphone mobile (vide)
   >
   >En supposant qu’ils renseignent le numéro de téléphone mobile, la troisième fois qu’ils visitent, ils verront :
   >
   >* Prénom (prérempli)
   >* Nom (prérempli)
   >* Adresse électronique (préremplie)
   >* Pays (vide)

1. Cliquez sur **Terminer**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Cliquez sur **Approuver et fermer**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Beau boulot ! Le travail que tu viens de faire va payer.

Testez cette fonctionnalité et veillez à la tester. Il est avancé, mais vous pouvez rendre vos formulaires très dynamiques de cette façon.
