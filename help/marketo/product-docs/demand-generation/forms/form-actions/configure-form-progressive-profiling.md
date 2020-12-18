---
unique-page-id: 2359646
description: Configurer le profilage progressif de formulaire - Documents marketing - Documentation du produit
title: Configurer le profilage progressif du formulaire
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Configurer le profilage progressif de formulaire {#configure-form-progressive-profiling}

Les formes courtes sont bonnes ! Lorsque quelqu’un revient à un formulaire, vous pouvez présenter de nouveaux champs et remplir progressivement le profil du visiteur. Voici comment.

>[!NOTE]
>
>Pour que cette fonction fonctionne correctement, assurez-vous que le préremplissage du formulaire est activé pour les champs visibles et [désactivé](http://docs.marketo.com/display/DOCS/Disable+Pre-fill+for+a+Form+Field) pour les champs masqués.

1. Accédez à **Marketing** **Activités**.

   ![](assets/ma-1.png)

1. Sélectionnez votre formulaire et cliquez sur **Modifier** **Formulaire**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Sous **Formulaire** **Paramètres**, cliquez sur **Paramètres**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Définissez **Progressive** **Profilage** sur **Activé**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. D&#39;accord, maintenant on le configure. Accédez à **Field** **Details**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)
Faites glisser et déposez tous les champs qui font partie du jeu de profils progressif.
   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Une fois tous les champs déplacés, il doit ressembler à ceci :

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Les champs situés à l’extérieur de la zone **Profilé** **Profilage** s’affichent toujours dans le formulaire, même s’ils sont remplis.

1. Sélectionnez la zone **Profilement progressif** **Profilage**.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Soyez prudent lorsque vous utilisez les champs requis dans le profilage progressif. Ces champs peuvent toujours rester vides si le visiteur entre une nouvelle adresse électronique (qui créerait une nouvelle personne) après avoir envoyé des données pour les autres champs, car elles seraient supprimées sur le dernier formulaire.

1. Désormais, choisissez le nombre de champs vierges que vous souhaitez voir dans la zone **Progressif** **Profilement** à un moment donné.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >**Exemple**
   >
   >
   >Si vous sélectionnez **Nombre** **de** **Vierge** **Champs** comme 1, le visiteur voit ce qui suit pour la première fois :
   >
   >    
   >    
   >    * Prénom (vide)
   >    * Nom (vide)
   >    * Adresse électronique (vide)
   >    * Numéro de téléphone (vide)

   >    
   >    
   >En supposant qu’ils remplissent chaque champ, la deuxième fois qu’ils visitent, ils verront :
   >
   >    
   >    
   >    * Prénom (prérempli)
   >    * Nom (prérempli)
   >    * Adresse électronique (préremplie)
   >    * Numéro de téléphone mobile (vide)

   >    
   >    
   >En supposant qu&#39;ils remplissent le numéro de téléphone mobile, la troisième fois qu&#39;ils visitent, ils verront :
   >
   >    
   >    
   >    * Prénom (prérempli)
   >    * Nom (prérempli)
   >    * Adresse électronique (préremplie)
   >    * Pays (vide)


1. Cliquez sur **Terminer**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Cliquez sur **Approuver et fermer**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Beau boulot ! Le travail que vous venez de faire va payer.

Testez cette fonction et veillez à la tester. Elle est avancée, mais vous pouvez rendre vos formulaires très dynamiques de cette façon.
