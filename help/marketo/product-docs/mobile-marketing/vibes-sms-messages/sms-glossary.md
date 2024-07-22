---
description: Glossaire SMS - Documents Marketo - Documentation du produit
title: Glossaire SMS
feature: Mobile Marketing
exl-id: 0c23ca9f-f994-42ae-bd72-7d37289b7a94
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Glossaire SMS {#sms-glossary}

Vous trouverez ci-dessous quelques termes courants que vous rencontrez lors de l’utilisation de SMS Vibes avec Marketo Engage.

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
    <td>Un événement est une occurrence définie qui peut être envoyée à la plateforme Vibes et utilisée pour déclencher des actions déclenchées par l’API, y compris des envois de message. Chaque événement contient des données spécifiques à l’événement, y compris un type event_type, qui est utilisé pour déterminer la campagne de messages déclenchés par l’API à laquelle il correspond. L’API Event peut être déclenchée via Webhook dans Marketo Engage. En savoir plus sur notre <a href="https://developer-platform.vibes.com/reference/event-api">référence d’API d’événement</a>.</td>
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
    <td>Un enregistrement de personne est un ensemble de données pour un numéro de téléphone mobile spécifique. Chaque enregistrement de personne se voit également attribuer une clé person_key unique pour identification. Les Marketo ID sont liés à Vibes à l’aide du champ external_person_id. Pour en savoir plus sur les enregistrements de personne, consultez la <a href="https://developer-platform.vibes.com/reference/person-api">documentation de l’API Vibes Person</a>.</td>
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
