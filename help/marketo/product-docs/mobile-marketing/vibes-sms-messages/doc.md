---
description: Doc - Documents Marketo - Documentation du produit
title: Doc
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '836'
ht-degree: 1%

---

# Doc {#doc}

Texte

## Glossaire SMS de vidéos {#vibes-sms-glossary}

<table>
<thead>
  <tr>
    <th>Terme</th>
    <th>Définition</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Campagne d’acquisition</td>
    <td>Opération réalisée pour acquérir de nouveaux abonnés à vos listes d’abonnements. Un abonné peut être ajouté à une campagne d’acquisition par le biais d’un formulaire web Marketo ou d’un texto à un mot-clé.</td>
  </tr>
  <tr>
    <td>Gestionnaire de campagnes</td>
    <td>Sur la plateforme Vibes, le gestionnaire de campagnes est l’emplacement où vous pouvez configurer une liste d’abonnements et une campagne d’acquisition. Les utilisateurs disposant d’une licence de plateforme Vibes complète ont accès à des types de campagne supplémentaires.</td>
  </tr>
  <tr>
    <td>Clé d’entreprise</td>
    <td>company_key est un identifiant alphanumérique unique pour votre compte de plateforme. Si la plateforme Vibes comporte plusieurs comptes d’entreprise (tels que des comptes enfants), il se peut que vous ayez plusieurs clés de société. Chaque instance de Marketo Engage ne peut être mappée qu’à une seule clé_société Vibes.</td>
  </tr>
  <tr>
    <td>CTA (appel à l’action)</td>
    <td>Signal numérique ou physique ou script verbal destiné à l’acquisition d’abonnés dans un programme de SMS récurrent ou une liste d’abonnements. Peuvent être mises en ligne, sur les médias sociaux, dans les emails, dans les publications, etc.</td>
  </tr>
  <tr>
    <td>Domaine court personnalisé</td>
    <td>Si vous utilisez le réducteur de liens Vibes, l’URL abrégée apparaîtra, par défaut, sous l’URL abrégée Vibes : https://vbs.cm/xxxxxx. Un domaine court personnalisé est un domaine unique à votre marque. <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">En savoir plus sur les domaines courts personnalisés</a>.<p>
    Cela ne s'applique qu'aux messages envoyés depuis la plateforme Vibes, notamment les messages de la campagne d'acquisition et les messages par défaut à code court.<p>
    Le réducteur d’URL Marketo est recommandé pour que les données de clics soient contenues dans votre programme Marketo.</td>
  </tr>
  <tr>
    <td>Messages par défaut</td>
    <td>Messages obligatoires pour le numéro court afin de répondre à des demandes d’AIDE, d’arrêt et de message non reconnu.</td>
  </tr>
  <tr>
    <td>Se déconnecter</td>
    <td>Les déconnexions sont une forme d’exclusion en raison du numéro de mobile supprimé d’un réseau d’opérateur. Les raisons d'une déconnexion sont les suivantes : un compte a été complètement fermé, un compte prépayé a manqué de fonds ou le numéro a été retiré du réseau de téléphonie mobile pour d'autres raisons inconnues. Les numéros de téléphone mobile déconnectés et non transférés vers un autre opérateur de téléphonie mobile sont désabonnés de toutes les listes d'abonnements de la plateforme Vibes.</td>
  </tr>
  <tr>
    <td>Double Opt-in</td>
    <td>Méthode d’acquisition qui nécessite qu’un abonné potentiel confirme son consentement à être ajouté à une liste d’abonnements avec une commande de réponse, telle que "Y" ou son code postal. L’utilisation d’une invite de double opt-in peut vous aider à vous conformer aux directives des États et de la Confédération en matière de messagerie texte.</td>
  </tr>
  <tr>
    <td>Événement</td>
    <td>Un événement est une occurrence définie qui peut être envoyée à la plateforme Vibes et utilisée pour déclencher des actions déclenchées par l’API, y compris des envois de message. Chaque événement contient des données spécifiques à l’événement, y compris un type event_type, qui est utilisé pour déterminer la campagne de messages déclenchés par l’API à laquelle il correspond. L’API Event peut être déclenchée via Webhook dans Marketo Engage. En savoir plus sur notre <a href="https://developer-platform.vibes.com/reference/event-api">Référence de l’API d’événement</a>.</td>
  </tr>
  <tr>
    <td>Mot-clé</td>
    <td>Mot court ou chaîne alphanumérique envoyé par le consommateur au code court pour initier une expérience mobile.</td>
  </tr>
  <tr>
    <td>Code long (10DLC)</td>
    <td>Identifiant d’expéditeur à partir duquel des messages bidirectionnels sont envoyés entre la marque et le consommateur. Les codes longs américains sont composés de 10 chiffres.</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>Numéro d’annuaire mobile ou numéro de téléphone d’une personne. Les numéros de téléphone mobile et MDN ne sont pas des identifiants uniques dans Marketo.</td>
  </tr>
  <tr>
    <td>Base de données mobile</td>
    <td>La base de données mobile est la base de données dans laquelle Vibes stocke les données d’abonnés. Chaque abonné dispose d’un "enregistrement de personne" unique, dans lequel le numéro de mobile et les champs personnalisés associés sont renseignés.</td>
  </tr>
  <tr>
    <td>Participant</td>
    <td>Personne qui a une ou plusieurs interactions mobiles (telles que l’envoi d’un message texte) avec votre programme mobile, mais qui ne s’est pas inscrite à une liste d’abonnements.</td>
  </tr>
  <tr>
    <td>Enregistrement de personne</td>
    <td>Un enregistrement de personne est un ensemble de données pour un numéro de téléphone mobile spécifique. Chaque enregistrement de personne se voit également attribuer une clé person_key unique pour identification. Les Marketo ID sont liés à Vibes à l’aide du champ external_person_id. En savoir plus sur les enregistrements de personne dans <a href="https://developer-platform.vibes.com/reference/person-api">Documentation de l’API Vibes Person</a>.</td>
  </tr>
  <tr>
    <td>Numéro court</td>
    <td>Identifiant d’expéditeur à partir duquel des messages bidirectionnels sont envoyés entre la marque et le consommateur. Les numéros courts des Etats-Unis sont composés de 5 à 6 chiffres. Les numéros courts canadiens se composent de 4 à 6 chiffres. L’intégration de Marketo LaunchPoint à Vibes prend en charge un numéro court par instance.</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>Service de messages courts. Il s’agit d’un message qui ne contient que du texte.</td>
  </tr>
  <tr>
    <td>Listes d’abonnements</td>
    <td>Liste des numéros de téléphone mobile (et de leurs enregistrements de personne correspondants) qui ont fourni le consentement pour recevoir des messages récurrents de votre programme.</td>
  </tr>
  <tr>
    <td>Abonné</td>
    <td>Numéro mobile abonné à une ou plusieurs listes d’abonnements.</td>
  </tr>
  <tr>
    <td>Plateforme Vibes</td>
    <td>Le site web sur lequel vous vous connectez pour gérer vos campagnes. Accédez à <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> pour accéder à la plateforme Vibes.</td>
  </tr>
</tbody>
</table>

## Rapports SMS {#sms-reporting}

Texte

Cliquez sur SMS message local ressource > Afficher le tableau de bord ; rapports au niveau du message.

CAPTURE D’ÉCRAN

Progression des SMS : affiche le total envoyé et le total diffusé. Les montants sont à droite et si vous passez la souris sur la barre, le pourcentage est affiché.

CAPTURE D’ÉCRAN

Le graphique de synthèse affiche le taux de rebond calculé sous la forme d’un pourcentage. Passez la souris sur la barre supérieure pour afficher le taux de diffusion par montant et pourcentage. Passez la souris sur la section Taux de rebond orange de la barre pour afficher les montants et pourcentages Taux de rebond soft et Taux de rebond hard .

CAPTURE D’ÉCRAN

Le graphique Activité dans le temps vous permet de sélectionner Total envoyé ou Total diffusé. Sélectionnez une plage appropriée dans le sélecteur de période.

CAPTURE D’ÉCRAN
