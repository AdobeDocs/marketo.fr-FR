---
description: Présentation des options d’envoi de campagne de ventes pour les étapes de courrier électronique - Documents Marketo - Documentation du produit
title: Présentation des options d’envoi de campagne de ventes pour les étapes de courrier électronique
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 832635c9e029754ce094e4137724bcc956dbcd35
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 2%

---

# Présentation des options d’envoi de campagne de ventes pour les étapes de courrier électronique {#understanding-sales-campaign-send-options-for-email-steps}

Lors de la création d’une campagne de ventes, vous disposez de plusieurs options pour créer vos étapes de courrier électronique dans les actions d’aperçu des ventes. En outre, en fonction de l’emplacement de votre email dans votre campagne de ventes, vos options diffèrent également.

## Options d’envoi première étape {#first-step-send-options}

Si c&#39;est votre première étape et le premier jour de votre campagne de ventes, vous disposez des options suivantes :

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### Je choisirai quand envoyer cet email {#first-step-i-will-choose}

* Cette option vous permet de choisir l’heure &quot;d’envoi&quot; pour le premier email de votre campagne de ventes lorsque vous lancez la campagne de ventes en ajoutant des personnes.

### Envoyer cet email à l&#39;heure suivante {#first-step-following-time}

* Lorsque vous lancez votre campagne de ventes en y ajoutant des personnes, nous planifions l’e-mail pour cette période.
* Vous avez toujours la possibilité de choisir un nouveau moment &quot;envoyer à&quot; lorsque vous lancez votre campagne de ventes.

### Créer une tâche ; j’enverrai moi-même cet e-mail {#first-step-create-a-task}

* Cette option crée une tâche de courrier électronique (et la synchronisation avec Salesforce) que vous pouvez envoyer à votre convenance.
* Une fois cette sélection effectuée, lorsque vous lancez votre campagne de ventes, nous mettrons ces tâches en file d’attente pour vous dans le Centre de commandes et le flux en direct. Vous pouvez ensuite personnaliser et envoyer (ou programmer) chaque email avant qu&#39;il ne sorte.

   * Si vous ouvrez cette tâche dans notre application web, une fenêtre de composition s’ouvre avec l’adresse email de votre contact, l’objet de votre email et le modèle que vous avez choisi.
   * Si vous ouvrez cette tâche dans Gmail ou Outlook, une fenêtre de composition native s’ouvre et vous renseignez dynamiquement l’adresse électronique de votre contact, l’objet de votre email et le modèle que vous avez choisi.

## Options d’envoi des étapes suivantes {#subsequent-step-send-options}

Pour tous les jours/étapes suivants de votre campagne de ventes, vous disposez des options suivantes :

### Envoyer cet email en même temps que l&#39;email précédent dans cette campagne de ventes {#subsequent-send-at-same-time}

* Cette option enverra l&#39;email en même temps que celui qui le précède directement.
* Il sera toujours envoyé le jour où il sera associé.

>[!IMPORTANT]
>
>L’envoi d’un email en même temps que le précédent email n’est pas pris en charge pour les emails envoyés le même jour. L’email sera envoyé au moment de l’envoi à partir du jour précédent. Si cette option est sélectionnée pour un email le premier jour de la campagne (non recommandée), cet email sera envoyé immédiatement au début de la campagne.

### Envoyer cet email à l&#39;heure suivante {#subsequent-send-at-following-time}

* Lorsque vous lancez votre campagne de ventes en y ajoutant des personnes, nous planifions l’e-mail pour cette période.
* Vous avez toujours la possibilité de choisir un nouveau moment &quot;envoyer à&quot; lorsque vous lancez votre campagne de ventes.

### Créer une tâche ; j’enverrai moi-même cet e-mail {#subsequent-create-a-task}

* Cette option crée une tâche de courrier électronique (et la synchronisation avec Salesforce) que vous pouvez envoyer à votre convenance.
* Une fois cette sélection effectuée, lorsque vous lancez votre campagne de ventes, les actions Sales Insight mettent ces tâches en file d’attente pour vous dans le Centre de commandes et le flux en direct. Vous pouvez ensuite personnaliser et envoyer (ou programmer) chaque email avant qu&#39;il ne sorte.

   * Si vous ouvrez cette tâche dans notre application web, une fenêtre de composition s’ouvre avec l’adresse email de votre contact, l’objet de votre email et le modèle que vous avez choisi.
   * Si vous ouvrez cette tâche dans Gmail ou Outlook, une fenêtre de composition native s’ouvre et vous renseignez dynamiquement l’adresse électronique de votre contact, l’objet de votre email et le modèle que vous avez choisi.

### Créez cet email comme suite à l&#39;email précédent dans cette campagne. {#subsequent-create-this-email}

* Activez cette case à cocher si vous souhaitez que le message précédent de votre campagne de vente soit ajouté au message suivant envoyé par votre campagne de ventes.
* Pour la copie annexée de l’email, le modèle d’email dans votre campagne de vente est toujours envoyé. Les modifications que l’utilisateur peut avoir effectuées avant son envoi ne seront pas incluses dans l’envoi.

>[!NOTE]
>
>Cette option de création d’un email en tant que suivi n’est disponible que lors d’une étape d’email, lorsque l’étape précédente est également un email. Si l’étape précédente est Appel, InMail ou Personnalisé, l’option de création d’un suivi ne s’affiche pas.

>[!MORELIKETHIS]
>
>[Créer une campagne de ventes](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>[Types d’étape de campagne de vente et tâches de rappel](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>[Paramètres de campagne de ventes](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}

