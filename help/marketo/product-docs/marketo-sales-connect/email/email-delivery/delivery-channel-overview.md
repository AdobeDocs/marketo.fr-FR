---
unique-page-id: 14352407
description: Présentation du Canal de diffusion - Documentation du marketing - Documentation du produit
title: Présentation du Canal de diffusion
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Présentation du Canal de diffusion {#delivery-channel-overview}

Nous allons ventiler les trois canaux différents que vous pouvez exploiter, comment les sélectionner, quand choisir l&#39;un par rapport à l&#39;autre, et les nuances qui les entourent.

>[!NOTE]
>
>Ces informations ne sont pertinentes que si vous envoyez vos courriers électroniques à partir de l’application [](http://toutapp.com/login)Web. Si vous utilisez Sales Connect dans Gmail ou Outlook, vos courriels seront envoyés via ces serveurs de messagerie.

## Serveurs de messagerie MSC (par défaut) {#msc-email-servers-default}

Par défaut, cette méthode est sélectionnée pour la diffusion de vos courriels. Les serveurs de messagerie MSC sont une excellente option pour les utilisateurs qui n&#39;utilisent pas Gmail ou Outlook. De plus, puisqu&#39;ils sont nos serveurs, nous avons la possibilité de prendre tout message d&#39;erreur concernant les rebonds ou les diffusions en échec et de les remonter jusqu&#39;à vous dans la section &quot;Diffusions en échec&quot; de l&#39;onglet Conversations.

L&#39;utilisation des serveurs MSC présente un autre avantage : lors de l&#39;utilisation d&#39;une identité [de](https://help.toutapp.com/hc/en-us/articles/215371427)courriel, le destinataire voit l&#39;adresse électronique de l&#39;identité que vous avez créée.

Lorsque vous utilisez des serveurs MSC, vos destinataires peuvent voir une balise &quot;via toutapp.com&quot;. Il s&#39;agit de leur client de messagerie qui leur indique que le courrier électronique a été envoyé à l&#39;aide de Sales Connect.

Pour plus de détails, consultez cet article [d&#39;aide de](https://support.google.com/mail/answer/1311182?hl=en)Gmail.

>[!NOTE]
>
>Nos serveurs MSC n&#39;ont pas d&#39;enregistrement [](https://dmarc.org/) DMARC disponible. Ils ne peuvent pas être placés sur la liste autorisée sur vos propres serveurs.

## Serveur Gmail {#gmail-server}

Si votre fournisseur de messagerie de société est Gmail, vous pouvez utiliser votre compte existant pour envoyer vos courriels Sales Connect. Il s&#39;agit d&#39;une excellente option si vous souhaitez éviter les informations &quot;via toutapp.com&quot; et si vous préférez vous fier à la réputation de votre domaine de société et à la délivrabilité. Un autre avantage de l&#39;utilisation d&#39;un serveur Gmail est que tout ce que vous envoyez à partir de l&#39;application web sera automatiquement ajouté à votre dossier Gmail envoyé.

Nous ne pouvons nous connecter correctement qu&#39;avec un seul compte Gmail (une seule adresse email) qui vous fournira vos e-mails de Sales Connect. Cela signifie que si vous utilisez plusieurs identités de courriel, seule l’adresse du compte auquel nous sommes connectés apparaîtra lors de l’examen des détails.

Dans l’application Web, votre identité s’affiche au fur et à mesure que vous la créez (ci-dessus). Cependant, l&#39;envoi via les serveurs Gmail affichera l&#39;adresse du compte connecté.

>[!NOTE]
>
>Comme Sales Connect ne gère pas directement vos serveurs Gmail, nous n&#39;enregistrons pas les événements de messagerie rebondis dans l&#39;application Web.

## Serveur SMTP personnalisé  {#custom-smtp-server}

Payer pour votre propre serveur ? Utiliser un environnement Microsoft Exchange ? C&#39;est une option pour vous. Consultez [ces instructions](http://docs.marketo.com/x/zYTS) sur la configuration. Comme les serveurs Gmail, puisque Sales Connect ne gère pas directement votre serveur, nous n&#39;enregistrons pas les événements de messagerie rebondis dans l&#39;application Web.

