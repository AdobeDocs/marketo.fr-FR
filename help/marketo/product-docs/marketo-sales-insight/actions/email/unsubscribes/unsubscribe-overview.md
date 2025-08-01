---
description: Présentation Du Désabonnement - Documents Marketo - Documentation Du Produit
title: Présentation du désabonnement
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Présentation du désabonnement {#unsubscribe-overview}

Il est de plus en plus important pour les entreprises de se conformer aux lois sur la confidentialité des e-mails. Pour faciliter cette opération, nous avons apporté quelques améliorations à notre expérience de désabonnement.

* Des liens de désabonnement sont placés sur tous les e-mails envoyés depuis [!DNL Marketo Sales] et [!DNL Salesforce] (cela ne s’applique pas aux e-mails personnalisés envoyés depuis [!DNL Outlook] ou Gmail)
* Les administrateurs peuvent modifier les messages de désabonnement pour l’ensemble de leur équipe
* Les informations de désabonnement sont stockées dans un fichier PDF
* Les désabonnements peuvent être effectués manuellement : lien cliqué, synchronisation des [!DNL Salesforce] et rebond
* Nouvelle page de destination du lien de désabonnement

## Page de destination du lien de désabonnement {#unsubscribe-link-landing-page}

Lorsqu’une personne clique sur votre lien de désabonnement, elle est redirigée vers une page de destination de désabonnement où elle peut sélectionner ce dont elle souhaite se désabonner et pourquoi.

![](assets/unsubscribe-overview-1.png)

Ces informations seront enregistrées dans la vue des détails de la personne pour être affichées ultérieurement.

## Désabonner le groupe {#unsubscribe-group}

Voir et gérer toutes les personnes désabonnées en un seul endroit.

![](assets/unsubscribe-overview-2.png)

Utilisez la barre de recherche pour rechercher des personnes désabonnées.

![](assets/unsubscribe-overview-3.png)

Si vous êtes un administrateur, vous pouvez accéder au groupe de désabonnements pour effectuer un filtrage par [!UICONTROL Désabonnements du compte] et afficher tous les désabonnements qui ont été collectés dans votre base de données des personnes.

![](assets/unsubscribe-overview-4.png)

## Carte d’historique de désabonnement {#unsubscribe-history-card}

La carte [!UICONTROL Historique de désabonnement] permet aux administrateurs et aux utilisateurs d’obtenir des informations contextuelles sur l’historique de désabonnement de leurs contacts. Accédez-y en vous rendant dans l’onglet [!UICONTROL Personnes] et en sélectionnant une personne. Elle se trouve au bas de l’onglet [!UICONTROL  À propos ] dans la vue Détails de la personne.

>[!NOTE]
>
>Une carte [!UICONTROL Historique de désabonnement] ne s’affiche que si la personne s’est _réabonnée_ à un moment donné.

![](assets/unsubscribe-overview-5.png)

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>[!UICONTROL Date]</strong></td>
   <td><p>Affiche la date à laquelle le désabonnement/réabonnement a eu lieu.</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Details]</strong></td>
   <td><p>Se désabonner : un administrateur [!DNL Sales Connect] a supprimé manuellement le désabonnement de l’enregistrement du contact. Elle peut également afficher certains détails relatifs aux raisons du désabonnement du contact.</p><p>Désabonnement : le contact a été désabonné.</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Source]</strong></td>
   <td><p>[!DNL Salesforce] Synchronisation : le désabonnement a été capturé par une synchronisation à partir de [!DNL Salesforce].</p><p>Manuel : l’utilisateur a cliqué sur le bouton de désabonnement pour se désabonner.</p><p>Lien cliqué : le destinataire d’un e-mail a cliqué sur le lien de désabonnement.</p><p>« Nom de l’administrateur » : le nom d’un administrateur s’affichera lorsque l’action consistait à réabonner des contacts. Cela permet aux utilisateurs de savoir qui a supprimé le désabonnement.</p></td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[Personnaliser le message du lien de désabonnement](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
