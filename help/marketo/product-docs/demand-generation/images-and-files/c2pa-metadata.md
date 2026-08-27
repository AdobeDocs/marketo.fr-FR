---
description: Découvrez comment les métadonnées C2PA sont automatiquement associées à des images générées par l’IA dans Marketo Engage, conservées par le biais de modifications et utilisées pour la provenance du contenu.
title: Métadonnées C2PA dans Marketo Engage
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 10781cbfd51019a2e4af346803a2e35ef40855d0
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 2%

---

# Métadonnées C2PA dans Marketo Engage

De nouvelles lois émergent autour de la transparence générative de l’IA, et Adobe s’efforce de répondre aux exigences applicables dans toutes les juridictions. Les métadonnées C2PA sont l’outil de provenance utilisé par Adobe pour répondre aux exigences de ces lois.

Les métadonnées C2PA sont des métadonnées durables et invisibles qui enregistrent la manière dont un élément de contenu a été créé ou modifié. Lorsque vous générez ou modifiez une image à l’aide d’outils d’IA génératifs dans Marketo Engage, des métadonnées C2PA sont automatiquement associées à cette image (aucune action n’est requise de votre part). Il s’agit d’informations chiffrées et infalsifiables qui peuvent aider les visiteurs et les visiteuses à comprendre la traçabilité du contenu et à assurer l’intégrité des ressources de la marque. Ces informations incluent :

* **Émetteur ou signataire** : informations sur l’entité ou la société qui a émis la signature numérique pour certifier ou signer la ressource.
* **Date de l’événement** : date à laquelle les métadonnées C2PA ont été appliquées à la ressource.
* **Crédit et utilisation** : informations sur le producteur de la ressource, y compris le nom, les identifiants de médias sociaux ou d’autres informations relatives à l’identité.
* **Processus** : enregistrements des modifications apportées à la ressource.
* **Détails de l’appareil** : informations sur l’application ou l’appareil utilisé pour créer ou modifier la ressource.
* **Outil d’IA utilisé** : si l’IA générative a été utilisée pour créer la ressource, le nom du modèle utilisé peut être inclus.
* **Autres informations pertinentes** : des données supplémentaires sont également incluses pour offrir plus de contexte sur l’historique d’une ressource.

## Actions qui joignent des métadonnées C2PA

Le tableau suivant résume le moment où des métadonnées C2PA sont jointes, en fonction de l’action d’image effectuée dans la génération d’images dans Marketo Engage.

| Action | Description | Métadonnées C2PA jointes ? | Exemple de cas d’utilisation |
|---|---|---|---|
| **Utiliser l’outil ’Générer l’image’** | Créez une image à partir d’une invite de texte ou d’une image de référence, ou générez une image similaire. | Toujours. L’image est générée par l’IA générative, elle transfère donc toujours de nouvelles métadonnées C2PA. | Une image de bannière pour une campagne par e-mail est générée à partir d’une invite de texte décrivant le visuel souhaité. |
| **Recadrer une image** | Ajustez une image aux dimensions demandées. | Uniquement si l’image source possédait déjà des métadonnées C2PA. Le recadrage recrée les pixels de l’image, ce qui effacerait normalement ces métadonnées C2PA. Marketo Engage les lit donc à partir de l’image source avant de les recadrer, puis les reconstruit et les relie au résultat recadré. Le recadrage lui-même n&#39;ajoute pas une nouvelle action générative de l&#39;IA : il préserve celle qui existe. | Une image de bannière générée est recadrée pour s’adapter à une page web : les métadonnées C2PA sont conservées par le recadrage. Une photo de catalogue téléchargée utilisée comme arrière-plan de notification push est recadrée pour s’adapter à l’écran : étant donné que la photo de catalogue ne comporte aucune action d’IA générative, aucune métadonnée C2PA n’est créée. |
| **Ajouter une superposition de texte** | Effectuez le rendu du texte généré sur une image d’arrière-plan. | Uniquement si l’image d’arrière-plan contenait déjà des métadonnées C2PA. Le rendu du recouvrement génère une nouvelle image à partir de l’arrière-plan plus le texte, ce qui effacerait normalement ces métadonnées C2PA. Marketo Engage les lit donc au préalable à partir de l’image d’arrière-plan, puis les recrée et les relie au résultat. L’étape de recouvrement n’ajoute pas de nouvelle action d’IA générative. | Un titre promotionnel est rendu sous la forme d’une superposition de texte sur une image d’arrière-plan générée pour une page de destination : les métadonnées C2PA de l’image d’arrière-plan sont conservées. |

## Types de contenu et leur portée

**Images** : Couvert. Les métadonnées C2PA sont jointes lorsque les images sont générées avec l’IA générative et conservées par le biais d’opérations de recadrage et de superposition de texte effectuées par la génération d’images dans Marketo Engage.

**Texte** : sans objet. Les sorties textuelles de la génération d’images dans Marketo Engage, telles que la génération de copies, la traduction et les suggestions d’alignement de marque, ne nécessitent pas de métadonnées C2PA.

## Ce qui se passe lorsque le contenu est déplacé

Marketo Engage conserve les métadonnées C2PA associées aux ressources d’images prises en charge. Si une image contient des métadonnées C2PA lors de son importation dans Marketo Engage, les métadonnées sont conservées lorsque la ressource est utilisée dans du contenu de campagne généré et des expériences d’e-mail sortant.

## Ressources supplémentaires

* [Transparence du contenu d’IA générative](https://experienceleague.adobe.com/fr/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency){target="_blank"}
* [Consignes d’utilisation de l’IA générative d’Adobe Experience Cloud](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}
* [Mécanismes de sécurisation et limitations](https://experienceleague.adobe.com/fr/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails){target="_blank"}
