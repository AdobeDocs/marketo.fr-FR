---
unique-page-id: 4720710
description: Configuration de SPF et DKIM pour la délivrabilité de vos emails - Documents Marketo - Documentation du produit
title: Configuration de SPF et DKIM pour la délivrabilité de vos emails
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Configuration de SPF et DKIM pour la délivrabilité de vos emails {#set-up-spf-and-dkim-for-your-email-deliverability}

Une méthode rapide pour améliorer les taux de diffusion de vos emails consiste à incorporer **SPF** (Sender Policy Framework) et **DKIM** (Domain Keys Identified Mail) dans vos paramètres DNS. Avec cet ajout à vos entrées DNS, vous informez les destinataires que vous avez autorisé Marketo à envoyer des emails en votre nom. Sans cette modification, votre email a de meilleures chances d’être marqué comme indésirable, car il a été envoyé à partir de votre domaine, mais à partir d’une adresse IP avec un domaine Marketo.

>[!CAUTION]
>
>Vous aurez besoin de votre administrateur réseau pour apporter cette modification à votre enregistrement DNS.

## Configuration de SPF {#set-up-spf}

**Si vous n’avez pas d’enregistrement SPF sur votre domaine**

Demandez à votre administrateur réseau d’ajouter la ligne suivante à vos entrées DNS. Remplacez [domain] par le domaine principal de votre site web (ex. &quot;company.com&quot;) et [corpIP] avec l’adresse IP de votre serveur de messagerie d’entreprise (ex. &quot;255.255.255.255&quot;). Si vous envoyez des emails à partir de plusieurs domaines via Marketo, vous devez les ajouter à chaque domaine (sur une seule ligne).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Si votre domaine contient un enregistrement SPF**

Si votre entrée DNS contient déjà un enregistrement SPF, ajoutez-y le code suivant :

include:mktomail.com

## Configuration de DKIM {#set-up-dkim}

**Qu&#39;est-ce que DKIM ? Pourquoi configurer DKIM ?**

DKIM est un protocole d’authentification utilisé par les destinataires d’un courrier électronique pour déterminer si un message électronique a été envoyé par celui qui le dit avoir été envoyé. DKIM améliore souvent la délivrabilité des emails vers la boîte de réception, car un destinataire peut être certain que le message n&#39;est pas une falsification.

**Comment fonctionne DKIM ?**

Après avoir configuré la clé publique dans votre enregistrement DNS et activé le domaine d’envoi dans la section Admin (A), nous activerons la signature DKIM personnalisée pour vos messages sortants, qui inclura une signature numérique chiffrée avec chaque email que nous vous envoyons (B). Les destinataires pourront déchiffrer la signature numérique en recherchant la &quot;clé publique&quot; dans le DNS (C) de votre domaine d’envoi. Si la clé de l&#39;email correspond à la clé de votre enregistrement DNS, le serveur de messagerie de réception sera plus susceptible d&#39;accepter l&#39;email Marketo envoyé en votre nom.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Comment configurer DKIM ?**

Reportez-vous à la section [Configuration d’une signature DKIM personnalisée](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [En savoir plus sur SPF et son fonctionnement](http://www.open-spf.org/Introduction/){target="_blank"}
>* [Ma configuration SPF est-elle correcte ?](https://www.kitterman.com/spf/validate.html){target="_blank"}
>* [Ai-je utilisé la syntaxe appropriée ?](http://www.open-spf.org/SPF_Record_Syntax/){target="_blank"}
