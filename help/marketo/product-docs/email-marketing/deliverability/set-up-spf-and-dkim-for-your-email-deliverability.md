---
unique-page-id: 4720710
description: Configurez SPF et DKIM pour la délivrabilité de votre courrier électronique - Documents marketing - Documentation du produit
title: Configuration de SPF et DKIM pour la diffusion de vos e-mails
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# Configuration de SPF et DKIM pour la diffusion de vos e-mails {#set-up-spf-and-dkim-for-your-email-deliverability}

Une méthode rapide pour améliorer vos taux de diffusion de courriel consiste à incorporer **SPF** (Sender Policy Framework) et **DKIM** (Domain Keys Identified Mail) dans vos paramètres DNS. Avec cet ajout à vos entrées DNS, vous informez les destinataires que vous avez autorisé Marketo à envoyer des courriers électroniques en votre nom. Sans cette modification, votre courriel a plus de chances d’être marqué comme indésirable puisque le courriel a été envoyé à partir de votre domaine, mais à partir d’une adresse IP avec un domaine Marketo.

>[!CAUTION]
>
>Vous aurez besoin de votre administrateur réseau pour apporter cette modification à votre enregistrement DNS.

## Configuration de SPF {#set-up-spf}

**Si vous n’avez pas d’enregistrement SPF sur votre domaine**

Demandez à votre administrateur réseau d&#39;ajouter la ligne suivante à vos entrées DNS. Remplacez [domaine] par le domaine principal de votre site Web (ex. &quot;société.com&quot;) et [corpIP] avec l’adresse IP de votre serveur de messagerie d’entreprise (ex. &quot;255.255.255.255&quot;). Si vous envoyez des courriers électroniques de plusieurs domaines par l’intermédiaire de Marketing Cloud, vous devez les ajouter à chaque domaine (sur une seule ligne).
[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all\
Si vous possédez un enregistrement SPF sur votre domaine

Si votre entrée DNS contient déjà un enregistrement SPF, ajoutez-y les éléments suivants :

include:mktomail.com

## Configuration de DKIM {#set-up-dkim}

### Qu&#39;est-ce que DKIM ? Pourquoi dois-je configurer DKIM ? {#what-is-dkim-why-do-i-want-to-set-up-dkim}

DKIM est un protocole d’authentification utilisé par les destinataires du courrier électronique pour déterminer si un message électronique a été envoyé par celui qui l’a indiqué. DKIM améliore souvent la délivrabilité des e-mails à la boîte de réception, car un destinataire peut être certain que le message n&#39;est pas une contrefaçon.

Comment fonctionne DKIM ?

Après avoir configuré la clé publique dans votre enregistrement DNS et activé le domaine d’envoi dans la section Admin (A), nous activerons la signature DKIM personnalisée pour vos messages sortants, qui inclura une signature numérique chiffrée avec chaque e-mail que nous vous enverrons (B). Les récepteurs pourront déchiffrer la signature numérique en recherchant la &quot;clé publique&quot; dans le DNS (C) de votre domaine d&#39;envoi. Si la clé du courrier électronique correspond à la clé de votre enregistrement DNS, le serveur de messagerie destinataire sera plus susceptible d’accepter le courrier électronique envoyé par le marketing en votre nom.

![](assets/image2015-1-12-13-3a56-3a55.png)

Comment configurer DKIM ?

Reportez-vous à [Configuration d&#39;une signature](set-up-a-custom-dkim-signature.md)DKIM personnalisée.

>[!MORELIKETHIS]
>
>* [En savoir plus sur SPF et son fonctionnement](http://www.open-spf.org/Introduction/)
>* [Outils de délivrabilité des courriers électroniques de MarketingTo](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [Mon SPF est-il configuré correctement ?](http://www.kitterman.com/spf/validate.html)
>* [Ai-je utilisé la bonne syntaxe ?](http://www.open-spf.org/SPF_Record_Syntax/)

>



