---
description: Le programme de clonage duplique un programme Marketo existant dans un nouveau dossier portant un nouveau nom, préservant sa structure tout en vous permettant de personnaliser la nouvelle campagne.
title: Cloner le programme
badge: Beta
hide: true
source-git-commit: 1e70b9383bf3a1cd30715df4379d440c4efb1abd
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 1%

---

# Cloner le programme {#clone-program}

L’agent de programme Clone copie un programme opérationnel, y compris ses campagnes intelligentes, ses étapes de flux, ses ressources d’e-mail et sa configuration, à un nouvel emplacement de votre environnement Marketo.

>[!PREREQUISITES]
>
>* Pour utiliser cette fonctionnalité, vous devez d’abord accepter les termes [&#x200B; Core Gen-AI et les termes supplémentaires](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>
>* Vous devez disposer des autorisations nécessaires pour créer des programmes dans le dossier de destination.
>
>* Le programme source que vous souhaitez cloner doit déjà exister dans votre environnement Marketo.

>[!AVAILABILITY]
>
>Cette fonctionnalité est actuellement en version bêta fermée. Veuillez ne pas diffuser cette documentation.

## Utilisation {#how-to-use}

1. Dans Mon Marketo, cliquez sur la mosaïque **Marketo AI**.
1. Dans la fenêtre d’invite, saisissez vos instructions. Par exemple, « Clonez mon programme de webinaire du 2e trimestre dans le dossier Campagnes du 3e trimestre et nommez-le Webinaire de démonstration du produit du 3e trimestre ».
1. L’IA dédiée au Marketo confirme le programme source, le dossier de destination et le nouveau nom. Vérifiez et confirmez.
1. Le clone est créé. L’IA dédiée au Marketo vous confirme qu’elle a bien été effectuée et vous indique où la trouver.
1. Ouvrez le nouveau programme dans Marketo et mettez à jour les éléments différents : contenu des e-mails, dates, filtres d’audience, jetons, etc.
1. Exécutez l’agent [Program QA](/help/marketo/product-docs/marketo-ai/skills/validate-programs.md) avant l’activation.

## Cas d’utilisation {#use-cases}

**Réutilisation trimestrielle des campagnes** : un responsable de campagne lance la même série de webinaires chaque trimestre. Ils demandent à l’IA dédiée au Marketo de cloner le programme de webinaire du dernier trimestre dans le dossier du nouveau trimestre avec un nom mis à jour. Ils mettent ensuite à jour la copie de l’e-mail, les jetons de date du webinaire et le lien d’enregistrement, ce qui permet de gagner des heures de configuration.

**Création d’un modèle à partir d’un programme éprouvé** : un spécialiste des opérations marketing clone un programme de lancement de produit hautement performant dans un dossier « Modèles » pour servir de point de départ pour les lancements futurs. Le clone reste désactivé et est utilisé comme copie de référence.

**A/B test d’une nouvelle approche** : un responsable de campagne souhaite tester une cadence d’e-mail différente sans modifier un programme en cours d’exécution. Il clone le programme actif, modifie les étapes d’attente du clone et active les deux, en les exécutant sur différents segments d’audience pour comparer les résultats.

## Éléments à noter {#things-to-note}

* Les programmes clonés sont créés dans un état désactivé. Rien ne passe en ligne tant que vous n’avez pas activé les campagnes intelligentes.
* Les ressources d’e-mail dans le clone sont des copies et ne sont pas partagées avec l’original. Les modifications apportées aux e-mails du clone n’affecteront pas le programme source.
* Les jetons utilisés dans le programme source sont copiés dans le clone. Cependant, elles doivent toujours être mises à jour avec de nouvelles valeurs (dates, URL, noms d’événement).
* Les filtres de campagne intelligente du clone référencent les mêmes listes et champs que l’original. Examinez et mettez à jour le ciblage des audiences avant l’activation.
* Les ressources locales référençant d’autres programmes ou listes partagées sont copiées dans le clone. Ces références doivent être examinées avant l’activation.
