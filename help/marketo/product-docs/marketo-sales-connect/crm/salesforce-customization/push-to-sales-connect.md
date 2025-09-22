---
unique-page-id: 14352477
description: Push to [!DNL Sales Connect] - Documents Marketo - Documentation du produit
title: Envoyer à  [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
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
1. Une nouvelle fenêtre s’affiche pour vérifier le nombre de leads/contacts que vous souhaitez transférer. Sélectionnez **[!UICONTROL Passer au groupe]**.[!DNL Sales Connect] ne transmettra aucun contact marqué comme [!UICONTROL Désinscription par e-mail] dans [!DNL Salesforce] ou [!UICONTROL Désabonné] dans [!DNL Sales Connect].

   >[!NOTE]
   >
   >[!DNL Sales Connect] ajouterai ce groupe intitulé « SFDC-... » à la page Relations de l’[application web](https://toutapp.com/login).

1. Sélectionnez **[!UICONTROL Envoyer un e-mail au groupe entier]** pour envoyer l’e-mail de ce groupe.
