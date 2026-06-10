---
description: Guide détaillé sur la création d’une campagne par e-mail dans CX Enterprise Coworker, de la rédaction d’invites à la révision et l’exportation de votre campagne.
title: Créer et générer des campagnes par e-mail
source-git-commit: b58edb707bf68aeed9f1b5eba8328c54a95c5a2f
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Créer et générer des campagnes par e-mail {#build-and-generate-email-campaigns}

Découvrez comment créer et examiner des campagnes par e-mail complètes en quelques minutes.

## Avant de commencer

Vérifiez que vous disposez des éléments suivants :

* Un compte CX Enterprise Coworker actif ([inscrivez-vous ici](https://coworker-essentials.experience.adobe.com/) si ce n&#39;est pas déjà fait).

* La configuration de votre marque sous **Vos affaires** > **Marques**.

* (Facultatif mais recommandé) Un modèle d’e-mail HTML téléchargé sous **Vos affaires** > **Modèles d’e-mail**.

* Un CSV d’audience prêt à être chargé.

* Une idée claire de l’objectif de votre campagne (par exemple, « reconquérir les clients obsolètes » ou « inviter des utilisateurs en évaluation à un webinaire »).

>[!TIP]
>
>Si vous êtes un débutant dans l’écriture d’invites pour les campagnes marketing, prenez deux minutes pour passer en revue _Inviter un collègue d’entreprise CX : bonnes pratiques_ avant de commencer.

## Étape 1 : démarrer une nouvelle conversation

Depuis la page d’accueil d’, vous pouvez commencer de trois façons :

* Saisissez une invite dans la barre d&#39;invite centrale.
* Sélectionnez un modèle de campagne prêt à l’emploi dans la section des modèles située sous la barre d’invite.
* Utilisez l&#39;option « m&#39;aider à m&#39;inviter » dans la liste déroulante de la barre d&#39;invite pour que CX Enterprise Coworker vous guide tout au long de la rédaction de votre invite.

[CAPTURE D’ÉCRAN : page d’accueil avec barre d’invite, ligne de modèle et option « m’aider à demander » mises en surbrillance]

[FOR KEITH : brève description de chaque option et quand l’utiliser. Recommandez des modèles pour les primo-accédants, des invites à structure libre pour les marketeurs qui savent ce qu&#39;ils veulent et « aidez-moi à m&#39;inviter » pour toute personne entre les deux.]

## Étape 2 : Rédiger votre invite

Une forte invite de collaborateur d’entreprise CX inclut :

* L’objectif de la campagne (ce que vous essayez d’atteindre).
* L’audience (son destinataire ou l’origine des données de l’audience).
* Le format et la structure (nombre d’e-mails, cadence, tonalité).
* Repères de marque ou de contexte (références à votre marque, produit ou campagne).

Exemple :

```
"Create a win-back email series for customers who bought last year but haven't returned. Use the CSV I uploaded. Include 2–3 emails that feel seasonal and remind them to shop again."
```

[FOR KEITH : peut ajouter 2 à 3 exemples rapides supplémentaires couvrant B2B et B2C pour donner de la variété. Extrayez des cas d’utilisation de notre document de collection à des fins de cohérence.]

[CAPTURE D’ÉCRAN : barre d’invite avec exemple d’invite saisie]

## Étape 3 : charger votre audience

[FOR KEITH : présentation du chargement CSV. Couverture : emplacement du bouton de chargement dans l’interface utilisateur. - Colonnes obligatoires et attentes en matière de format. - Champs de personnalisation que CX Enterprise Coworker peut utiliser (prénom, date de dernière commande, catégorie de produit, etc.). - Lien vers l’exemple de fichier CSV. - Que se passe-t-il si les données sont désordonnées ou si les champs sont manquants ]

[CAPTURE D’ÉCRAN : flux de chargement CSV]

>[!TIP]
>
>Excluez les contacts que vous ne souhaitez pas envoyer par e-mail (utilisateurs désabonnés, adresses internes, comptes de test) avant le chargement. Bien que nous activerons progressivement la fonctionnalité pour « exclure » des utilisateurs spécifiques ou « ajouter des attributs » au cours de l’essai, elle n’est pas immédiatement disponible à partir de la date de lancement.

## Étape 4 : Ajouter un résumé et des documents de référence

[FOR KEITH : expliquez comment joindre un résumé, des documents de référence de marque ou un autre contexte. Couverture : - Types de fichiers pris en charge. - Comment CX Enterprise Coworker utilise ces informations (extraites dans le contexte de l&#39;invite, appliquées à la génération de contenu, etc.) - Limites de taille de fichier, le cas échéant

Voici une analyse approfondie de ma session au Summit, où je passe en revue ce qui suit : https://business.adobe.com/summit/2026/sessions/3-2-1-launch-project-halo-revealed-s232.html\
Limites - Je peux vous mettre en relation avec l&#39;engg - Neha Pullabhotla, qui pourra nous aider sur les détails ici. ]

[CAPTURE D’ÉCRAN : interface utilisateur de pièce jointe de résumé/référence]

## Etape 5 : générer la campagne

Cliquez sur **Générer la campagne**. Le collaborateur d’entreprise CX :

* Générez un plan de campagne structuré.
* Demandez votre audience cible, qui sera également utilisée pour la personnalisation du contenu.
* Rédiger un contenu d’e-mail personnalisé pour chaque étape.
* Créez le parcours de manière dynamique en cours de route.
* Regroupez tous les éléments sur un seul tableau de campagne.

[FOR KEITH : description de l’apparence du tableau de campagne et de son contenu. Couvrez la vue en plan, la vue en parcours et la vue de contenu. Notez la durée habituelle de la génération, qui dépend du nombre de points de contact dans leur parcours. Rappelez-vous que lorsqu’ils ouvrent un éditeur pour le workflow ou pour l’e-mail, leur conversation leur montre ceci afin qu’ils soient dans le contexte du composant spécifique. Expliquez également comment l’éditeur d’e-mail est un éditeur d’e-mail de type pointer-cliquer, avec la limitation qu’il n’est pas destiné à être un concepteur à part entière. Les utilisateurs peuvent modifier des images dans Adobe Express ou même se connecter à Google Drive ou à AEM Assets à l’aide d’Adobe Express. Toutes leurs ressources d’image sont stockées dans Express. Ils regénèrent les images dans notre éditeur d’e-mail avec Firefly en ligne ou les remplacent par une image locale à partir de leur ordinateur. Il peut changer de modèle HTML et générer de nouveau du contenu, puis s’envoyer un « e-mail de test » pour valider ce que le client final recevra]

[CAPTURE D’ÉCRAN : panorama de campagne généré avec plan, parcours et contenu visibles]

## Étape 6 : examiner et affiner

L&#39;interface conversationnelle rend le raffinement simple. Pour apporter des modifications, adressez-vous à un collègue d’entreprise CX :

* « Rendre l’objet de l’e-mail 2 plus urgent. »
* « Raccourcissez la copie du corps dans tous les e-mails. »
* « Échangez l’audience vers des clients de la région Ouest uniquement. »
* « Ajoutez un quatrième e-mail avec un CTA plus puissant. »
* « Remplacez l’attente de 3 jours par 5 jours. »

[FOR KEITH : Découvrir comment apporter des modifications par chat et par édition directe. Expliquez comment les artefacts sont mis à jour. Mentionnez qu’il n’existe aucune possibilité d’ajouter d’autres nœuds au workflow via l’éditeur, et qu’il n’existe actuellement aucun contrôle de version. Pour de meilleurs résultats, nous les encourageons également à demander toute modification de leur workflow global dès le début de la création de leur plan]

[CAPTURE D’ÉCRAN : amélioration de la conversation en action — afficher un avant et un après d’un e-mail après une demande de conversation]

## Étape 7 : envoyer un BAT par e-mail

Avant le lancement, envoyez la campagne à vous-même ou à un membre de votre équipe pour l’examiner dans une véritable boîte de réception.

[FOR KEITH : procédure d’envoi du BAT. Couverture : - Emplacement du bouton du BAT. - Qui peut recevoir des BAT (actuellement uniquement l’utilisateur connecté) - Si tous les e-mails du parcours sont envoyés, ou un par un (actuellement uniquement un à la fois, sauf si l’utilisateur indique « BAT cette série » dans le chat. - Éléments à vérifier dans le BAT (rendu, liens, jetons de personnalisation, pied de page de désabonnement).]

[CAPTURE D’ÉCRAN : envoyer le flux de BAT]

## Étape 8 : Lancement ou exportation

Lorsque vous êtes satisfait(e) de la campagne, vous disposez de quelques options :

>[!NOTE]
>Launch n’est actuellement pas disponible à la version, mais sera activé dans les deux semaines suivant la version initiale, en attendant l’approbation de la loi.

* Lancez la campagne.
* Exportez des e-mails individuels en tant qu’HTML.
* Exportez l’intégralité de la campagne sous la forme d’un document Word ou PDF pour révision par l’équipe.

[FOR KEITH : détails sur chaque option et vérifications avant le lancement de l’exécution de CX Enterprise Coworker (conformité, liens rompus, champs de personnalisation manquants, etc.).]

[CAPTURE D’ÉCRAN : options de lancement/d’exportation]

## Questions courantes

[FOR KEITH : 4-6 FAQ basées sur les premiers commentaires des utilisateurs. Suggestions de démarrage - pour discuter avec notre équipe Eng :
* « Pourquoi la première réponse prend-elle autant de temps ?
* « Et si la sortie de CX Enterprise Coworker n&#39;est pas tout à fait correcte ? »
* « Puis-je modifier les e-mails directement ou uniquement par chat ? »
* « Comment enregistrer une campagne sans la lancer ? »
* « Que se passe-t-il si mon fichier CSV d’audience comporte des erreurs ? »
* « Puis-je dupliquer ou remixer une campagne ? »
* « Comment partager un brouillon de campagne avec un coéquipier pour révision ? »]
