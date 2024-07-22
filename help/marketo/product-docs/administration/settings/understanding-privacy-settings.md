---
unique-page-id: 10617187
description: Présentation des paramètres de confidentialité - Documents Marketo - Documentation du produit
title: Présentation des paramètres de confidentialité
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Présentation des paramètres de confidentialité {#understanding-privacy-settings}

## Vue d’ensemble {#overview}

Marketo permet aux spécialistes du marketing d’obtenir le consentement des visiteurs web pour effectuer leur suivi. Il existe deux façons de vous exclure ou vous pouvez choisir d’être suivi par une adresse IP anonyme.

* Les visiteurs web sélectionnent la fonction Ne pas suivre (DNT) dans leur navigateur (et le marketeur honore la demande du visiteur web de ne pas suivre).
* Les visiteurs web utilisent un cookie d’exclusion fourni par un marketeur sur un site web.

Le marketeur peut également effectuer le suivi des utilisateurs, mais utiliser une adresse IP anonyme.

Ces méthodes peuvent avoir une incidence sur la valeur et les fonctionnalités de Marketo dans des zones spécifiques. Cependant, si le spécialiste du marketing _ne modifie rien dans la configuration de Marketo, la fonctionnalité Marketo reste la même._

## Paramètres du navigateur pour Ne pas effectuer de suivi {#browser-settings-for-do-not-track}

Les visiteurs web peuvent définir leur navigateur pour empêcher le suivi par n’importe quel site web en sélectionnant &quot;Ne pas suivre&quot; (DNT). Cela empêche le suivi pour ce navigateur et cet appareil particulier. Pour plus d’informations, voir les paramètres de confidentialité du navigateur.

Dans [!DNL Munchkin], un marketeur peut [ décider de prendre en charge ou d’ignorer le paramètre DNT du navigateur ](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

Dans Web Personalization, un spécialiste du marketing peut décider de [prendre en charge ou d’ignorer le paramètre DNT du navigateur ](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Exclusion d’un site web spécifique {#opt-out-from-a-specific-website}

Vous pouvez également autoriser les visiteurs du site à exclure le suivi du site Web de votre site, que les paramètres **Browser Do Not Track** soient configurés ou non. Cela permet aux visiteurs du site de spécifier leurs préférences de suivi directement à partir de votre site web.

Pour ce faire, vous devez ajouter un paramètre à un lien d’exclusion sur une page web dont le suivi [!DNL Munchkin] est activé. Il peut s’agir de n’importe quelle page web, mais le lien de la page web doit contenir le paramètre suivant :

?marketo_opt_out=true

Vous trouverez ci-dessous des exemples de page web avec un lien d’exclusion et une page d’entrée pour une fois le lien cliqué. Les vôtres varieront.

Voici une page web avec un bouton avec le paramètre &quot;?marketo_opt_out=true&quot; dans le lien d’exclusion.

![](assets/understanding-privacy-settings-1.png)

Vous pouvez créer et publier une landing page en tant que page de relance lorsque vous cliquez sur votre lien avec le paramètre &quot;?marketo_opt_out=true&quot;.

![](assets/understanding-privacy-settings-2.png)

Lorsque l’utilisateur clique sur le lien, Marketo ajoute un cookie appelé **mkto_opt_out** au navigateur du visiteur qui désactive le suivi [!DNL Munchkin] pour le visiteur du site qui clique sur le lien avec le paramètre ci-dessus.

Pour vérifier que le cookie peut être implanté, vérifiez que vous êtes une piste avec cookie et cliquez sur le lien. Vérifiez ensuite les cookies de votre navigateur pour vérifier que le cookie **mkto_opt_out** a été ajouté.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Actuellement, cela fonctionne uniquement avec les versions 152 et ultérieures de [!DNL Munchkin].

## Participer {#opt-in}

Les marketeurs peuvent permettre aux utilisateurs de s’inscrire en utilisant les fonctionnalités de Marketo dans les emails, les formulaires, les landing pages et d’autres méthodes.

## Suivi à l’aide d’une adresse IP optimisée {#tracking-using-an-anonymized-ip}

Les marketeurs peuvent préserver la confidentialité en suivant les utilisateurs avec une adresse IP anonyme. Pour ce faire, ajoutez ce code au code JavaScript RTP ou [!DNL Munchkin] incorporé dans le site web.

* Pour [!DNL Munchkin], ajoutez simplement {&quot;anonymizeIP&quot;,true} à la fonction init.

  >[!NOTE]
  >
  >L’utilisation de ce paramètre nécessite l’activation de [!DNL Munchkin] V2. Pour l’activer pour votre abonnement, contactez le [support Marketo](https://nation.marketo.com/community/support_solutions).

* Pour Web Personalization (RTP), ajoutez ceci au JavaScript :

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
