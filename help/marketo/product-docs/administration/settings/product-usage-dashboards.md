---
description: Tableaux de bord d’utilisation du produit - Documents Marketo - Documentation du produit
title: Tableaux de bord d’utilisation du produit
hide: true
hidefromtoc: true
feature: Administration
source-git-commit: f3bc58c0d65e8110c5366269fdb4abf817370aee
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Tableaux de bord d’utilisation du produit {#product-usage-dashboards}

Les tableaux de bord d’utilisation des produits Marketo Engage permettent d’afficher l’utilisation des produits et des plateformes par rapport à certaines limites ou à la liste d’attente de débit des données, l’utilisation par rapport au quota quotidien et les mesures clés d’un abonnement. L’infrastructure est allouée afin de fournir des limites de performances définies pour les niveaux de produit pour des attributs spécifiques. Certaines de ces limites, comme l’utilisation des API, sont des limites souscrites dans le cadre de votre package ou de votre niveau de produit.

## Accès {#how-to-access}

1. Dans Marketo Engage, cliquez sur **Admin**.

   ![](assets/product-usage-dashboards-1.png)

1. Dans l’arborescence de gauche, faites défiler l’écran vers le bas et sélectionnez **Tableaux de bord d’utilisation du produit**.

   ![](assets/product-usage-dashboards-2.png)

## Tableau de bord d’utilisation des activités {#activity-usage-dashboard}

### Activités Hebdomadaires Moyennes {#average-weekly-activities}

Le tableau de bord Utilisation hebdomadaire des activités fournit un décompte hebdomadaire des types d’activités sur une période mobile de 52 semaines. Les activités hebdomadaires produites sont un bon indicateur de l’ampleur du marketing que vous effectuez dans Marketo Engage. Les activités servent de proxy pour les différents processus système et événements pouvant faire l’objet d’un suivi dans Marketo.

Les types d’activités incluent à la fois le nombre d’activités capturées lorsque des personnes interagissent avec des événements marketing, ainsi que les activités système déclenchées par des actions de flux. Voici quelques exemples d’activités initiées par une personne : lorsqu’une personne ouvre un e-mail ou clique sur un lien dans un e-mail. Un exemple d’activités système déclenchées par une action de flux est « Envoyer à SFDC » lorsque le déclencheur est lancé. Pour afficher le nombre de types d’activités pour une semaine particulière, passez la souris sur une semaine et consultez le nombre.

![](assets/product-usage-dashboards-3.png){width="800" zoomable="yes"}

#### Questions fréquentes {#faq}

**Quels types d’activités sont comptabilisés ?**

Cela dépend des activités qui sont incluses dans le pipeline.

**L’activité lead/personne connue et anonyme est-elle incluse ?**

Uniquement des personnes/prospects connus.

**À quelle fréquence les données sont-elles actualisées ?**

Le décompte des activités est actualisé tous les matins.

## Répartition des activités {#activity-breakdown}

Ici, nous obtenons le décompte des activités au cours des sept jours précédents en fonction de tranches significatives des données. Regroupez les activités selon les types d’activités les plus courants observés au cours des sept derniers jours. Cela peut inclure des catégories telles que « Modifier la valeur des données », « Ajouter à la liste » ou « Envoyer un e-mail ». Vous pouvez ainsi voir quels types d’activités se produisent le plus souvent dans le système. L’utilisation du type d’activité est un indicateur clé pour déterminer la croissance ou si des optimisations sont nécessaires pour réduire l’utilisation.

>[!NOTE]
>
>* Toutes les répartitions ci-dessous sont une somme « mobile de sept jours » et n’incluent **** le jour en cours. Pensez donc à « hier + six jours avant ».
>
>* Le tableau de bord n’affiche que les 20 principaux types d’activité, les autres étant triés dans une catégorie intitulée « Autre ».

![](assets/product-usage-dashboards-4.png){width="800" zoomable="yes"}

L’utilisation des activités est un indicateur clé de la quantité de marketing réalisée et permet de visualiser la croissance par rapport au niveau identifié pour le niveau de produit pour lequel un contrat a été conclu. Les tableaux de bord peuvent également être utilisés comme guide pour déterminer le niveau d’optimisation qui peut/doit être réalisé en réduisant le nombre de champs mis à jour.

### Par type {#by-type}

Regroupez les activités selon les types d’activités les plus courants observés au cours des sept derniers jours. Cela peut inclure des catégories telles que _Modifier la valeur des données_, _Ajouter à la liste_ ou _Envoyer un e-mail_. Vous pouvez ainsi identifier les types d’activités qui se produisent le plus souvent dans Marketo Engage.

### Par Attribut Modifier La Valeur Des Données {#by-change-data-value-attribute}

_Modifier la valeur des données_ est le type d’activité le plus courant. Indique le moment où une information sur un enregistrement de personne/prospect est mise à jour. Ici, nous regroupons les données par champs qui sont modifiés le plus souvent afin que vous puissiez déterminer si les informations sont utiles à vos opérations marketing, s’il existe des opportunités d’optimiser l’utilisation de la plateforme, etc.

### Par campagne {#by-campaign}

Groupe par lequel les campagnes produisent le plus d’activités. Insight pourra ainsi voir si des campagnes particulièrement « bruyantes » génèrent plus d’activité que nécessaire. Découvrez rapidement les campagnes qui doivent être désactivées ou celles qui font plus de travail que prévu.

### Par Source (BIENTÔT DISPONIBLE) {#by-source}

Regroupez par source des activités (_Synchronisation CRM_, _Action de flux de campagne_, _Chargement d’API_, _Remplissage de formulaire de page de destination_, etc.). Cela vous permet de comprendre si la plupart de vos activités sont générées par des actions marketing, des synchronisations CRM ou par les personnes/prospects eux-mêmes.
