---
solution: Marketo Engage
product: marketo
title: Test du rendu des e-mails avec Litmus
description: Les utilisateurs de Marketo Engage peuvent intégrer leur compte Litmus pour tester facilement le rendu de contenu dans divers clients de messagerie.
level: Beginner, Intermediate
feature: Email Designer
exl-id: ccef36af-362a-4ac0-9030-492e9d7f10b5
source-git-commit: 3a71e0f0da0f6201ccda73a0c8bd5b94864308c0
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 2%

---

# Test du rendu des e-mails avec Litmus {#test-email-rendering-with-litmus}

Tirez parti de votre compte [Litmus](https://www.litmus.com/email-testing) dans Marketo Engage pour voir instantanément comment vos e-mails sont rendus dans les clients de messagerie populaires.

>[!AVAILABILITY]
>
>Cette fonctionnalité est disponible pour tous les utilisateurs de Marketo Engage qui disposent d’un compte Litmus actif.

## Utilisateurs Entreprise Litmus {#litmus-enterprise}

Les étapes suivantes s&#39;adressent aux utilisateurs du [Plan d&#39;entreprise Litmus](https://www.litmus.com/pricing/enterprise){target="_blank"}.

1. Sur l’écran _Modifier le contenu de l’e-mail_, cliquez sur le bouton **Simuler du contenu**.

   ![](assets/test-email-rendering-with-litmus-1.png)

1. Sélectionnez le destinataire du test et cliquez sur le bouton **Rendu de l’e-mail**.

   ![](assets/test-email-rendering-with-litmus-2.png){width="800" zoomable="yes"}

1. Si ce n&#39;est pas déjà fait, **connectez votre compte Litmus**. Si vous l’avez déjà fait, passez à l’étape 6.

   ![](assets/test-email-rendering-with-litmus-3.png){width="800" zoomable="yes"}

1. Saisissez vos identifiants Litmus et cliquez sur **Se connecter**.

   >[!IMPORTANT]
   >
   >Lors de la connexion de votre compte Litmus à Marketo Engage, vous acceptez que les e-mails de test soient envoyés à Litmus. Après l’envoi, ces e-mails de test ne sont plus gérés par Adobe. Ainsi, la politique e-mail de rétention des données de Litmus s’applique à ces e-mails, y compris les données de personnalisation qui peuvent y être incluses.

1. Cliquez sur **Connexion** pour terminer l’intégration.

   ![](assets/test-email-rendering-with-litmus-4.png)

1. Cliquez sur le bouton **Exécuter le test** pour générer des prévisualisations d&#39;e-mail.

1. Découvrez à quoi ressemble votre contenu dans les principaux clients de messagerie de bureau, mobiles et web. Cliquez sur autant de miniatures que vous le souhaitez pour l’aperçu.

   ![](assets/test-email-rendering-with-litmus-5.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Découvrez comment [personnaliser votre liste de clients de messagerie par défaut](https://help.litmus.com/article/227-change-your-default-email-clients-list).

1. Une fois le test terminé, cliquez sur la flèche vers l’arrière dans le coin supérieur gauche pour revenir à l’écran _Simuler du contenu_.

   ![](assets/test-email-rendering-with-litmus-6.png)

**ÉTAPE FACULTATIVE** : Si vous décidez d&#39;apporter des modifications à votre e-mail, après avoir cliqué sur **Rendu de l&#39;e-mail** pour les afficher, veillez également à cliquer sur le bouton **Retester** dans le coin supérieur droit de l&#39;écran Litmus _Prévisualisations d&#39;e-mail_.

![](assets/test-email-rendering-with-litmus-7.png)

## Utilisateurs principaux de Litmus {#litmus-core}

Les étapes suivantes s&#39;adressent aux utilisateurs du [Plan principal Litmus](https://www.litmus.com/pricing/){target="_blank"}.

1. Dans votre compte Litmus, récupérez l’adresse e-mail de test en cliquant sur le bouton **Copier l’adresse de test** dans l’écran _Tester_.

   ![](assets/test-email-rendering-with-litmus-8.png){width="800" zoomable="yes"}

1. Dans Marketo Engage, accédez à l’écran _Modifier le contenu de l’e-mail_ de l’e-mail souhaité, puis cliquez sur le bouton **Simuler le contenu**.

   ![](assets/test-email-rendering-with-litmus-9.png){width="600" zoomable="yes"}

1. Sélectionnez vos destinataires de test et cliquez sur le bouton **Envoyer un BAT**.

   ![](assets/test-email-rendering-with-litmus-10.png){width="800" zoomable="yes"}

1. Saisissez l’adresse e-mail Litmus que vous avez copiée à l’étape 1 et cliquez de nouveau sur **Envoyer le BAT**.

   ![](assets/test-email-rendering-with-litmus-11.png)

1. Vérifiez l&#39;e-mail dans votre compte Litmus (dans le dossier correspondant à l&#39;adresse e-mail que vous avez copiée à partir de Litmus).

   ![](assets/test-email-rendering-with-litmus-12.png){width="800" zoomable="yes"}
