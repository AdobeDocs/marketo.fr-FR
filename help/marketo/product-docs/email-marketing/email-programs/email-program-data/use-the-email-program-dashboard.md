---
unique-page-id: 2359476
description: Utiliser le tableau de bord du programme de messagerie électronique - Documents Marketo - Documentation du produit
title: Utiliser le tableau de bord du programme d’e-mail
exl-id: 47c1925a-144b-4277-a08d-1af660ed3d50
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 3%

---

# Utiliser le tableau de bord du programme d’e-mail {#use-the-email-program-dashboard}

Découvrez comment vos programmes de messagerie se comportent avec cette vue de tableau de bord.

>[!CAUTION]
>
>Pour des rapports précis, évitez de _réutiliser_ un e-mail d’un programme de messagerie, soit en le référençant dans une campagne dynamique, soit en déplaçant la ressource du programme de messagerie lancé vers un nouveau programme. Toutes les données de chaque tableau de bord de rapports joint à cet e-mail seront ainsi agrégées. Si vous devez réutiliser un e-mail, [clonez-le](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-an-asset-in-a-program.md){target="_blank"} à la place, car cela copie l’e-mail, mais en crée un nouveau avec un nouvel ID d’e-mail.

>[!NOTE]
>
>Si votre programme comporte un test A/B, consultez la section [Tableau de bord du programme d’e-mail - Vue Test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}.

![](assets/image2014-9-12-14-3a12-3a56.png)

>[!NOTE]
>
>Toutes les données de cette vue sont agrégées (inclut le test A/B ainsi que l’envoi final de l’e-mail).

## Email Send {#email-send}

Vous pouvez voir ici combien d’e-mails ont été envoyés, rejetés et diffusés.

![](assets/image2014-9-12-14-3a13-3a3.png)

>[!NOTE]
>
>En raison des normes de délivrabilité des e-mails qui ne sont pas contrôlées par Marketo, les statistiques Rebonds et Diffusions sont approximatives, et non exactes.

## Ouvertures/clics {#opens-clicks}

Ce graphique montre le nombre d’e-mails ouverts/ayant fait l’objet d’un clic pendant des périodes spécifiques après l’exécution du programme de messagerie.

![](assets/image2014-9-12-14-3a13-3a7.png)

>[!TIP]
>
>Notez que le nombre d’ouvertures/clics diminue au fil du temps.

## Résumé - Engagement {#summary-engagement}

Cela vous montre le [score d’engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"} global.

![](assets/image2014-9-12-14-3a13-3a11.png)

## Résumé - Reste {#summary-rest}

Le reste des données affiche Ouvertures, Clics, Taux de clics/ouvertures et Désabonnements.

![](assets/image2014-9-12-14-3a13-3a15.png)

>[!TIP]
>
>Le taux de **Désabonnement** dans l’exemple ci-dessus était si faible que Marketo a effectué un zoom avant pour vous donner une meilleure apparence. Le deuxième nombre à l&#39;intérieur de la barre est simplement ajouté pour l&#39;échelle.

>[!NOTE]
>
>**Définition**
>
>Les **[!UICONTROL ouvertures]** sont comptabilisées lorsque le destinataire de l’e-mail télécharge les images de l’e-mail, qui incluent un pixel de suivi inséré dans Marketo. Si le destinataire consulte l’e-mail mais choisit de ne pas télécharger ses images, cela ne sera pas comptabilisé comme une ouverture. Si les images se chargent dans le volet d’aperçu du destinataire, cela compte généralement comme une ouverture, mais cela varie en fonction du client de messagerie.
>
>**[!UICONTROL Cliquer pour ouvrir]** mesure le pourcentage d’e-mails ouverts avec un lien sur lequel l’utilisateur a cliqué. Nous divisons le nombre de clics uniques par le nombre d’ouvertures uniques, puis nous le multiplions par 100 pour l’afficher en pourcentage.

## Actualiser le tableau de bord {#refresh-dashboard}

Pour afficher les données les plus récentes, il vous suffit de cliquer sur l’icône d’actualisation dans le tableau de bord.

![](assets/refreshicon.png)

>[!MORELIKETHIS]
>
>[Utiliser le tableau de bord du programme de messagerie - Vue Test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}
