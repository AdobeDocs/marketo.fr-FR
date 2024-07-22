---
unique-page-id: 10096681
description: Présentation des états du programme Webinaire - Documents Marketo - Documentation du produit
title: Présentation des états du programme du webinaire
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Présentation des états du programme du webinaire {#understanding-webinar-program-statuses}

Les statuts de programme représentent les différents statuts d’un événement par le biais duquel une personne passe en tant que membre de l’événement. Ils sont associés à un type de canal. Marketo dispose d’un type de canal intégré appelé **Webinar**. Les états peuvent être utilisés dans les campagnes par lots et les campagnes de déclenchement.

Les gens passent par les statuts de programme de façon linéaire et ne retournent pas dans leur statut. Par exemple, une personne dont l’état est **Attending** ne peut pas revenir à **Registered**.

Voici une brève description des états du programme associé au canal Webinaire.

>[!TIP]
>
>Pour mettre à jour manuellement les états, cliquez sur **Actualiser à partir du fournisseur de webinaires** dans la liste déroulante **Actions d’événement** .

![](assets/image2015-12-17-13-3a52-3a39.png)

**Not in Program** - Utilisez cet état pour supprimer des personnes de l’événement.

**Invité** - Utilisez cet état pour ajouter des personnes à l’événement.

**Autorisation en attente** - Utilisez ce statut pour suspendre l’envoi d’un email de confirmation à vos utilisateurs. Pour plus d’informations, voir &quot;Validation manuelle des inscrits&quot; dans [Mises à jour de l’enregistrement d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"} .

**Liste d’attente** - Utilisez cet état pour faire attendre certaines personnes jusqu’à ce que des sièges supplémentaires soient disponibles.

**Refusé** - Utilisez cet état pour rejeter l’enregistrement d’une personne dans votre événement.

**Registered** - Cet état envoie les personnes vers ON24 lorsque vous utilisez l’intégration ON24. Le statut de la personne est mis à jour lorsque ON24 indique que la personne a bien été enregistrée.

**Erreur d’enregistrement** - Cet état indique que l’utilisateur a rencontré une erreur lors de la tentative d’enregistrement de l’événement.

>[!NOTE]
>
>Si une erreur d’enregistrement se produit, vous pouvez obtenir des informations supplémentaires pour cette personne en consultant la colonne Raison de l’état dans l’onglet Membres de votre programme. Une fois l’erreur corrigée, vous pouvez modifier manuellement l’état du programme de l’utilisateur en Registered dans Marketo.

**Participé** - À la fin du webinaire, ON24 renvoie une liste des personnes ayant assisté au séminaire. Cet état est automatiquement transmis dans Marketo.

**Participé à la demande** - Les personnes qui ont assisté à la version archivée du webinaire reçoivent ce statut.

**Non à l’affichage** - À la fin du webinaire et une fois les données de participation extraites de ON24, le statut des personnes qui se sont enregistrées mais n’ont pas assisté à l’événement est mis à jour vers Non à l’affichage. Il peut s’écouler entre 30 minutes et 3 heures avant que l’on24 ne prépare les informations finales sur l’assiduité et les rende disponibles dans Marketo.

>[!NOTE]
>
>Pour que Marketo puisse extraire l’état &quot;Aucun affichage&quot;, les personnes doivent avoir été enregistrées *dans Marketo*. Nous ne sommes pas en mesure de capturer Aucun affichage provenant du flux de données On24.

>[!MORELIKETHIS]
>
>[Compréhension des événements d’adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
