---
description: Découvrez comment les remplacements du suivi des e-mails au niveau de la personne vous permettent de contrôler l’ouverture des e-mails et le suivi des clics pour chaque personne afin de prendre en charge les exigences de consentement et de confidentialité.
title: Suivi des e-mails au niveau de la personne
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/kF-5V-G6-xr3uV-NQBTmFNfhQnk-r-RYt-v0HvJ-4Go'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a913c84b1c4f8927c951af685884edfc792ff213
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 2%
---
# Suivi des e-mails au niveau de la personne {#email-tracking-at-person-level}

Les remplacements du suivi des e-mails au niveau de la personne vous permettent d’appliquer une valeur par défaut au niveau de l’environnement Marketo, puis de modifier cette valeur par défaut pour des personnes individuelles. Le suivi des ouvertures et des clics est contrôlé indépendamment.

Utilisez cette fonctionnalité lorsque vos exigences de confidentialité ou vos politiques d’organisation nécessitent un consentement avant le suivi de l’engagement des e-mails.

>[!IMPORTANT]
>
>Cette fonctionnalité fournit des contrôles qui peuvent vous aider à respecter vos obligations de conformité ; elle ne détermine pas les lois qui s’appliquent ni les personnes qui doivent donner leur consentement. Collaborez avec vos équipes juridiques et de confidentialité pour décider comment configurer le suivi et comment collecter et conserver le consentement.

## Fonctionnement du suivi des décisions {#how-tracking-decisions-work}

Trois paramètres fonctionnent ensemble :

| Paramètre | Niveau | Fonction |
|---|---|---|
| **Remplacements du suivi des e-mails au niveau de la personne** | Environnement | Active ou désactive la fonction. Lorsqu’il est désactivé, Marketo Engage ignore les champs d’environnement par défaut et de remplacement de personne et utilise le comportement de suivi normal. |
| **Suivi des e-mails désactivé par défaut** | Environnement | Définit la valeur par défaut pour le suivi des ouvertures et des clics. Lorsqu’il est désactivé, le suivi est activé par défaut. Lorsqu’il est activé, le suivi est désactivé par défaut. |
| **Remplacer le suivi des ouvertures par défaut** et **Remplacer le suivi des clics par défaut** | Personne | Champs de personne booléens. Une valeur de `true` applique l’inverse de la valeur d’environnement par défaut pour ce type de suivi. Une valeur de `false` ou une valeur vide suit la valeur par défaut de l’environnement. |

Les champs de remplacement ne signifient pas « opt-in » ou « opt-out » par eux-mêmes. **`true`signifie toujours « l’opposé de la valeur par défaut de l’environnement ».**

### Table des décisions de tracking {#tracking-decision-table}

Marketo Engage applique cette décision séparément aux ouvertures d’e-mail et aux clics sur e-mail.

| Fonctionnalité | Environnement par défaut | Le remplacement de la personne est `false` ou vide. | Remplacement de la personne : `true` |
|---|---|---|---|
| Activé | Tracking sur par défaut | Suivi | Non activé |
| Activé | Suivi par défaut | Non activé | Suivi |
| Désactivé | Non applicable | Suivi normal ; le remplacement et la valeur par défaut sont ignorés | Suivi normal ; le remplacement et la valeur par défaut sont ignorés |

### Exemple {#example}

Supposons que la fonctionnalité soit activée et que la valeur par défaut de l’environnement soit activé pour le suivi. Une personne a **Remplacer la valeur par défaut du suivi des ouvertures** définie sur `true`, tandis que **Remplacer la valeur par défaut du suivi des clics** est vide. Marketo Engage ne suit pas les ouvertures d’e-mail de cette personne, mais il continue à suivre les clics sur ses e-mails.

## Choisir un modèle de tracking {#choose-a-tracking-model}

Choisissez le modèle qui correspond à vos exigences en matière de consentement et de confidentialité avant d’activer la fonctionnalité ou de renseigner les champs de personne.

| Modèle | Environnement par défaut | Définissez le remplacement sur `true` lorsque | Utilisation type |
|---|---|---|---|
| Désinscription (opt-out) | Tracking sur par défaut | Une personne s’oppose au suivi | Suivez la plupart des personnes, mais arrêtez le suivi des personnes qui s’y opposent. |
| Opt-in (consentement) | Suivi par défaut | Une personne donne son consentement au suivi. | Demander le consentement avant le suivi, y compris pour les destinataires couverts par les conseils CNIL ou Garante applicables. |

>[!CAUTION]
>
>Choisissez votre modèle avant de remplir les champs de remplacement et évitez de modifier la valeur par défaut de l’environnement par la suite. Comme `true` signifie « le contraire de la valeur par défaut », la modification de la valeur par défaut inverse l’effet de chaque valeur de remplacement existante. Par exemple, le fait de passer du suivi sur par défaut au suivi sur par défaut peut entraîner le suivi de personnes qui se sont précédemment opposées au suivi. Si vous devez modifier la valeur par défaut, mettez à jour les valeurs de remplacement pour toutes les personnes concernées avant que la modification ne prenne effet.

