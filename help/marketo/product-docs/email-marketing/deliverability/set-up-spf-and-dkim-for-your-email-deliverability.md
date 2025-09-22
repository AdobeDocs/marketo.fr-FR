---
unique-page-id: 4720710
description: Configurer SPF et DKIM pour la délivrabilité des e-mails - Documents Marketo - Documentation du produit
title: Configurer SPF et DKIM pour la délivrabilité de vos e-mails
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 4%

---

# Configurer SPF et DKIM pour la délivrabilité de vos e-mails {#set-up-spf-and-dkim-for-your-email-deliverability}

Une méthode rapide pour améliorer vos taux de diffusion e-mail consiste à incorporer **SPF** (Sender Policy Framework) et **DKIM** (Domain Keys Identified Mail) dans vos paramètres DNS. Avec cet ajout à vos entrées DNS, vous indiquez aux destinataires que vous avez autorisé Marketo à envoyer des e-mails en votre nom. Sans cette modification, votre e-mail risque davantage d’être marqué comme indésirable, car il a été adressé à partir de votre domaine, mais envoyé à partir d’une adresse IP avec un domaine Marketo.

>[!CAUTION]
>
>Votre administrateur réseau devra effectuer cette modification dans votre enregistrement DNS.

## Configurer SPF {#set-up-spf}

**Si vous ne disposez PAS d’un enregistrement SPF sur votre domaine**

Demandez à votre administrateur réseau d’ajouter la ligne suivante à vos entrées DNS. Remplacez [domain] par le domaine principal de votre site web (ex. « company.com ») et [corpIP] avec l’adresse IP de votre serveur de messagerie d’entreprise (par exemple,  »255.255.255.255 »). Si vous envoyez des e-mails à partir de plusieurs domaines via Marketo, vous devez l’ajouter à chaque domaine (sur une ligne).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Si votre domaine comporte un enregistrement SPF**

Si votre entrée DNS contient déjà un enregistrement SPF, ajoutez-y les éléments suivants :

include:mktomail.com

## Configuration de DKIM {#set-up-dkim}

**Qu’est-ce que DKIM ? Pourquoi dois-je configurer DKIM ?**

DKIM est un protocole d’authentification utilisé par les destinataires d’e-mails pour déterminer si un e-mail a été envoyé par qui il a été envoyé. DKIM améliore souvent la délivrabilité des e-mails vers la boîte de réception, car le destinataire peut être certain que le message n’est pas un faux.

**Comment DKIM fonctionne-t-il ?**

Après avoir configuré la clé publique dans votre enregistrement DNS et activé le domaine d’envoi dans la section Admin (A), nous activerons la signature DKIM personnalisée pour vos messages sortants, qui inclura une signature numérique chiffrée avec chaque e-mail que nous envoyons pour vous (B). Les récepteurs pourront déchiffrer la signature numérique en recherchant la « clé publique » dans le DNS (C) de votre domaine d&#39;envoi. Si la clé dans l’e-mail correspond à la clé de votre enregistrement DNS, le serveur de messagerie de réception sera plus susceptible d’accepter le Marketo d’e-mail envoyé en votre nom.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Comment configurer DKIM ?**

Reportez-vous à la section [Configuration d’une signature DKIM personnalisée](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* En savoir plus sur SPF et son fonctionnement`: http://www.open-spf.org/Introduction/`
>* Mon SPF est-il correctement configuré ? : `https://www.kitterman.com/spf/validate.html`
>* Ai-je utilisé la bonne syntaxe ? : `http://www.open-spf.org/SPF_Record_Syntax/`
