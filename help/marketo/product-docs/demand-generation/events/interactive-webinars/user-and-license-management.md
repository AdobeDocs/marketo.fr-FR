---
description: Gestion des utilisateurs et des licences - Documents Marketo - Documentation du produit
title: Gestion des utilisateurs et des licences
hide: true
hidefromtoc: true
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
source-git-commit: 093af2946aa0279aff20d4388312fa7630e693a2
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

---

# Gestion des utilisateurs et des licences {#user-and-license-management}

Découvrez comment ajouter et supprimer des utilisateurs et afficher vos licences actuelles.

## Ajout d’un utilisateur {#add-a-user}

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/user-and-license-management-1.png)

1. Cliquez sur **Webinaires interactifs**.

   ![](assets/user-and-license-management-2.png)

1. Cliquez sur **Ajout/suppression d’utilisateurs**.

   ![](assets/user-and-license-management-3.png)

1. Cliquez sur la liste déroulante Utilisateurs disponibles , sélectionnez le ou les utilisateurs que vous souhaitez ajouter, puis cliquez sur **OK**.

   ![](assets/user-and-license-management-4.png)

## Suppression d’un utilisateur {#remove-a-user}

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/user-and-license-management-5.png)

1. Cliquez sur **Webinaires interactifs**.

   ![](assets/user-and-license-management-6.png)

1. Cliquez sur **Ajout/suppression d’utilisateurs**.

   ![](assets/user-and-license-management-7.png)

1. Mettez en surbrillance le ou les utilisateurs que vous souhaitez supprimer, puis appuyez sur la touche Suppr de votre clavier. Cliquez sur **OK** une fois terminé.

   ![](assets/user-and-license-management-8.png)

## Utilisation de la licence {#license-usage}

Les webinaires interactifs offrent des licences spécifiques pour la création d’événements Adobe Connect. Chaque fois qu’une licence est ajoutée, une nouvelle boîte d’utilisation de licence s’affiche. Les administrateurs de Marketo peuvent afficher (et non modifier) les licences en suivant les étapes ci-dessous. Contactez l’équipe du compte Adobe (votre gestionnaire de compte) pour obtenir des licences supplémentaires.

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/user-and-license-management-9.png)

1. Cliquez sur **Webinaires interactifs**.

   ![](assets/user-and-license-management-10.png)

1. Faites défiler jusqu’à la ou les cartes d’utilisation de la licence.

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>Date de début</b></td>
   <td>Date à laquelle la licence commence.</td>
  </tr>
  <tr> 
   <td><b>Date d’expiration</b></td>
   <td>Date d’expiration de la licence.</td>
  </tr>
  <tr> 
   <td><b>Type</b></td>
   <td>Type de licence achetée. Trois types sont disponibles : Licence d’événements partagés, licence d’espaces partagés, licence d’espace de stockage supplémentaire.</td>
  </tr>
  <tr> 
   <td><b>Capacité de l’événement</b></td>
   <td>Nombre maximum de participants pouvant être pris en charge dans un événement.</td>
  </tr>
  <tr> 
   <td><b>Nombre total d’événements</b></td>
   <td>Le nombre total d’événements qui ont été configurés avec cette licence.</td>
  </tr>
  <tr> 
   <td><b>Événements utilisés</b></td>
   <td>Nombre total d’événements terminés.</td>
  </tr>
  <tr> 
   <td><b>Capacité de stockage</b></td>
   <td>Quantité de stockage disponible pour le stockage des enregistrements, des collatéraux, des heros images, de la documentation et d’autres ressources.</td>
  </tr>
  </tbody>
</table>

**Informations à noter**

* Le type &quot;Licence de stockage supplémentaire&quot; fournit uniquement du stockage, par conséquent la valeur de chaque champ. _besides_ La capacité de stockage sera simplement répertoriée sous la forme &quot;-&quot;.

* Le type &quot;Licence de salle partagée&quot; contient un nombre illimité d’événements et &quot;Licence de stockage supplémentaire&quot; fournit uniquement du stockage. Le champ Total d’événements pour ces licences sera donc répertorié simplement comme &quot;-&quot;.

* Chaque fois qu’un événement est créé, il est compté comme &quot;consommé&quot; à partir de sa licence respective (sauf s’il s’agit d’une licence de salle partagée). La préférence sera accordée à la &quot;Licence d’événement partagé&quot; s’il existe à la fois une &quot;Licence d’événement partagé&quot; et une &quot;Licence d’espace partagé&quot; de la même capacité. Si l’événement n’a pas été diffusé et si le programme d’événements est supprimé avant l’heure planifiée, le nombre d’événements est réapprovisionné en soustrayant un événement des événements consommés.

* Une fois qu’une licence a été épuisée, sa mosaïque reste sur l’écran Webinaires interactifs de la section Admin avec les valeurs &quot;Total des événements&quot; et &quot;Événements consommés&quot; identiques. Ce n’est que lorsque la licence expire qu’elle sera supprimée de l’écran.
