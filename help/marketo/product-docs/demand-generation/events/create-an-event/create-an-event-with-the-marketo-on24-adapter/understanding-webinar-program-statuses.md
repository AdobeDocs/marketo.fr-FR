---
unique-page-id: 10096681
description: Présentation des états du programme Webinaire - Documents Marketo - Documentation du produit
title: Présentation des états du programme du webinaire
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Présentation des états du programme du webinaire {#understanding-webinar-program-statuses}

>[!IMPORTANT]
>
>Depuis août 2022, ON24 ne prend plus en charge les nouvelles intégrations Marketo. Les informations de cet article s’appliquent uniquement aux utilisateurs existants.

Les statuts de programme représentent les différents statuts d’un événement par le biais duquel une personne passe en tant que membre de l’événement. Ils sont associés à un type de canal. Marketo dispose d’un type de canal intégré appelé **Webinaire**. Les états peuvent être utilisés dans les campagnes par lots et les campagnes de déclenchement.

Les gens passent par les statuts de programme de façon linéaire et ne retournent pas dans leur statut. Par exemple, une personne dont le statut est **Attaché** ne peut pas revenir à **Inscrits**.

Voici une brève description des états du programme associé au canal Webinaire.

>[!TIP]
>
>Pour mettre à jour manuellement les états, cliquez sur  **Actualisation à partir du fournisseur de webinaire** dans le **Actions d’événement** menu déroulant.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Pas dans le programme** - Utilisez cet état pour supprimer des personnes de l’événement.

**Invité** - Utilisez cet état pour ajouter des personnes à l’événement.

**En attente d’approbation** - Utilisez ce statut pour suspendre l’envoi d’un email de confirmation à vos contacts. Voir &quot;Validation manuelle des inscrits&quot; dans [Mises à jour de l’enregistrement d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md) pour plus d’informations.

**Liste d’attente** - Utilisez ce statut pour que certaines personnes attendent jusqu&#39;à ce que des places supplémentaires soient disponibles.

**Rejetés** - Utilisez cet état pour rejeter l’enregistrement d’une personne sur votre événement.

**Inscrits** - Cet état envoie les personnes vers ON24 lorsque vous utilisez l’intégration ON24. Le statut de la personne est mis à jour lorsque ON24 indique que la personne a bien été enregistrée.

**Erreur d’enregistrement** - Cet état indique que l’utilisateur a rencontré une erreur lors de la tentative d’enregistrement de l’événement.

>[!NOTE]
>
>Si une erreur d’enregistrement se produit, vous pouvez obtenir des informations supplémentaires pour cette personne en consultant la colonne Raison de l’état dans l’onglet Membres de votre programme. Une fois l’erreur corrigée, vous pouvez modifier manuellement l’état du programme de l’utilisateur en Registered dans Marketo.

**Attaché** - A la fin du webinaire, ON24 renvoie une liste des participants. Cet état est automatiquement transmis dans Marketo.

**Participé à la demande** - Les personnes ayant assisté à la version archivée du webinaire reçoivent ce statut.

**Aucun affichage** - À la fin du webinaire et après l’extraction des données de fréquentation de ON24, le statut des personnes qui se sont inscrites mais n’y ont pas assisté est mis à jour vers No Show. Il peut s’écouler entre 30 minutes et 3 heures avant que l’on24 ne prépare les informations finales sur l’assiduité et les rende disponibles dans Marketo.

>[!NOTE]
>
>Pour que Marketo puisse extraire l’état Non affiché , les personnes doivent avoir été enregistrées. *dans Marketo*. Nous ne sommes pas en mesure de capturer Aucun affichage provenant du flux de données On24.

>[!MORELIKETHIS]
>
>[Présentation des événements de l’adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
