---
description: Présentation des options d’envoi de campagne commerciale pour les étapes d’e-mail - Documents Marketo - Documentation du produit
title: Comprendre les options d’envoi de campagne de ventes pour les étapes d’e-mail
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 2%

---

# Comprendre les options d’envoi de campagne de ventes pour les étapes d’e-mail {#understanding-sales-campaign-send-options-for-email-steps}

Lorsque vous créez une campagne de ventes, vous disposez de plusieurs options sur la manière dont les étapes d’e-mail sont créées dans [!DNL Sales Insight Actions]. De plus, selon l’emplacement de votre e-mail dans votre campagne de vente, vos options diffèrent également.

## Options d’envoi de la première étape {#first-step-send-options}

S’il s’agit de votre première étape et du premier jour de votre campagne de ventes, vous disposez des options suivantes :

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### Je choisirai quand envoyer cet e-mail {#first-step-i-will-choose}

* Cette option vous permet de choisir l’heure « Envoyer à » pour le premier e-mail de votre campagne de ventes lorsque vous lancez la campagne de ventes en ajoutant des personnes.

### Envoyez cet e-mail au moment suivant {#first-step-following-time}

* Lorsque vous lancez votre campagne de ventes en y ajoutant des personnes, nous planifierons l’e-mail pour cette période.
* Vous avez toujours la possibilité de choisir une nouvelle heure d&#39;envoi lorsque vous lancez votre campagne de ventes.

### Créer une tâche ; j’enverrai moi-même cet e-mail {#first-step-create-a-task}

* Cette option crée une tâche d’e-mail (et la synchronise sur [!DNL Salesforce]) que vous pouvez envoyer à votre convenance.
* Une fois cette sélection effectuée, lorsque vous lancez votre campagne de vente, ces tâches sont mises en file d’attente pour vous dans le centre de commande et le flux en direct. Vous pouvez ensuite personnaliser et envoyer (ou planifier) chaque e-mail avant qu’il ne soit envoyé.

   * Si vous ouvrez cette tâche dans notre application web, une fenêtre de composition s’ouvre avec l’adresse e-mail de votre contact, l’objet de votre e-mail et le modèle que vous avez choisi.
   * Si vous ouvrez cette tâche dans Gmail ou [!DNL Outlook], une fenêtre de composition native s’ouvre et l’adresse e-mail du contact, l’objet de l’e-mail et le modèle que vous avez choisi sont renseignés dynamiquement.

## Options d’envoi de l’étape suivante {#subsequent-step-send-options}

Pour les jours/étapes suivants de votre campagne de ventes, vous disposez des options suivantes :

### Envoyez cet e-mail en même temps que l’e-mail précédent dans cette campagne de ventes {#subsequent-send-at-same-time}

* Cette option envoie l’e-mail en même temps que l’e-mail directement avant lui.
* Il sera toujours envoyé le jour auquel il est associé.

>[!IMPORTANT]
>
>L&#39;envoi d&#39;un e-mail en même temps que l&#39;e-mail précédent n&#39;est pas pris en charge pour les e-mails envoyés le même jour. Au lieu de cela, l’e-mail sera envoyé au moment de l’e-mail envoyé à partir de la veille. Si cette option est sélectionnée pour un e-mail le premier jour de la campagne (non recommandé), cet e-mail sera envoyé immédiatement au début de la campagne.

### Envoyez cet e-mail au moment suivant {#subsequent-send-at-following-time}

* Lorsque vous lancez votre campagne de ventes en y ajoutant des personnes, nous planifierons l’e-mail pour cette période.
* Vous avez toujours la possibilité de choisir une nouvelle heure d&#39;envoi lorsque vous lancez votre campagne de ventes.

### Créer une tâche ; j’enverrai moi-même cet e-mail {#subsequent-create-a-task}

* Cette option crée une tâche d’e-mail (et la synchronise sur [!DNL Salesforce]) que vous pouvez envoyer à votre convenance.
* Une fois cette sélection effectuée, lorsque vous lancez votre campagne de vente, [!DNL Sales Insight Actions] met ces tâches en file d’attente pour vous dans le centre de commande et le flux en direct. Vous pouvez ensuite personnaliser et envoyer (ou planifier) chaque e-mail avant qu’il ne soit envoyé.

   * Si vous ouvrez cette tâche dans notre application web, une fenêtre de composition s’ouvre avec l’adresse e-mail de votre contact, l’objet de votre e-mail et le modèle que vous avez choisi.
   * Si vous ouvrez cette tâche dans Gmail ou [!DNL Outlook], une fenêtre de composition native s’ouvre et l’adresse e-mail du contact, l’objet de l’e-mail et le modèle que vous avez choisi sont renseignés dynamiquement.

### Créez cet e-mail en guise de suivi à l’e-mail précédent dans cette campagne {#subsequent-create-this-email}

* Cochez cette case si vous souhaitez que l’e-mail précédent de votre campagne de ventes soit ajouté à l’e-mail suivant que votre campagne de ventes envoie.
* Pour la copie jointe de l’e-mail, le modèle d’e-mail de votre campagne commerciale sera toujours envoyé. Toutes les modifications que l’utilisateur ou l’utilisatrice a apportées avant l’envoi ne seront pas incluses dans l’envoi.

>[!NOTE]
>
>Cette option de création d’un e-mail de relance n’est disponible que lors d’une étape par e-mail, lorsque l’étape précédente est également un e-mail. Si l’étape précédente est Appel, InMail ou Personnalisé, l’option de création d’un suivi n’apparaît pas.

>[!MORELIKETHIS]
>
>[Créer une campagne de ventes](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>>[Types d&#39;étapes de campagne commerciale et tâches de rappel](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>>[Paramètres de la campagne de ventes](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}

