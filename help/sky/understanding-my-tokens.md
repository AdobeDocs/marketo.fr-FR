---
title: compréhension-mes-jetons
description: Présentation de mes jetons
exl-id: d56748e2-d742-45dd-96a8-dd80e30d9d8b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 5%

---

# Présentation de mes jetons

<br> 

Mes jetons sont des variables personnalisées que vous pouvez créer et utiliser dans vos programmes ou dossiers de campagne. Voici à quoi ils ressemblent : `{{_my.Name of Token_}}`

## Exemples

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Pour accéder à et créer Mes jetons, sélectionnez votre dossier de programme ou de campagne et accédez à l&#39;onglet [!UICONTROL Mes jetons]. Faites glisser n’importe quel jeton sur votre canevas [!UICONTROL Jetons locaux].

![Image un](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>Les noms de mes jetons ne peuvent pas être modifiés après leur enregistrement. Choisissez donc soigneusement.

>[!NOTE]
>
>Mes jetons ne seront pas résolus lors de l&#39;envoi d&#39;un courrier électronique à partir de Sales Insight sur Microsoft Dynamics ou Salesforce ; seuls les jetons standard sont renseignés (piste, Société, etc.). Les valeurs par défaut des jetons fonctionneront toutefois.

>[!NOTE]
>
>Les jetons de lien ne fonctionneront pas dans les courriers électroniques contenant uniquement du texte.

## Jetons imbriqués

Lorsque vous créez un jeton, il peut être référencé par d’autres objets de l’arborescence. Vous pouvez remplacer les variables globales à des niveaux inférieurs dans l’arborescence. Il existe une structure d&#39;attribution de noms pour l&#39;emplacement où le jeton a été créé afin d&#39;en faciliter la gestion.

* **Jeton local :** le jeton a été créé directement dans ce programme ou dossier.
* **[Jeton remplacé :](/help/sky/override-an-inherited-my-token.md)** le jeton a été hérité, mais une exception a été faite dans ce programme ou dossier.
* **Jeton hérité :** le jeton a été créé dans l’arborescence dans un programme ou un dossier de niveau supérieur.

Vous pouvez trouver ces trois types sous l&#39;onglet **[!UICONTROL Mes jetons]** dans votre dossier de programme ou de campagne.

![Image 2](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Le déplacement de programmes et de dossiers affecte également les jetons. Vérifiez toujours que les références ne sont pas rompues pendant le déplacement.

>[!NOTE]
>
>Si le courrier électronique envoyé à partir d’un programme d’engagement est un message électronique enfant d’un programme par défaut (c.-à-d. non local à votre programme d’engagement), tous les jetons utilisés dans le courrier électronique sont résolus à partir du programme par défaut dans lequel réside le courrier électronique enfant.

## Utilisation de jeton

Sélectionnez un jeton, puis cliquez sur l’icône d’utilisation dans le coin supérieur droit pour afficher une liste de ressources qui contient ce jeton.

![Image trois](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Image 4](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Pour aller plus loin**

En savoir plus sur chacun des jetons My Tokens :

* [Campagne CRM](/help/sky/my-token-crm-campaign.md)
* [Date](/help/sky/my-token-date.md)
* [Fichier du calendrier](/help/sky/my-token-calendar-file.md)
* [Image](/help/sky/my-token-image.md)
* [Lien](/help/sky/my-token-link.md)
* [Nombre](/help/sky/my-token-number.md)
* [Texte complet](/help/sky/my-token-rich-text.md)
* [Évaluation](/help/sky/my-token-score.md)
* [Script de l&#39;e-mail](/help/sky/my-token-email-script.md)
* [Texte](/help/sky/my-token-text.md)
