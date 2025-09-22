---
unique-page-id: 10096681
description: Présentation Des Statuts Du Programme De Webinaire - Documents Marketo - Documentation Du Produit
title: Présentation des statuts du programme de webinaire
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 1%

---

# Présentation des statuts du programme de webinaire {#understanding-webinar-program-statuses}

Les statuts de programme représentent les différents statuts d&#39;un événement par lequel une personne passe en tant que membre de l&#39;événement. Ils sont associés à un type de canal. Marketo intègre un type de canal appelé **webinaire**. Les statuts peuvent être utilisés dans les campagnes par lots et de déclenchement.

Les gens passent d&#39;un statut de programme à l&#39;autre de façon linéaire et ne reviennent pas dans leur statut. Par exemple, une personne dont le statut est **Terminé avec succès** ne peut pas revenir à **Inscrit**.

Voici une brève description des statuts du programme associés au canal du webinaire.

>[!TIP]
>
>Pour mettre à jour manuellement les statuts, cliquez sur **Actualiser à partir du fournisseur de webinaires** dans le menu déroulant **Actions d’événement**.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Pas dans le programme** - Utilisez ce statut pour supprimer des personnes de l’événement.

**Invité** - Utilisez ce statut pour ajouter des personnes à l’événement.

**Approbation en attente** - Utilisez ce statut pour différer l’envoi d’un e-mail de confirmation à vos salariés. Pour plus d&#39;informations, consultez la section « Approbation manuelle des inscrits » dans [Mises à jour de l&#39;inscription aux événements ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}.

**En attente répertoriée** - Utilisez ce statut pour faire attendre certaines personnes jusqu’à ce que d’autres places soient disponibles.

**Refusé** - Utilisez ce statut pour refuser l’inscription d’une personne à votre événement.

**Enregistré** - Ce statut pousse les utilisateurs vers ON24 lorsque vous utilisez l’intégration ON24. Le statut de la personne est mis à jour lorsque ON24 répond que la personne a bien été enregistrée.

**Erreur d’enregistrement** - Ce statut indique que l’utilisateur a rencontré une erreur lors de sa tentative d’enregistrement à l’événement.

>[!NOTE]
>
>Si une erreur d’enregistrement se produit, vous pouvez obtenir des informations supplémentaires pour cette personne en regardant la colonne Raison du statut dans l’onglet Membres de votre programme. Une fois l’erreur corrigée, vous pouvez modifier manuellement le statut du programme de l’utilisateur en Enregistré dans Marketo.

**Participé** - À la fin du webinaire, ON24 renvoie une liste des personnes qui y ont assisté. Ce statut est automatiquement intégré à Marketo.

**Participants à la demande** - Les personnes qui ont assisté à la version archivée du webinaire reçoivent ce statut.

**Pas d’exposition** - À la fin du webinaire et après extraction des données de présence à partir de ON24, le statut des personnes qui se sont inscrites mais n’ont pas participé est mis à jour sur Pas d’exposition. On24 peut prendre entre 30 minutes et 3 heures pour préparer les informations finales de présence et les rendre disponibles dans Marketo.

>[!NOTE]
>
>Pour que Marketo puisse afficher le statut Non affiché, les personnes doivent avoir été enregistrées *dans Marketo*. Nous ne sommes pas en mesure de capturer les Aucun affichage provenant du flux de données On24.

>[!MORELIKETHIS]
>
>[Présentation des événements de l&#39;adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
