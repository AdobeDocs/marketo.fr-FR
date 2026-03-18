---
unique-page-id: 4720710
description: Découvrez comment configurer SPF et DKIM dans votre DNS pour améliorer la délivrabilité des e-mails. Autoriser Marketo à envoyer en votre nom et réduire les indicateurs de spam.
title: Configurer SPF et DKIM pour la délivrabilité de vos e-mails
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 94%

---

# Configurer SPF et DKIM pour la délivrabilité de vos e-mails {#set-up-spf-and-dkim-for-your-email-deliverability}

Une méthode rapide pour améliorer vos taux de diffusion e-mail consiste à incorporer **SPF** (Sender Policy Framework) et **DKIM** (Domain Keys Identified Mail) dans vos paramètres DNS. Avec cet ajout à vos entrées DNS, vous indiquez aux personnes destinataires que vous avez autorisé Marketo à envoyer des e-mails en votre nom. Sans cette modification, votre e-mail risque davantage d’être marqué comme indésirable, car il a été adressé à partir de votre domaine, mais envoyé à partir d’une adresse IP avec un domaine Marketo.

>[!CAUTION]
>
>Votre administrateur ou administratrice réseau devra effectuer cette modification dans votre enregistrement DNS.

## Configurer SPF {#set-up-spf}

**Si vous ne disposez PAS d’un enregistrement SPF sur votre domaine.**

Demandez à votre administrateur ou administratrice réseau d’ajouter la ligne suivante à vos entrées DNS. Remplacez [domain] par le domaine principal de votre site web (par exemple, « company.com ») et [corpIP] avec l’adresse IP de votre serveur de messagerie d’entreprise (par exemple, « 255.255.255.255 »). Si vous envoyez des e-mails à partir de plusieurs domaines via Marketo, vous devez l’ajouter à chaque domaine (sur une ligne).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Si votre domaine comporte un enregistrement SPF.**

Si vous avez déjà un enregistrement SPF existant dans l’entrée DNS, ajoutez-y ce qui suit :

include:mktomail.com

## Configurer DKIM {#set-up-dkim}

**Qu’est-ce que DKIM ? Pourquoi dois-je configurer DKIM ?**

DKIM est un protocole d’authentification utilisé par les personnes destinataires d’e-mails pour déterminer si un e-mail a bien été envoyé par l’entité indiquée. DKIM améliore souvent la délivrabilité des e-mails vers la boîte de réception, car la personne destinataire peut être certaine que le message n’est pas un faux.

**Fonctionnement de DKIM**

Après avoir configuré la clé publique dans votre enregistrement DNS et activé le domaine d’envoi dans la section Admin (A), nous activerons la signature DKIM personnalisée pour vos messages sortants, qui inclura une signature numérique chiffrée avec chaque e-mail que nous envoyons pour vous (B). Les personnes destinataires pourront déchiffrer la signature numérique en recherchant la « clé publique » dans le DNS (C) de votre domaine d’envoi. Si la clé dans l’e-mail correspond à la clé de votre enregistrement DNS, le serveur de messagerie de réception sera plus susceptible d’accepter l’e-mail Marketo envoyé en votre nom.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Comment configurer DKIM ?**

Reportez-vous à [Configuration d’une signature DKIM personnalisée](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* En savoir plus sur SPF et son fonctionnement`: http://www.open-spf.org/Introduction/`
>* Mon SPF est-il correctement configuré ? : `https://www.kitterman.com/spf/validate.html`
>* Ai-je utilisé la bonne syntaxe ? : `http://www.open-spf.org/SPF_Record_Syntax/`
