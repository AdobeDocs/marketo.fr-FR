---
unique-page-id: 2359476
description: Utilisation du tableau de bord du programme de messagerie électronique - Documents Marketo - Documentation du produit
title: Utilisation du tableau de bord du programme de messagerie
exl-id: 47c1925a-144b-4277-a08d-1af660ed3d50
feature: Email Programs
source-git-commit: b2ceefb068005d916027fb71be0dc4e25849ae23
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Utilisation du tableau de bord du programme de messagerie {#use-the-email-program-dashboard}

Vérifiez les performances de vos programmes de messagerie avec cette vue de tableau de bord.

>[!CAUTION]
>
>Pour des rapports précis, évitez les _réutiliser_ un email provenant d’un programme de messagerie, soit en le référençant dans une campagne dynamique, soit en déplaçant la ressource du programme de messagerie lancé vers un nouveau programme. Cela agrégera toutes les données de chaque tableau de bord de rapport joint à cet email. Si vous devez réutiliser un email, veuillez [le cloner](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-an-asset-in-a-program.md){target="_blank"} car copie le courrier électronique, mais en crée un avec un nouvel ID de courrier électronique.

>[!NOTE]
>
>Si votre programme comporte un test A/B, consultez la [Tableau de bord du programme de messagerie électronique - Mode Test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}.

![](assets/image2014-9-12-14-3a12-3a56.png)

>[!NOTE]
>
>Toutes les données de cette vue sont agrégées (y compris le test A/B ainsi que l’envoi final de l’email).

## Email Send {#email-send}

Vous pouvez y voir le nombre d’emails envoyés, rebonds et remis.

![](assets/image2014-9-12-14-3a13-3a3.png)

>[!NOTE]
>
>En raison des normes de délivrabilité des emails qui ne sont pas sous le contrôle de Marketo, les statistiques de bounce et de Delivered sont approximatives, pas exactes.

## Ouvertures/clics {#opens-clicks}

Ce graphique montre le nombre d&#39;emails ouverts/cliqués pendant des périodes spécifiques après l&#39;exécution du programme de messagerie.

![](assets/image2014-9-12-14-3a13-3a7.png)

>[!TIP]
>
>Remarquez la diminution du nombre d’ouvertures/clics au fil du temps.

## Résumé - Engagement {#summary-engagement}

Vous pouvez ainsi visualiser l’ensemble [score d&#39;engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

![](assets/image2014-9-12-14-3a13-3a11.png)

## Résumé - REST {#summary-rest}

Le reste des données affichera les options Ouvertures, Clics, Ratio clic/ouverture et Désabonnement.

![](assets/image2014-9-12-14-3a13-3a15.png)

>[!TIP]
>
>La variable **Désabonner** Le taux dans l’exemple ci-dessus était si faible que Marketo a zoomé pour vous donner un meilleur aperçu. Le deuxième numéro de la barre est simplement ajouté à l’échelle.

>[!NOTE]
>
>**Définition**
>
>**Ouvertures** sont comptabilisés lorsque le destinataire de l’email télécharge les images de l’email, qui incluent un pixel de suivi inséré par Marketo. Si le destinataire consulte l&#39;email mais choisit de ne pas télécharger ses images, cela ne sera pas considéré comme une ouverture. Si les images se chargent dans le volet d&#39;aperçu du destinataire, cela sera généralement compté comme une ouverture, mais cela varie en fonction du client de messagerie.
>
>**Cliquez pour ouvrir** mesure le pourcentage d’emails ouverts et sur lesquels un lien a cliqué dans l’email. Nous prenons le nombre de clics uniques divisé par le nombre d’ouvertures uniques, puis multiplions par 100 pour l’afficher en pourcentage.

## Actualiser le tableau de bord {#refresh-dashboard}

Pour afficher les données les plus récentes, il vous suffit de cliquer sur l’icône d’actualisation du tableau de bord.

![](assets/refreshicon.png)

>[!MORELIKETHIS]
>
>[Utilisation du tableau de bord du programme de messagerie électronique - vue de test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}
