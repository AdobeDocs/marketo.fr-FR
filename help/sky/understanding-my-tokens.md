---
title: compréhension-mes-jetons
description: Présentation de mes jetons
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---


# Présentation de mes jetons

<br> 

Mes jetons sont des variables personnalisées que vous pouvez créer et utiliser dans vos programmes ou dossiers de campagne. Voici à quoi ils ressemblent : `{{_my.Name of Token_}}`

## Exemples

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Pour accéder à et créer Mes jetons, sélectionnez votre dossier de programme ou de campagne et accédez à l’onglet [!UICONTROL Mes jetons] . Faites glisser n’importe quel jeton sur votre canevas de jetons  locaux.

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

* **Jeton local :** Le jeton a été créé directement dans ce programme ou dossier.
* **[Jeton remplacé :](/help/sky/override-an-inherited-my-token.md)** Le jeton a été hérité, mais une exception a été faite dans ce programme ou dossier.
* **Jeton hérité :** Le jeton a été créé dans l’arborescence quelque part dans un programme ou un dossier de niveau supérieur.

Vous pouvez trouver ces trois types sous l’onglet [!UICONTROL **Mes jetons**] dans votre dossier de programme ou de campagne.

![Image 2](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Le déplacement de programmes et de dossiers affecte également les jetons. Vérifiez toujours que les références ne sont pas rompues pendant le déplacement.

>[!NOTE]
>
>Si le courrier électronique envoyé à partir d’un programme d’engagement est un message électronique enfant d’un programme par défaut (c.-à-d. non local à votre programme d’engagement), tous les jetons utilisés dans le courrier électronique sont résolus à partir du programme par défaut dans lequel réside le courrier électronique enfant.

## Utilisation du jeton

Sélectionnez un jeton, puis cliquez sur l’icône d’utilisation dans le coin supérieur droit pour afficher une liste de ressources qui contient ce jeton.

![Image trois](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Image 4](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Plongée profonde**

En savoir plus sur chacun des jetons My Tokens :

* [CRM Campaign](/help/sky/my-token-crm-campaign.md)
* [Date](/help/sky/my-token-date.md)
* [Fichier de calendrier](/help/sky/my-token-calendar-file.md)
* [Image](/help/sky/my-token-image.md)
* [Lien](/help/sky/my-token-link.md)
* [Nombre](/help/sky/my-token-number.md)
* [Texte enrichi](/help/sky/my-token-rich-text.md)
* [Score](/help/sky/my-token-score.md)
* [Script de courriel](/help/sky/my-token-email-script.md)
* [Texte](/help/sky/my-token-text.md)