## Activer la fonctionnalité {#enable-the-feature}

Les remplacements du suivi des e-mails au niveau de la personne sont désactivés par défaut. Pour l’activer, contactez le service clientèle d’Adobe. Vous pouvez également indiquer si vous souhaitez que le statut par défaut de la fonctionnalité soit **Activé** ou **Désactivé** pour votre environnement Marketo.

>[!NOTE]
>
>Vous devez être un administrateur Marketo pour soumettre cette demande.

>[!TIP]
>
>Avant de demander à Adobe d’activer la fonctionnalité, renseignez les champs de remplacement pour les personnes existantes. Cela permet de s’assurer que le comportement de suivi prévu s’applique à partir du premier e-mail préparé après l’activation.

## Définir des valeurs de remplacement pour les personnes {#set-override-values-for-people}

Les champs de remplacement sont des champs de personne booléens. Définissez-les à l’aide de la méthode adaptée à votre workflow :

| Méthode | Notes |
|---|---|
| [Étape de flux Modifier la valeur de données](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value){target="_blank"} | Utilisez une campagne dynamique pour définir un champ lorsqu’une personne répond à vos critères, comme l’envoi d’une case à cocher de consentement sur un formulaire. |
| Formulaires | Mappez une case à cocher ou un champ masqué d’un formulaire Marketo Engage au champ de personne. |
| Import de liste | Insérez le champ sous forme d’une colonne dans le fichier d’importation. |
| API REST | Utilisez les noms de champ API `overrideOpenTrackingDefault` et `overrideClickTrackingDefault`. |

Définissez chaque champ en fonction du consentement de la personne. Si votre langue de consentement traite les ouvertures et les clics séparément, configurez chaque champ indépendamment.

## Changements dans l’e-mail {#what-changes-in-the-email}

Lorsque Marketo Engage ne suit pas une personne, il modifie le contenu de l’e-mail qu’il envoie à cette personne.

| Tracking désactivé pour | Changements | Ce qui fonctionne toujours |
|---|---|---|
| Ouvertures | L’e-mail n’inclut pas le pixel de suivi d’ouverture. Aucune activité **Ouvrir l&#39;e-mail** n&#39;est enregistrée. | Autres fonctionnalités de messagerie, notamment le suivi des clics, si elles restent activées. |
| Clics | Les liens vont directement à leurs destinations au lieu de passer par le domaine de suivi Marketo Engage. Le lien de suivi masqué n’est pas ajouté. Aucune activité **Cliquer sur l&#39;e-mail** n&#39;est enregistrée. | Les liens de désabonnement, le lien d&#39;opt-out du pied de page d&#39;e-mail, `list-unsubscribe` et les liens **Afficher en tant que page web** continuent de fonctionner. L’utilisation de ces liens n’enregistre pas d’activité **Cliquer sur l’e-mail**. |

## Quels emails sont affectés ? {#which-emails-are-affected}

| Type d’e-mail | Remplacements appliqués ? |
|---|---|
| E-mails par lots, tels que les e-mails envoyés à partir d’une campagne dynamique par lots ou d’un programme de messagerie | Oui |
| E-mails de déclenchement, tels que les e-mails envoyés à partir d’un déclencheur de campagne intelligente | Oui |
| E-mails avec tests A/B ou variantes championnes ou challenger | Oui. Le tracking est décidé séparément pour chaque personne, quelle que soit la variante qu&#39;elle reçoit. |
| Afficher en tant que page web | Oui. La version web suit les paramètres actuels de la personne. L’affichage d’une modification peut prendre jusqu’à une heure. |
| [E-mails opérationnels](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational){target="_blank"} | Non. Ils suivent le comportement normal de suivi. |
| Exemples d’e-mails (test) | Non. Ils suivent le comportement normal de suivi. |
| Prévisualisations des e-mails | Pas de changement. Les aperçus ne sont pas suivis. |
| E-mails d’alerte | Pas de changement. Les alertes ne sont pas suivies. |
| Messages SMS | Non. Cette fonctionnalité s’applique uniquement aux e-mails. |

## Lorsque Marketo Engage prend la décision de suivi {#when-marketo-engage-makes-the-tracking-decision}

Marketo Engage lit les valeurs de remplacement d’une personne lorsqu’il prépare l’e-mail à envoyer.

