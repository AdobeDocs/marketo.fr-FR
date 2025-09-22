---
description: Glossaire SMS - Documents Marketo - Documentation du produit
title: Glossaire des SMS
feature: Mobile Marketing
exl-id: 0c23ca9f-f994-42ae-bd72-7d37289b7a94
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 1%

---

# Glossaire des SMS {#sms-glossary}

Vous trouverez ci-dessous quelques termes courants que vous rencontrerez lors de l’utilisation de SMS Vibes avec Marketo Engage.

<table>
<thead>
  <tr>
    <th>Terme</th>
    <th>Définition</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Campagne D’Acquisition</td>
    <td>Une campagne effectuée pour acquérir de nouveaux abonnés à vos listes d’abonnements. Un abonné peut être ajouté à une campagne d’acquisition par le biais d’un formulaire web Marketo ou en envoyant un SMS à un mot-clé.</td>
  </tr>
  <tr>
    <td>Responsable de campagne</td>
    <td>Sur la plateforme Vibes, Campaign Manager permet de configurer une liste d’abonnements et une campagne d’acquisition. Les utilisateurs disposant d’une licence de plateforme Vibes complète ont accès à d’autres types de campagne.</td>
  </tr>
  <tr>
    <td>Clé d’entreprise</td>
    <td>company_key est un identifiant alphanumérique unique pour votre compte platform. Si la plateforme Vibes comporte plusieurs comptes de société (tels que des comptes enfants), vous pouvez avoir plusieurs clés_société. Chaque instance de Marketo Engage ne peut être mappée qu’à une seule company_key Vibes.</td>
  </tr>
  <tr>
    <td>CTA (call to action)</td>
    <td>Signalétique numérique ou physique ou script verbal pour l'acquisition d'abonnés dans un programme de messages texte récurrent ou une liste d'abonnement. Peut être placé en ligne, sur les médias sociaux, dans les e-mails, dans les imprimés, etc.</td>
  </tr>
  <tr>
    <td>Custom Short Domain</td>
    <td>Si vous utilisez le raccourcisseur de lien Vibes, l’URL raccourcie apparaîtra par défaut sous l’URL courte Vibes : https://vbs.cm/xxxxxx. Un domaine court personnalisé est un domaine unique à votre marque. <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">En savoir plus sur les domaines courts personnalisés</a>.<p>
    Cela s'applique uniquement aux messages envoyés à partir de la plateforme Vibes, en particulier les messages de campagne d'acquisition et les messages par défaut à code court.<p>
    Le raccourcisseur d’URL Marketo est recommandé pour que les données de clic soient présentes dans votre programme Marketo.</td>
  </tr>
  <tr>
    <td>Messages par défaut</td>
    <td>Messages obligatoires pour le code court afin de répondre aux demandes HELP, STOP et de messages non reconnus.</td>
  </tr>
  <tr>
    <td>Se déconnecter</td>
    <td>Les déconnexions sont une forme d’opt-out en raison de la suppression du numéro de mobile d’un réseau d’opérateurs. Les raisons de cette déconnexion sont les suivantes : un compte a été complètement fermé, un compte prépayé est à court de fonds ou le numéro a été retiré du réseau d’opérateurs pour d’autres raisons inconnues. Les numéros mobiles déconnectés et non transférés vers un autre opérateur mobile sont désabonnés de toutes les listes d'abonnement de la plateforme Vibes.</td>
  </tr>
  <tr>
    <td>Double Opt-in</td>
    <td>Méthode d’acquisition qui nécessite qu’un abonné potentiel confirme son consentement à être ajouté à une liste d’abonnements avec une commande de réponse, telle que « Y » ou son code postal. L'utilisation d'une invite de double opt-in peut vous aider à vous conformer aux directives des SMS de l'État et fédérales.</td>
  </tr>
  <tr>
    <td>Événement</td>
    <td>Un événement est une occurrence définie qui peut être envoyée à la plateforme Vibes et utilisée pour déclencher des actions déclenchées par l’API, y compris les envois de messages. Chaque événement contient des données spécifiques à l’événement, y compris un event_type, qui est utilisé pour déterminer à quelle campagne de messages déclenchée par l’API il correspond. L’API d’événement peut être déclenchée via le Webhook dans Marketo Engage. En savoir plus avec notre <a href="https://developer-platform.vibes.com/reference/event-api">référence d’API d’événement</a>.</td>
  </tr>
  <tr>
    <td>Mot-clé</td>
    <td>Mot court ou chaîne alphanumérique envoyé par le client au code court pour lancer une expérience mobile.</td>
  </tr>
  <tr>
    <td>Code Long (10DLC)</td>
    <td>Identifiant d’expéditeur à partir duquel les messages bidirectionnels sont envoyés entre la marque et le client. Les codes longs US sont à 10 chiffres.</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>Numéro d’annuaire mobile ou numéro de téléphone d’une personne. Les numéros de MDN et de téléphone mobile ne sont pas des identifiants uniques dans Marketo.</td>
  </tr>
  <tr>
    <td>Base de données mobile</td>
    <td>La base de données mobile est la base de données dans laquelle Vibes stocke les données des abonnés. Chaque abonné possède un « enregistrement de personne » unique, où le numéro de mobile et les champs personnalisés associés sont renseignés.</td>
  </tr>
  <tr>
    <td>Participant</td>
    <td>Une personne qui a une ou plusieurs interactions mobiles (comme l’envoi d’un message texte) avec votre programme mobile, mais qui ne s’est pas abonnée à une liste d’abonnements.</td>
  </tr>
  <tr>
    <td>Enregistrement de personne</td>
    <td>Un enregistrement de personne est un ensemble de données relatives à un numéro de téléphone mobile spécifique. Chaque enregistrement de personne se voit également attribuer une clé_personne unique pour identification. Les identifiants Marketo sont liés à Vibes à l’aide du champ external_person_id . En savoir plus sur les enregistrements de personne dans <a href="https://developer-platform.vibes.com/reference/person-api">Documentation de l’API Personne Vibes</a>.</td>
  </tr>
  <tr>
    <td>Numéro court</td>
    <td>Identifiant d’expéditeur à partir duquel les messages bidirectionnels sont envoyés entre la marque et le client. Les numéros courts américains sont composés de 5 à 6 chiffres. Les numéros courts canadiens sont composés de 4 à 6 chiffres. L’intégration de Marketo LaunchPoint à Vibes prend en charge un numéro court par instance.</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>Service de messages courts. Il s’agit d’un message qui comprend uniquement du texte.</td>
  </tr>
  <tr>
    <td>Listes d’abonnements</td>
    <td>Liste de numéros de mobile (et des enregistrements de personne correspondants) ayant consenti à recevoir des messages récurrents de votre programme.</td>
  </tr>
  <tr>
    <td>Abonné</td>
    <td>Numéro de mobile abonné à une ou plusieurs listes d’abonnements.</td>
  </tr>
  <tr>
    <td>Plateforme Vibes</td>
    <td>Site web auquel vous vous connectez pour gérer vos campagnes. Accédez à <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> pour accéder à la plateforme Vibes.</td>
  </tr>
</tbody>
</table>
