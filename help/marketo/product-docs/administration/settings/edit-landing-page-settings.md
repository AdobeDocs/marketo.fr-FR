---
unique-page-id: 2359918
description: Modifier les paramètres du Landing page - Documents marketing - Documentation du produit
title: Modifier les paramètres du Landing page
translation-type: tm+mt
source-git-commit: 95ca406109e04f56c9846f83cb2c4202bf606518
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Modifier les paramètres du Landing page {#edit-landing-page-settings}

Vous pouvez modifier le nom de domaine et la page de secours, activer ou désactiver le préremplissage de formulaire, éviter toute utilisation abusive de votre landing page, etc. Voici comment.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Sous **Admin**, cliquez sur **Landings page**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. Dans la section **Landings page** , cliquez sur **Modifier**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Entrez vos informations de domaine et de page.

   | Terme | Définition |
   |---|---|
   | Nom de domaine pour les landings page | Voici votre CNAME. Un CNAME est la première partie de l’URL que vous donnez aux personnes pour les landings page. Par exemple, dans `http://go.yourCompany.com`, le mot &quot;go&quot; est le CNAME. Vous pouvez en avoir plusieurs, mais la plupart des gens n&#39;utilisent que celle-ci. |
   | Page de secours | C&#39;est là qu&#39;il faut aller si le landing page n&#39;existe pas ou est en panne. En savoir plus sur les pages [de](set-a-fallback-page.md)secours. |
   | Page d&#39;accueil | Entrez l’URL de votre site d’entreprise. |

   ![](assets/three.png)

1. Cochez la case **Préremplissage** de formulaire pour autoriser les formulaires à préremplir les informations des personnes connues (cookies). Décochez la case pour bloquer.

   ![](assets/four.png)

1. Si vous souhaitez empêcher qu’un site malveillant ne semble héberger votre contenu, cochez la case **Ne pas autoriser l’incorporation de pages marketing dans des pages** Web externes.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Si vous souhaitez que la `<script>` balise de préremplissage s’affiche à la fin de la `<head>` balise dans le code, cochez la case **Injecter le script de préremplissage à la fin de l’en-tête** . Ne cochez pas cette case si vous souhaitez qu’elle s’affiche au début.
   >
   >Cochez la case **Supprimer les liens** de favicon par défaut pour empêcher Marketo d&#39;insérer des liens de favicon dans le code.

1. Après avoir effectué vos sélections, cliquez sur **Enregistrer.**

   ![](assets/six.png)

   Super boulot ! Vos landings page ont maintenant les bonnes informations et devraient début travailler immédiatement.

