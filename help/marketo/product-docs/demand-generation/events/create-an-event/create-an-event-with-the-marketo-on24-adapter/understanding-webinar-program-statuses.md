---
unique-page-id: 10096681
description: Comprendre l'état des Programmes du webinaire - Documentation du marketing - Documentation du produit
title: Comprendre l'état des Programmes du webinaire
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---


# Comprendre l&#39;état des Programmes du webinaire {#understanding-webinar-program-statuses}

Les états de programme représentent les différents états de événement par lesquels une personne passe en tant que membre du événement. Ils sont associés à un type de canal. Marketo possède un type de canal intégré appelé **Webinaire**. Les états peuvent être utilisés dans les campagnes par lots et les campagnes déclencheuses.

Les gens se déplacent à travers les états de programme de façon linéaire et ne retournent pas dans le statut. Par exemple, une personne ayant le statut **Participé** ne peut pas revenir à **Enregistré**.

Voici une brève description des états des programmes associés au canal Webinaire.

>[!TIP]
>
>Pour mettre à jour manuellement les états, cliquez sur **Actualiser à partir du fournisseur de webinaires** dans la liste déroulante **Actions du Événement**.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Non dans le Programme**  - Utilisez cet état pour supprimer des personnes du événement.

** Invité** - Utilisez ce statut pour ajouter des personnes au événement.

**En attente d&#39;approbation**  - Utilisez cet état pour bloquer l&#39;envoi d&#39;un courrier électronique de confirmation à votre personnel. Pour plus d&#39;informations, consultez la section &quot;Approbation manuelle des inscrits&quot; dans [Mises à jour de l&#39;inscription au Événement ON24](on24-event-registration-updates.md).

**Liste d&#39;attente**  - Utilisez ce statut pour que certaines personnes attendent jusqu&#39;à ce que d&#39;autres places soient disponibles.

**Refusé**  - Utilisez ce statut pour rejeter l&#39;enregistrement d&#39;une personne sur votre Événement.

**Enregistré**  : ce statut envoie les utilisateurs vers ON24 lorsque vous utilisez l&#39;intégration ON24. Le statut de la personne est mis à jour lorsque ON24 répond que la personne a été enregistrée avec succès.

**Erreur**  d&#39;inscription : cet état indique que l&#39;utilisateur a rencontré une erreur lors de sa tentative d&#39;inscription au Événement.

>[!NOTE]
>
>Si une erreur d&#39;inscription se produit, vous pouvez obtenir des informations supplémentaires pour cette personne en consultant la colonne Motif de l&#39;état dans l&#39;onglet Membres de votre programme. Une fois l’erreur corrigée, vous pouvez modifier manuellement l’état de programme de l’utilisateur en Inscrit dans Marketing.

**Participé** - À la fin du webinaire, ON24 renvoie une liste de personnes qui ont assisté à la conférence. Cet état est automatiquement extrait dans Marketo.

**Participation à la demande**  - Les personnes qui ont assisté à la version archivée du webinaire reçoivent ce statut.

**No Show**  - A la fin du webinaire et après que les données de présence ont été extraites de ON24, le statut des personnes qui se sont inscrites mais n&#39;y ont pas assisté est mis à jour à No Show. Il peut prendre entre 30 minutes et 3 heures pour ON24 pour préparer les informations finales de présence et les rendre disponibles sur Marketo.

>[!NOTE]
>
>Pour que Marketo puisse retirer le statut Non Afficher, les personnes doivent avoir été enregistrées *dans Marketo*. Nous ne sommes pas en mesure de capturer Aucun affichage provenant du flux de données On24.

>[!MORELIKETHIS]
>
>* [Présentation des Événements d&#39;adaptateurs Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



