---
solution: Marketo Engage
product: marketo
title: Importation de modèles
description: Découvrez comment importer vos modèles d’e-mail existants à partir de l’éditeur classique dans le nouveau Designer d’e-mail.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: f5f5e256631b09937d97d7b70f9475f2c286676d
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 1%

---

# Importation de modèles {#template-import}

Importez facilement vos modèles d’e-mail existants à partir de l’éditeur classique dans le nouveau Designer d’e-mail, en préservant vos conceptions et en accélérant la création de modèles avec des structures familières et réutilisables.

1. Accédez au **Design Studio**.

   CAPTURE D’ÉCRAN

1. Cliquez sur **Modèles d’e-mail** puis sélectionnez **Modèles d’e-mail (nouveau)**.

   CAPTURE D’ÉCRAN

1. Cliquez sur **Créer un modèle**.

   CAPTURE D’ÉCRAN

1. Saisissez un _Nom_ et (facultatif) un _Description_.

   CAPTURE D’ÉCRAN

1. Cliquez sur les **Modèles Marketo** puis choisissez les Modèles existants créés dans l’éditeur d’e-mail classique.

   CAPTURE D’ÉCRAN

   >[!NOTE]
   >
   >Seuls les modèles approuvés et les modèles qui ont été partagés avec l&#39;espace de travail actuel peuvent être importés.

1. Sélectionnez le modèle souhaité.

   CAPTURE D’ÉCRAN

1. Cliquez sur Utiliser ce modèle.

   CAPTURE D’ÉCRAN

1. Le modèle importé s’ouvre dans le Designer d’e-mail.

1. Passez en revue les composants pour une conversion correcte et effectuez les ajustements souhaités à l’aide du Designer. Lorsque vous êtes satisfait(e) du modèle, approuvez-le pour une utilisation dans les e-mails.

## Créer des fragments {#create-fragments}

Il est conseillé de créer des fragments de sections répétables en vue d&#39;une utilisation ultérieure.

1. Cliquez sur le bouton **...Plus** en haut et sélectionnez **Enregistrer en tant que fragment**.

   CAPTURE D’ÉCRAN

1. Sélectionnez un composant ou une structure, puis cliquez sur **Créer**.

   CAPTURE D’ÉCRAN

1. Saisissez un nom (et une description facultative) et cliquez sur **Enregistrer**.

   CAPTURE D’ÉCRAN

## Bonnes pratiques {#best-practices}

* Comme le style libre d’HTML peut varier considérablement, l’importateur peut ne pas toujours interpréter tous les composants parfaitement. Vérifiez les modèles importés pour vous assurer que toutes les sections sont modifiables et correctement mappées. Si un article n&#39;est pas sélectionnable, recréez simplement cette section pour obtenir les meilleurs résultats.

* Après l’importation, vous pouvez enregistrer des sections réutilisables en tant que fragments et les approuver pour qu’elles soient utilisées par les auteurs d’e-mails. Appliquez des thèmes de marque pour maintenir la cohérence et la conformité.

* Vous pouvez continuer à utiliser les scripts Velocity et envisager de réimplémenter d’anciens fragments de code à l’aide d’une combinaison de fragments et de contenu conditionnel pour une flexibilité et un contrôle améliorés.

<table><thead>
  <tr>
    <th>Limite</th>
    <th>Motif</th>
    <th>Remède</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Les variables définies dans l’éditeur d’e-mail classique ne sont pas disponibles au niveau de l’e-mail.</td>
    <td>À l’origine, les variables étaient conçues pour simplifier la modification des e-mails lorsque l’éditeur ne proposait pas encore de fonctionnalités WYSIWYG. Dans le Designer d’e-mail, les utilisateurs et utilisatrices peuvent bénéficier d’une flexibilité similaire grâce aux commandes disponibles. L’importateur conserve la structure et les composants de votre modèle existant, ce qui vous permet de le recréer efficacement dans le Designer d’e-mail.</td>
    <td>Les utilisateurs doivent pouvoir effectuer cette opération dans le Designer. <p>
    Pour les modules , vous pouvez enregistrer différents segments en tant que fragments. Les fragments approuvés pourront être utilisés au niveau de l’e-mail.</td>
  </tr>
  <tr>
    <td>Si l’HTML source contient des blocs imbriqués, les calques les plus profonds ne sont pas adressables dans le Designer.</td>
    <td>Le Designer d’e-mail ne prend pas en charge les commentaires imbriqués.</td>
    <td>Même si le Designer ne permet pas la modification des structures imbriquées, il doit s’afficher avec précision. Veillez d’abord à tester le modèle.<p>
    Recréez la structure à l’aide de la grille .</td>
  </tr>
  <tr>
    <td>Parfois, les boutons sont importés sous la forme de simples conteneurs contenant du texte.</td>
    <td>Certains styles d’implémentation utilisant HTML peuvent être mal interprétés lors de l’importation.</td>
    <td>Recréez le bouton dans le Designer.</td>
  </tr>
  <tr>
    <td>Les boutons peuvent parfois être surdimensionnés.</td>
    <td>Conflit entre le CSS de l’e-mail Marketo et d’autres éléments de niveau inférieur (<code>&lt;span&gt;</code>)</td>
    <td>Essayez d’ajuster les marges et les marges intérieures du bouton dans le Designer.</td>
  </tr>
  <tr>
    <td>Les puces ne sont pas prises en charge de manière native.</td>
    <td>Le Designer d’e-mail ne propose pas de puces pour le moment.</td>
    <td>Envisagez de réimplémenter les puces à l’aide de techniques alternatives.</td>
  </tr>
  <tr>
    <td>L’alignement vertical est déformé lorsque le contenu du conteneur ne respecte pas la valeur d’attribut valign.</td>
    <td><code>valign</code> ne fonctionne pas dans les conteneurs définis dans le modèle.</td>
    <td>Essayez d’ajuster les marges et les marges intérieures du bouton dans le Designer Email.</td>
  </tr>
  <tr>
    <td>Les jetons Personalization au niveau du programme (mes jetons) au niveau du modèle peuvent entraîner des erreurs de validation.</td>
    <td>Les modèles d’e-mail ne prennent pas en charge les jetons au niveau du programme.</td>
    <td>Remplacez-les par d’autres types de jetons dans les modèles, puis remplacez-les par Mes jetons dans les e-mails individuels.</td>
  </tr>
  <tr>
    <td>Les composants du séparateur ne peuvent pas être sélectionnés.</td>
    <td>Les composants de séparateur ne sont pas couverts dans la version.</td>
    <td>s/o</td>
  </tr>
  <tr>
    <td>Si l’HTML d’origine comporte des structures incorrectes, elles sont susceptibles d’être conservées.</td>
    <td>Problèmes avec l’HTML d’origine.</td>
    <td>Les problèmes doivent être résolus avant l’importation.</td>
  </tr>
  <tr>
    <td>Pour le contenu importé, l’utilisation de l’aperçu du contenu n’est pas un indicateur fiable.</td>
    <td>La fonction d’aperçu Designer ne prend pas en charge les HTML personnalisées.</td>
    <td>Il est recommandé de tester votre e-mail à l’aide de l’option <b> Envoyer un BAT </b> dans l’écran <i> Simuler du contenu </i>.</td>
  </tr>
  <tr>
    <td>Les fragments de code de l’ancien modèle ne fonctionnent pas dans le Designer d’e-mail.</td>
    <td>Le Designer d’e-mail ne prend pas en charge les fragments de code.</td>
    <td>Réimplémentez vos fragments de code en tant que fragments de code associés à du contenu conditionnel.</td>
  </tr>
</tbody></table>
