---
description: Gestion des utilisateurs et des licences - Documents Marketo - Documentation du produit
title: Gestion des utilisateurs et utilisatrices et des licences
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 3%

---

# Gestion des utilisateurs et utilisatrices et des licences {#user-and-license-management}

Découvrez comment ajouter et supprimer des utilisateurs, ainsi qu’afficher vos licences actuelles.

## Ajouter un utilisateur {#add-a-user}

1. Accédez à la zone **Admin**.

   ![](assets/user-and-license-management-1.png)

1. Cliquez sur **Webinaires interactifs**.

   ![](assets/user-and-license-management-2.png)

1. Cliquez sur **Ajouter/supprimer des utilisateurs**.

   ![](assets/user-and-license-management-3.png)

1. Cliquez sur la liste déroulante Utilisateurs disponibles, sélectionnez le ou les utilisateurs que vous souhaitez ajouter, puis cliquez sur **OK**.

   ![](assets/user-and-license-management-4.png)

## Supprimer un utilisateur {#remove-a-user}

1. Accédez à la zone **Admin**.

   ![](assets/user-and-license-management-5.png)

1. Cliquez sur **Webinaires interactifs**.

   ![](assets/user-and-license-management-6.png)

1. Cliquez sur **Ajouter/supprimer des utilisateurs**.

   ![](assets/user-and-license-management-7.png)

1. Mettez en surbrillance le ou les utilisateurs à supprimer, puis appuyez sur la touche Supprimer du clavier. Cliquez sur **OK** lorsque vous avez terminé.

   ![](assets/user-and-license-management-8.png)

## Utilisation des licences {#license-usage}

Les webinaires interactifs offrent des licences spécifiques pour créer des événements optimisés par Adobe Connect. Chaque fois qu’une licence est ajoutée, une nouvelle boîte d’utilisation de licence s’affiche. Les administrateurs Marketo peuvent afficher (et non modifier) les licences en suivant les étapes ci-dessous. Contactez l’équipe du compte Adobe (votre gestionnaire de compte) pour obtenir des licences supplémentaires.

1. Accédez à la zone **Admin**.

   ![](assets/user-and-license-management-9.png)

1. Cliquez sur **Webinaires interactifs**.

   ![](assets/user-and-license-management-10.png)

1. Faites défiler l’écran jusqu’à la ou les cartes Utilisation des licences .

   ![](assets/user-and-license-management-11.png)

<table>
  <tr>
   <td width="20%"><b>Date de début</b></td>
   <td width="80%">Date de début de la licence.</td>
  </tr>
  <tr>
   <td width="20%"><b>Date d’expiration</b></td>
   <td width="80%">Date d’expiration de la licence.</td>
  </tr>
  <tr>
   <td width="20%"><b>Type</b></td>
   <td width="80%">Type de licence acheté. Trois types sont disponibles : licence d’événements partagés, licence de salles partagées, licence de stockage supplémentaire.</td>
  </tr>
  <tr>
   <td width="20%"><b>Capacité de l'événement</b></td>
   <td width="80%">Nombre maximal de participants et participantes pouvant être accueillis dans un événement.</td>
  </tr>
  <tr>
   <td width="20%"><b>Nombre total d'événements</b></td>
   <td width="80%">Nombre total d’événements qui ont été configurés avec cette licence.</td>
  </tr>
  <tr>
   <td width="20%"><b>Événements consommés</b></td>
   <td width="80%">Tous les événements terminés et actuellement planifiés. <a href="#things-to-note">En savoir plus</a></td>
  </tr>
  <tr>
   <td width="20%"><b>Capacité de stockage</b></td>
   <td width="80%">Quantité de stockage disponible pour le stockage d’enregistrements, de documents, d’images principales et d’autres ressources.</td>
  </tr>
  </tbody>
</table>

### Éléments à noter {#things-to-note}

* Chaque fois qu’un événement est créé, il est comptabilisé comme « consommé » à partir de sa licence respective (sauf s’il s’agit d’une licence de salle partagée). La préférence est donnée à la « licence d’événement partagée » s’il existe à la fois une « licence d’événement partagée » et une « licence de salle partagée » de même capacité. Si l&#39;événement n&#39;a pas été diffusé et que le programme d&#39;événement est supprimé avant l&#39;heure planifiée, le nombre d&#39;événements est réapprovisionné. Si l&#39;événement n&#39;est pas diffusé et que le programme d&#39;événement n&#39;est pas supprimé avant l&#39;heure planifiée, l&#39;événement n&#39;est pas réapprovisionné.

* Le type « Licence de stockage supplémentaire » fournit uniquement du stockage. Par conséquent, la valeur dans chaque champ _en plus_ Capacité de stockage sera simplement répertoriée comme « - ».

* Le type « Licence de salle partagée » comporte un nombre illimité d’événements et « Licence de stockage supplémentaire » fournit uniquement l’espace de stockage. Le champ Total des événements pour ces licences sera donc simplement répertorié comme « - ».

* Une fois qu’une licence est épuisée, sa mosaïque reste sur l’écran des webinaires interactifs dans la section Administration avec « Total des événements » et « Événements consommés » ayant la même valeur. Ce n’est qu’à l’expiration de la licence qu’elle sera supprimée de l’écran.

## Accès utilisateur {#user-access}

Les webinaires interactifs permettent de réguler l’utilisation en donnant aux utilisateurs de Marketo Engage les autorisations de création et de diffusion de webinaires interactifs. Cependant, un utilisateur de webinaire interactif (ou un non-utilisateur) peut toujours avoir un accès en lecture/modification aux programmes d’événement de webinaires interactifs créés par d’autres utilisateurs.

Les utilisateurs de Marketo qui disposent des autorisations de webinaires interactifs et qui sont propriétaires d’un programme d’événement de webinaires interactifs spécifique pourront exécuter toutes les fonctions de webinaires interactifs liées à ce programme. Cela inclut : la création, l’accès, la modification, le clonage, le déplacement et la suppression de ce programme. Cependant, une fois que cet utilisateur n’est plus un utilisateur de webinaire interactif, le propriétaire du programme peut accéder au programme et le déplacer, mais ne peut effectuer aucune autre fonction.

Les utilisateurs de Marketo qui disposent des autorisations de webinaires interactifs et qui ne sont _pas_ propriétaires d’un programme d’événement de webinaires interactifs spécifique pourront exécuter des fonctions limitées sur ces programmes. Les utilisateurs non-administrateurs de Marketo pourront accéder au programme et le cloner, mais ils ne pourront effectuer aucune autre fonction s’ils disposent des autorisations pour les webinaires interactifs. Cependant, les utilisateurs administrateurs de Marketo _pourront_ exécuter toutes les fonctions, comme accéder à, modifier, cloner, déplacer et supprimer ce programme (à condition qu’ils disposent des autorisations pour les webinaires interactifs). Une fois cette autorisation révoquée pour les utilisateurs et utilisatrices administrateurs et non administrateurs de Marketo, ils ne pourront accéder qu’au programme d’événement de webinaire interactif et ne pourront effectuer aucune autre fonction.

La restriction des fonctions activables est indiquée par un bouton d’action grisé et un message de survol. Voici quelques exemples de boutons d’action grisés : « Créer votre webinaire » ou « Saisir votre webinaire ». Pour les fonctions non activables, un message soulignant les restrictions est fourni. Voir l’exemple ci-dessous :

![](assets/user-and-license-management-12.png)
