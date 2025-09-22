---
description: FAQ sur la synchronisation des comptes de personne - Documents Marketo - Documentation du produit
title: Questions fréquentes sur la synchronisation d’un compte de personne
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Questions fréquentes sur la synchronisation d’un compte de personne {#person-account-sync-faq}

Marketo Engage synchronise l’ensemble de votre base de données avec les [!DNL Veeva] pour le type d’enregistrements Compte de personne . Après la synchronisation, il attend 5 minutes, puis se synchronise à nouveau, toute la journée, tous les jours.

Les comptes de personne peuvent être configurés dans [!DNL Veeva] en fonction des besoins de votre entreprise.

>[!NOTE]
>
>Nous synchronisons uniquement les comptes de niveau « Professionnel » en tant que comptes de personne.

**Qu’est-ce qu’un compte personnel ?**

Un compte de personne est très similaire à l’objet de compte dans [!DNL Veeva] CRM. Cependant, un compte de personne a accès aux champs de compte et aux champs de contact.

**Que se passe-t-il lorsqu’un compte de personne est synchronisé avec Marketo ?**

Un compte de personne est synchronisé avec Marketo en tant que société et en tant que personne.

>[!NOTE]
>
>Les champs personnalisés d’un compte de personne sont copiés à la fois dans la société et dans la personne dans Marketo.

**Comment faire la distinction entre les comptes professionnels et les comptes particuliers ?**

Utilisez le filtre « Est un compte de personne » dans votre liste dynamique pour séparer les comptes de personne des comptes professionnels standard.

**Quel champ d’e-mail dois-je utiliser pour les comptes de personne ?**

Il existe deux champs d’adresse électronique pour un compte de personne. Utilisez le champ Adresse e-mail dans vos formulaires (et non l’adresse e-mail de la personne) pour vous assurer que la déduplication et le traitement des autres e-mails dans Marketo fonctionnent correctement.

## Direction de synchronisation {#sync-direction}

La synchronisation des champs liés aux contacts du compte de personne est bidirectionnelle. Si vous apportez des modifications à un contact dans [!DNL Veeva] CRM ou Marketo, vos mises à jour seront répercutées sur les deux systèmes. Les champs du compte ne se synchronisent que dans un seul sens, depuis [!DNL Veeva] CRM vers Marketo.

**Que se passe-t-il si des modifications sont apportées simultanément dans les deux systèmes aux champs Contact du compte de personne ?**

Nous serions gentils et laisserions [!DNL Veeva] CRM gagner. Il est toutefois rare que ce type de collision de données se produise.

**Les enregistrements de type Lead ou Contact sont-ils synchronisés avec [!DNL Veeva] CRM ?**

[!DNL Veeva] CRM traite uniquement des objets de compte de personne et dispose également de comptes professionnels. Les types CRM traditionnels de lead, contacts et opportunités ne sont pas vraiment utilisés dans les systèmes CRM [!DNL Veeva] traditionnels. Ils peuvent être créés dans [!DNL Veeva] CRM, mais ils ne sont pas officiellement pris en charge à l’aide de ce connecteur.

**Puis-je convertir un contact en contact dans Marketo ?**

Non, car le lead et le contact ne sont pas des types pris en charge pour la synchronisation avec [!DNL Veeva] CRM. La conversion n’est donc pas prise en charge.

**Puis-je forcer manuellement la synchronisation d&#39;un contact ?**

Non, puisque le contact n’est pas un type d’enregistrement indépendant, la synchronisation d’une personne avec [!DNL Veeva] n’est pas prise en charge.

**Chaque champ standard est-il synchronisé avec Marketo ?**

Non, tous les champs standard ne sont pas utiles. Tous les champs personnalisés peuvent faire partie de la synchronisation.

>[!NOTE]
>
>Marketo synchronise uniquement les champs auxquels l’utilisateur de synchronisation Marketo a accès.

**Marketo respectera-t-il les règles de validation [!DNL Veeva] ?**

Oui, en cas de conflit, nous consignerons le résultat dans le journal d’activité du prospect.

>[!MORELIKETHIS]
>
>* [Default [!DNL Veeva] Field Mapping](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Synchronisation des messages d’appel et de clé d’appel](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
