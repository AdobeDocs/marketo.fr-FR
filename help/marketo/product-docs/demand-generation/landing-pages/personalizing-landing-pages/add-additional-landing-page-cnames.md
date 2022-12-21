---
unique-page-id: 2359798
description: Ajout de CNAME de page d’entrée supplémentaires - Documents Marketo - Documentation du produit
title: Ajout de CNAME de page d’entrée supplémentaires
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Ajout de CNAME de page d’entrée supplémentaires {#add-additional-landing-page-cnames}

Vous pouvez ajouter des CNAME de landing page pour permettre à différentes URL de pointer vers vos landing pages Marketo. Suivez les étapes ci-dessous pour gérer plusieurs domaines.

>[!CAUTION]
>
>Les cookies ne peuvent pas être partagés entre les domaines.

>[!TIP]
>
>**Même domaine de niveau supérieur - Bon ! Les cookies sont partagés**.<br/> **go**.mycompany.com > **info**.mycompany.com
>
>**Domaines de niveau supérieur différents - Mauvais ! Les cookies sont _not_ shared**.<br/> allez-y.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Rechercher votre chaîne de compte {#find-your-account-string}

1. Accédez au **Administration** zone et clic **Pages d’entrée**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Copiez le **Chaîne de compte** de la **Paramètres** .

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Notez-le pour l’étape suivante.

## Envoyer la demande au service informatique {#send-request-to-it}

1. Demandez à votre service informatique de configurer le CNAME suivant : (Remplacer le mot [CNAME] avec le CNAME de votre choix et [CHAÎNE DE COMPTE] avec le texte de l’étape précédente).

   [CNAME].YourCompany.com > [CHAÎNE DE COMPTE].mktoweb.com

## Ajout d’un nouveau CNAME {#add-a-new-cname}

1. Une fois que votre service informatique a créé le CNAME, accédez à **Administration** puis cliquez sur **Pages d’entrée**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Cliquez sur **Nouveau** puis sélectionnez **Nouvel alias de domaine**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Saisissez votre **Alias du domaine.** Le **Page par défaut** s’affiche si le visiteur ne place pas d’URL. Entrez où ils doivent aller dans ce cas.

   >[!NOTE]
   >
   >Pour la page par défaut, vous pouvez sélectionner une landing page ou une URL externe, telle que votre site web public.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Saisissez votre **Page par défaut** et cliquez sur **Créer**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Beau ! Vous savez maintenant quoi faire si vous souhaitez ajouter un CNAME.