- **Diffusion planifiée ou différée :** Si un e-mail est préparé maintenant et envoyé ultérieurement (par exemple, avec [Démarrage anticipé](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs){target="_blank"} ou [Fuseau horaire du destinataire](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone){target="_blank"}), les valeurs au moment de la préparation s&#39;appliquent. Une modification apportée après la préparation ne modifie pas cet e-mail.
- **E-mails déjà diffusés :** La modification du remplacement d’une personne ne modifie pas les e-mails qu’elle a déjà reçus. Les clics sur les liens des e-mails précédemment envoyés peuvent toujours être suivis si ces liens ont été préparés avec le suivi activé.
- **Courriers électroniques futurs :** Une modification s’applique aux courriers électroniques que Marketo Engage prépare après la modification.

Si une personne retire son consentement, mettez à jour sa valeur de remplacement dès que possible afin que la modification s’applique à l’e-mail suivant préparé pour elle.

## Impact sur les rapports, les listes dynamiques et la notation {#impact-on-reporting-smart-lists-and-scoring}

Lorsque Marketo Engage ne suit pas une personne, il n’enregistre pas les activités **Ouvrir l’e-mail** ou **Cliquer sur l’e-mail**. Par conséquent :

- **Listes dynamiques/campagnes :** les filtres et les déclencheurs tels que **E-mail ouvert** et **Lien de clics dans l’e-mail** ne correspondent pas ou ne se déclenchent pas pour cette personne lorsque l’activité correspondante n’est pas suivie.
- **Rapports et tableaux de bord :** les taux d’ouverture des e-mails, les taux de clics et les performances des liens reflètent uniquement les personnes suivies. Les mesures d’engagement peuvent diminuer à mesure qu’un plus grand nombre de personnes ne sont pas suivies.
- **Notation et succès du programme :** les règles et les étapes de succès du programme basées sur les ouvertures ou les clics ne s’appliquent pas aux personnes dont les activités ne sont pas suivies. Revoyez ces règles afin que les personnes ne soient pas notées ou avancées injustement.
- **Association d’activité web :** Lorsque le suivi des clics est désactivé, les liens d’e-mail ne comportent pas de jeton de suivi Marketo Engage. Si la personne n’est pas déjà connue de Munchkin, la visite d’un site web à partir de cet e-mail n’est pas associée à la personne via le lien.

>[!NOTE]
>
>Les activités Envoyés, Diffusés, Rebonds et Désabonnés ne sont pas affectés.

## Fonctionnement avec d’autres paramètres de tracking {#how-this-works-with-other-tracking-settings}

Les remplacements du suivi des e-mails au niveau de la personne peuvent désactiver le suivi pour une personne. Il n’active pas le suivi lorsqu’un autre paramètre l’a déjà désactivé. Par exemple, les liens marqués de la classe `mktNoTrack` restent non suivis même si les paramètres de la personne autorisent le suivi des clics.

## Désactiver la fonctionnalité {#disable-the-feature}

Pour désactiver les remplacements du suivi des e-mails au niveau de la personne, contactez le service clientèle d’Adobe.

>[!NOTE]
>
>Vous devez être un administrateur Marketo pour soumettre cette demande.

Lors de la désactivation, les e-mails préparés après la modification reviennent au comportement normal de suivi. Les valeurs de remplacement restent dans les enregistrements de personne, mais sont ignorées. Si la fonction est activée à nouveau ultérieurement, les valeurs stockées s’appliquent à nouveau.

## Questions fréquentes {#frequently-asked-questions}

### Puis-je suivre les ouvertures mais pas les clics pour une personne, ou l’inverse ? {#can-i-track-opens-but-not-clicks-for-a-person-or-the-reverse}

Oui. Le suivi des ouvertures et des clics est décidé indépendamment. Définissez uniquement le champ de remplacement pour le type de suivi que vous souhaitez modifier.

### Cette fonctionnalité m’empêche-t-elle d’envoyer des e-mails à une personne ? {#does-this-feature-stop-me-from-sending-emails-to-a-person}

Non. Il contrôle uniquement le suivi. Pour arrêter l’envoi d’e-mails marketing à une personne, utilisez les fonctionnalités de désabonnement et de consentement existantes.

### Les personnes qui ne sont pas suivies voient-elles toujours des liens de désabonnement actifs ? {#do-people-who-are-not-tracked-still-see-working-unsubscribe-links}

Oui. Les liens de désabonnement et les liens **Afficher en tant que page web** continuent de fonctionner pour tout le monde.

### Pourquoi une personne qui s’est désabonnée possède-t-elle toujours une activité Cliquer sur l’e-mail ? {#why-does-a-person-who-opted-out-still-have-a-click-email-activity}

Il est probable qu’ils aient cliqué sur un lien dans un e-mail préparé avant la modification de leur valeur de remplacement. Les modifications s&#39;appliquent aux e-mails préparés après la modification.

### Dois-je modifier mes modèles d’e-mail ? {#do-i-need-to-change-my-email-templates}

Non. Marketo Engage applique la décision de tracking lors de la création de chaque e-mail. Vous n’avez pas besoin de modifier vos modèles ou vos e-mails.
