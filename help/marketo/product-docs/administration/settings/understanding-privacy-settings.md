---
unique-page-id: 10617187
description: Présentation des paramètres de confidentialité - Documents marketing - Documentation du produit
title: Présentation des paramètres de confidentialité
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Présentation des paramètres de confidentialité {#understanding-privacy-settings}

## Aperçu {#overview}

Marketo permet aux spécialistes du marketing d&#39;obtenir le consentement des visiteurs Web pour les suivre. Il existe deux façons de opt-out, ou vous pouvez choisir d’être suivi par une adresse IP anonyme.

* Les visiteurs Web sélectionnent la fonction Ne pas suivre (DNT) dans leur navigateur (et le spécialiste du marketing honore la demande du visiteur Web de ne pas suivre).
* Les visiteurs Web utilisent un cookie opt-out fourni par un spécialiste du marketing sur un site Web.

Le spécialiste du marketing peut également effectuer un suivi sur les utilisateurs, mais utiliser une adresse IP anonyme.

Ces méthodes peuvent affecter la valeur et les fonctionnalités du marketing dans des domaines spécifiques. Cependant, si le spécialiste du marketing *ne* change rien dans la configuration de Marketo, la fonctionnalité de Marketo reste la même.

## Paramètres du navigateur pour Ne pas effectuer le suivi {#browser-settings-for-do-not-track}

Les visiteurs Web peuvent définir leur navigateur pour empêcher le suivi par n’importe quel site Web en choisissant &quot;Ne pas suivre&quot; (DNT). Ceci empêche le suivi pour ce navigateur et ce périphérique en particulier. Consultez les paramètres de confidentialité du navigateur pour en savoir plus.

Dans Munchkin, un spécialiste du marketing peut [décider de prendre en charge ou d’ignorer le paramètre DNT du navigateur](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

Dans la personnalisation Web, un spécialiste du marketing peut décider de [prendre en charge ou d’ignorer le paramètre DNT du navigateur](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## opt-out à partir d&#39;un site Web spécifique {#opt-out-from-a-specific-website}

Vous pouvez également autoriser les visiteurs du site à opt-out le suivi des sites Web à partir de votre site Web, que les paramètres **Navigateur Ne pas suivre** soient ou non configurés. Cela permet au visiteur du site de spécifier ses préférences de suivi directement depuis votre site Web.

Pour ce faire, vous devez ajouter un paramètre à un lien opt-out sur une page Web pour laquelle le suivi de la serviette est activé. Il peut s’agir de n’importe quelle page Web, mais le lien de la page Web doit contenir le paramètre suivant :

?marketo_opt_out=true

Vous trouverez ci-dessous des exemples de page Web contenant un lien d’exclusion et un landing page pour une fois le lien cliqué. Les vôtres varieront.

Voici une page Web avec un bouton avec le paramètre &quot;?marketo_opt_out=true&quot; dans le lien d’exclusion.

![](assets/opt-out-1.png)

Vous pouvez créer et publier un landing page en tant que page de suivi lorsque vous cliquez sur votre lien avec le paramètre &quot;?marketo_opt_out=true&quot;.

![](assets/opt-out-2.png)

Lorsque vous cliquez sur le lien, Marketo ajoute un cookie nommé **mkto_opt_out** au navigateur du visiteur qui désactive le suivi Munchkin pour le visiteur du site qui clique sur le lien avec le paramètre ci-dessus.

Pour vérifier que le cookie peut être implanté, vérifiez que vous êtes une piste avec cookie et cliquez sur le lien. Vérifiez ensuite les cookies de votre navigateur pour vérifier que le cookie **mkto_opt_out** a été ajouté.

![](assets/opt-out-3.png)

>[!NOTE]
>
>Pour l&#39;instant, cela ne fonctionne qu&#39;avec les versions 152 et ultérieures de Munchkin.

## opt-in {#opt-in}

Les marketeurs peuvent permettre aux utilisateurs de opt-in en utilisant les fonctionnalités de Marketo dans les courriels, les formulaires, les landings page et d’autres méthodes.

## Suivi à l’aide d’une adresse IP anonyme {#tracking-using-an-anonymized-ip}

Les marketeurs peuvent préserver la confidentialité en suivant les utilisateurs avec une adresse IP anonyme. Pour ce faire, ajoutez ce code au code Javascript RTP ou Munchkin qui est incorporé dans le site Web.

* Pour Munchkin, ajoutez simplement {&quot;anonymizeIP&quot;,true} à la fonction init.

   >[!NOTE]
   >
   >L&#39;utilisation de ce paramètre nécessite l&#39;activation de Munchkin V2. Pour l&#39;activer pour votre abonnement, contactez le [Support marketing](http://nation.marketo.com/community/support_solutions).

* Pour la personnalisation Web (RTP), ajoutez ceci au javascript :

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
