---
unique-page-id: 14352477
description: Découvrez comment utiliser le bouton Push to Sales Connect dans Salesforce. Ajoutez des leads ou des contacts de Salesforce à Sales Connect en un seul clic.
title: Envoyer à  [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/piy3bPtiO48FQhWEmpu5qo4denlJ8v1ZU-VXBlWh0Mg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 190
ht-degree: 0%

---

# Intégrer à [!DNL Sales Connect] {#push-to-sales-connect}

Notre bouton [!UICONTROL Push to Tout] prendra une liste de vos leads/contacts dans [!DNL Salesforce] et les intégrera à un groupe dans [!DNL Sales Connect]. Vous pouvez ensuite envoyer rapidement un e-mail de groupe personnalisable avec le suivi Tout joint.

## Exigences {#requirements}

* Package [!DNL Sales Connect Salesforce] installé par [!DNL Salesforce] Admin

* Bouton [!UICONTROL Push to Sales Connect] installé pour afficher la liste par [!DNL Salesforce] administrateur

* [!DNL Salesforce] Connexion établie avec [!DNL Sales Connect] pour l&#39;utilisateur effectuant la notification push

## Comment {#how-to}

1. Cliquez sur l’onglet **[!UICONTROL Lead/Contact]** dans [!DNL Salesforce].
1. Basculez vers la vue Liste sur laquelle vous souhaitez POUSSER pour [!DNL Sales Connect] à côté du bouton [!UICONTROL Aller].
1. Cliquez sur **[!UICONTROL Aller]**.
1. Sélectionnez tous les leads/contacts que vous souhaitez promouvoir.
1. Sélectionnez **[!UICONTROL Push to MSE]**.
1. Une nouvelle fenêtre s’affiche pour vérifier le nombre de leads/contacts que vous souhaitez transférer. Sélectionnez **[!UICONTROL Passer au groupe]**.[!DNL Sales Connect] ne transmet aucun contact marqué comme [!UICONTROL Désinscription par e-mail] dans [!DNL Salesforce] ou [!UICONTROL Désabonné] dans [!DNL Sales Connect].

   >[!NOTE]
   >
   >[!DNL Sales Connect] ajoutera ce groupe intitulé « SFDC-... » à la page Relations de l’[application web](https://toutapp.com/login).

1. Sélectionnez **[!UICONTROL Envoyer un e-mail au groupe entier]** pour envoyer l’e-mail de ce groupe.
