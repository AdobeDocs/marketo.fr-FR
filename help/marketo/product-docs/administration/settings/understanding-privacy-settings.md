---
unique-page-id: 10617187
description: Présentation des paramètres de confidentialité - Documents Marketo - Documentation du produit
title: Présentation des paramètres de confidentialité
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: eccf4a66f5d3c581a82a363918b40ae37aa73576
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Présentation des paramètres de confidentialité {#understanding-privacy-settings}

## Vue d’ensemble {#overview}

Marketo permet aux marketeurs d’obtenir le consentement des visiteurs web pour les suivre. Il existe deux façons de se désinscrire, ou vous pouvez choisir d&#39;être suivi par une adresse IP anonymisée.

* Les visiteurs web sélectionnent la fonction Ne pas suivre (DNT) dans leur navigateur (et le marketeur honore la demande du visiteur web pour Ne pas suivre)
* Les visiteurs et visiteuses web utilisent un cookie de désinscription fourni par un spécialiste marketing sur un site web

Le marketeur peut également effectuer le suivi des utilisateurs, mais en utilisant une adresse IP anonymisée.

Ces méthodes peuvent avoir une incidence sur la valeur et les fonctionnalités de Marketo dans des zones spécifiques. Cependant, si le marketeur _ne modifie rien_ dans la configuration de Marketo, la fonctionnalité de Marketo reste la même.

## Paramètres du navigateur pour Ne pas suivre {#browser-settings-for-do-not-track}

Les visiteurs du Web peuvent paramétrer leur navigateur pour empêcher le suivi par n&#39;importe quel site Web en choisissant « Ne pas suivre » (DNT). Cela empêche le suivi de ce navigateur et de cet appareil en particulier. Consultez les paramètres de confidentialité du navigateur pour plus d’informations.

En [!DNL Munchkin], un spécialiste marketing peut [décider de prendre en charge ou d’ignorer le paramètre DNT du navigateur](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

Dans Web Personalization, un spécialiste du marketing peut décider de [prendre en charge ou ignorer le paramètre DNT du navigateur](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Exclusion d’un site web spécifique {#opt-out-from-a-specific-website}

Vous pouvez également autoriser les visiteurs et visiteuses du site à se désinscrire du suivi du site web de votre site web, que les paramètres **Ne pas suivre le navigateur** soient configurés ou non. Cela permet au visiteur du site de spécifier ses préférences de suivi directement à partir de votre site web.

Pour ce faire, vous devez ajouter un paramètre à un lien d’opt-out sur une page web dont le suivi des [!DNL Munchkin] est activé. Il peut s’agir de n’importe quelle page web, mais le lien de la page web doit contenir le paramètre suivant :

?marketo_opt_out=true

Vous trouverez ci-dessous des exemples de page web avec un lien d’opt-out et une page de destination pour une fois le lien cliqué. La vôtre varie.

Voici une page web comportant un bouton avec le paramètre «?marketo_opt_out=true » dans le lien d’exclusion.

![](assets/understanding-privacy-settings-1.png)

Vous pouvez créer et publier une page de destination en tant que page de suivi lorsque l’utilisateur clique sur votre lien avec le paramètre «?marketo_opt_out=true ».

![](assets/understanding-privacy-settings-2.png)

Lorsque l’utilisateur clique sur le lien, Marketo ajoute un cookie appelé **mkto_opt_out** au navigateur du visiteur, ce qui désactive [!DNL Munchkin] suivi pour le visiteur du site qui clique sur le lien avec le paramètre ci-dessus.

Pour vérifier que le cookie peut être placé, vérifiez que vous êtes un prospect sous forme de cookie et cliquez sur le lien. Vérifiez ensuite les cookies de votre navigateur pour vous assurer que le cookie **mkto_opt_out** a bien été ajouté.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Actuellement, cela fonctionne uniquement avec les versions 152 et ultérieures d’[!DNL Munchkin].

## Opt-in (Accord préalable) {#opt-in}

Les marketeurs peuvent permettre aux utilisateurs de s’inscrire en utilisant les fonctionnalités de Marketo dans les e-mails, les formulaires, les pages de destination et d’autres méthodes.

## Tracking à l’aide d’une adresse IP anonymisée {#tracking-using-an-anonymized-ip}

Les marketeurs peuvent préserver la confidentialité en suivant les utilisateurs avec une adresse IP anonymisée. Pour ce faire, ajoutez ce code au code RTP ou [!DNL Munchkin] JavaScript intégré au site web.

* Par [!DNL Munchkin], ajoutez simplement des `{"anonymizeIP",true}` à la fonction [init](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/configuration){target="_blank"}.

* Pour le Web Personalization (RTP), ajoutez ceci au javascript :

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
