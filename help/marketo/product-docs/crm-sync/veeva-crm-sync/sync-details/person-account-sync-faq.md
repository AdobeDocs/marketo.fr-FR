---
description: FAQ sur la synchronisation des comptes de personne - Documentation Marketo - Documentation du produit
title: FAQ sur la synchronisation des comptes de personne
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# FAQ sur la synchronisation des comptes de personne {#person-account-sync-faq}

Marketo Engage synchronise l’ensemble de votre base de données avec Veeva pour le type d’enregistrements Compte de personne . Après la synchronisation, il attend 5 minutes, puis se synchronise à nouveau, toute la journée, tous les jours.

Des comptes de personnes peuvent être configurés à Veeva pour répondre aux besoins de votre organisation.

>[!NOTE]
>
>Nous synchronisons uniquement les comptes de niveau &quot;professionnel&quot; en tant que comptes de personne.

**Qu’est-ce qu’un compte de personne ?**

Un compte de personne est très similaire à l’objet de compte dans le CRM Veeva. Cependant, un compte de personne a accès aux champs du compte et aux champs de contact.

**Que se passe-t-il lorsqu’un compte de personne est synchronisé avec Marketo ?**

Un compte de personne est synchronisé avec Marketo en tant qu’entreprise et en tant que personne.

>[!NOTE]
>
>Les champs personnalisés d’un compte de personne sont copiés dans la société et dans la personne dans Marketo.

**Comment puis-je différencier les comptes professionnels et les comptes de personnes ?**

Utilisez le filtre de compte &quot;Is Person&quot; dans votre liste dynamique pour séparer les comptes de personnes des comptes professionnels standard.

**Quel champ d’adresse électronique dois-je utiliser pour les comptes de personne ?**

Il existe deux champs de courrier électronique pour un compte de personne. Utilisez le champ Adresse électronique dans vos formulaires (et non l’adresse électronique de la personne) pour vous assurer que la déduplication de Marketo et d’autres processus de courrier électronique fonctionnent correctement.

## Direction de la synchronisation {#sync-direction}

La synchronisation des champs associés aux contacts du compte de personne est bidirectionnelle. Si vous apportez des modifications à un contact dans Veeva CRM ou Marketo, vos mises à jour seront répercutées dans les deux systèmes. Les champs du compte ne se synchronisent que dans une seule direction, de la gestion de la relation client Veeva à Marketo.

**Que se passe-t-il si des modifications sont effectuées simultanément dans les deux systèmes pour contacter les champs du compte de personne ?**

Nous serions gentils et laisserions Veeva CRM gagner. Il est toutefois rare que ce type de collision de données se produise.

**Les enregistrements de type Plate-forme ou Contact sont-ils synchronisés avec Veeva CRM ?**

Veeva CRM traite uniquement des objets de compte personnel et possède aussi des comptes professionnels. Les types CRM traditionnels de Lead, de contacts et d’opportunités ne sont pas vraiment utilisés dans les systèmes CRM traditionnels de Veeva. Ils peuvent être créés dans Veeva CRM, mais ils ne sont pas officiellement pris en charge à l’aide de ce connecteur.

**Puis-je convertir une personne en contact dans Marketo ?**

Non, puisque les types Prospect et Contact ne sont pas pris en charge pour la synchronisation avec la gestion de la relation client Veeva. Par conséquent, la conversion n’est pas prise en charge.

**Puis-je forcer manuellement la synchronisation d&#39;un contact ?**

Non, puisque Contact n’est pas un type d’enregistrement indépendant, la synchronisation d’une personne avec Veeva n’est pas prise en charge.

**Chaque champ standard est-il synchronisé avec Marketo ?**

Non, tous les champs standard ne sont pas utiles. Tous les champs personnalisés peuvent être synchronisés.

>[!NOTE]
>
>Marketo synchronise uniquement les champs auxquels votre utilisateur de synchronisation Marketo a accès.

**Marketo respectera-t-il les règles de validation de Veeva ?**

Oui, en cas de conflit, nous consignerons le résultat dans le journal d’activité du prospect.

>[!MORELIKETHIS]
>
>* [Mappage de champ Veeva par défaut](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Synchronisation des messages clés d’appel et d’appel](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
