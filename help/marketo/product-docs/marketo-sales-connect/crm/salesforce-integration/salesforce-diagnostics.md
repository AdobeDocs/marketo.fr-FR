---
unique-page-id: 14745730
description: Diagnostics Salesforce - Documents Marketo - Documentation du produit
title: Diagnostics Salesforce
exl-id: a2b5bd10-bc92-4fd4-bc1b-4e02b48c9d83
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 1%

---

# Diagnostics Salesforce {#salesforce-diagnostics}

Une partie de notre intégration Salesforce inclut une page de diagnostic Salesforce dans l’application web. Cette page capture les erreurs provenant de la journalisation des données ayant échoué dans Salesforce. Les erreurs peuvent s’avérer utiles, mais ne sont pas toujours lisibles. Ainsi, nous avons mis en place une feuille de tricherie qui aide à expliquer les messages d&#39;erreur.

**Erreur :** API_CURRENTLY_DISABLED\
**Catégorie :** Accès/Validation\
**Message :** L’API est désactivée pour cet utilisateur\
**Ce qui se passe :** L’utilisateur ne dispose pas d’un accès à l’API\
**Étapes de dépannage :** L’administrateur Salesforce doit accorder l’accès à l’API utilisateur.

<br> 

**Erreur :** AUTHENTICATION_FAILURE\
**Catégorie :** Authentification\
**Message :** invalid_grant : échec d’authentification\
**Ce qui se passe :** Échec de l’authentification\
**Étapes de dépannage :** Déconnectez-vous de Salesforce, puis reconnectez-vous.

<br> 

**Erreur :** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Catégorie :** Accès/Validation\
**Message :** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Session expirée ou non valide&quot;}\
**Ce qui se passe :**

1 - Le code du déclencheur provoque l’échec de la mise à jour.\
2 - L’utilisateur ne dispose pas d’autorisations d’écriture au niveau de l’objet sur l’objet donné.

**Étapes de dépannage :**

1 - Déclencheur de révision qui échoue.\
2 - Accordez à l’utilisateur l’accès en écriture pour l’objet OU désactivez la fonction qui tente d’écrire sur l’objet.

<br> 

**Erreur :** CANNOT_UPDATE_CONVERTED_LEAD\
**Catégorie :** Autre\
**Message :** ne peut pas référencer de prospect converti\
**Ce qui se passe :** Nous tentons de nous connecter à une piste convertie lors de la journalisation des activités les plus récentes pour les contacts et les pistes. J&#39;en ai aussi vu quelques-uns pour les terrains.\
**Étapes de dépannage :** Veuillez signaler tout cas de ce type à notre [équipe d&#39;assistance](https://nation.marketo.com/t5/Support/ct-p/Support).

<br> 

**Erreur :** ENTITY_IS_LOCKED\
**Catégorie :** Accès/Validation\
**Message :** l’entité est verrouillée pour modification\
**Ce qui se passe :** L’enregistrement est dans un processus de validation où il est verrouillé de toute modification supplémentaire jusqu’à ce qu’il soit approuvé ou refusé par une personne propriétaire de la validation.\
**Étapes de dépannage :** Voir ci-dessus.

<br> 

**Erreur :** EXPIRED_ACCESS
**Catégorie :** Authentification
**Message :** invalid_grant : jeton d’accès/d’actualisation expiré
**Ce qui se passe :** Le jeton d’accès ou d’actualisation a expiré. Les jetons expirent en fonction de [paramètres de session dans Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Étapes de dépannage :** Vous devrez vous authentifier à nouveau. Déconnectez la connexion Salesforce et reconnectez-vous.

<br> 

**Erreur :** FAILED_WRITE\
**Catégorie :** Intermittent\
**Message :** fin de fichier atteinte\
**Ce qui se passe :** Problème de performance avec Salesforce, probablement en raison de déclencheurs sous-optimaux côté client.\
**Étapes de dépannage :** La logique de reprise doit gérer cela. Si cela ne fonctionne toujours pas, travaillez avec votre administrateur Salesforce pour résoudre un problème de déclencheur.

<br> 

**Erreur :** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Catégorie :** Accès/Validation
**Message :** Varie d’un client à l’autre.
**Ce qui se passe :** Échec d’une règle de validation personnalisée pour l’objet.
**Étapes de dépannage :** Vérifiez la règle de validation personnalisée à l’origine de cette erreur. Puisqu’il s’agit d’une règle personnalisée, l’erreur doit être traitée ponctuellement.

<br> 

**Erreur :** FIELD_FILTER_VALIDATION_EXCEPTION\
**Catégorie :** Accès/Validation\
**Message :** La valeur n’existe pas ou ne correspond pas aux critères de filtre\
**Ce qui se passe :** Les données incorrectes existantes dans Salesforce sont appliquées lors de la mise à jour.\
**Étapes de dépannage :** Voir ci-dessus.

<br> 

**Erreur :** FIELD_INTEGRITY_EXCEPTION\
**Catégorie :** Accès/Validation\
**Message :** Le pays/territoire existant ne reconnaît pas la valeur de l’état pour le champ : Code état/province\
**Ce qui se passe :** Les données incorrectes existantes dans Salesforce sont appliquées lors de la mise à jour.\
**Étapes de dépannage :** Voir ci-dessus.

<br> 

**Erreur :** INACTIVE_ORGANIZATION\
**Catégorie :** Authentification\
**Message :** invalid_grant : organisation inactive\
**Ce qui se passe :** Votre organisation Salesforce n’est plus principale.\
**Étapes de dépannage :** Déconnectez-vous puis reconnectez-vous de Salesforce.

**Erreur :** INACTIVE_USER
**Catégorie :** Authentification
**Message :** invalid_grant : utilisateur inactif
**Ce qui se passe :** L’utilisateur Salesforce n’est plus principal
**Étapes de dépannage :** Déconnectez-vous puis reconnectez-vous de Salesforce.

**Erreur :** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Catégorie :** Intermittent\
**Message :** (aucun message supplémentaire)\
**Ce qui se passe :** L’instance Salesforce est en mode de maintenance.\
**Étapes de dépannage :** Patientez jusqu’à ce que la maintenance du système soit terminée, puis relancez la journalisation.

**Erreur :** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Catégorie :** Accès/Validation
**Message :** droits d’accès insuffisants sur l’identifiant d’objet
**Ce qui se passe :** Accès à l’enregistrement parent pour une tâche.
**Étapes de dépannage :** Voir ci-dessus.

<br> 

**Erreur :** INSUFFICIENT_ACCESS_OR_READONLY\
**Catégorie :** Accès/Validation
**Message :** droits d’accès insuffisants sur l’identifiant d’objet
**Ce qui se passe :** La journalisation de l’activité la plus récente ne peut pas modifier l’enregistrement spécifique, car l’utilisateur ne dispose pas d’un accès en écriture.\
**Étapes de dépannage :** Accordez à l’utilisateur l’accès dans Salesforce OU désactivez la journalisation de l’activité la plus récente pour cet objet.

**Erreur :** INVALID_FIELD\
**Catégorie :** Intermittent\
**Message :** Net::ReadTimeout\
**Ce qui se passe :** La demande expire. Cela est probablement dû à un trop grand nombre de transactions lentes.\
**Étapes de dépannage :** Examinez les personnalisations existantes pour détecter les éventuels coupables des problèmes de latence et/ou désactivez la journalisation de l’activité la plus récente pour un ou tous les objets afin de réduire la charge.

**Erreur :** INVALID_FIELD_FOR_INSERT_UPDATE\
**Catégorie :** Accès/Validation\
**Message :** Impossible de créer/mettre à jour les champs : ToutApp__Tout_Last_Replied__c. Vérifiez les paramètres de sécurité de ce champ.
**Ce qui se passe :** Les utilisateurs n’ont pas accès en écriture aux champs personnalisés Tout nécessaires pour effectuer la transaction de journalisation de l’activité la plus récente. L’équipe a peut-être installé le package mais n’a pas activé les champs appropriés pour les utilisateurs.\
**Étapes de dépannage :** L’administrateur Salesforce doit accorder l’accès aux champs personnalisés OU désactiver la journalisation de l’activité la plus récente.

**Erreur :** INVALID_GRANT\
**Catégorie :** Authentification\
**Message :** invalid_grant : ip restricted\
**Ce qui se passe :** Nous tentons d’accéder à votre Salesforce, mais vous disposez de restrictions de IP qui nous empêchent de le faire.\
**Étapes de dépannage :** Votre administrateur Salesforce devra placer sur la liste autorisée nos adresses IP. Les utilisateurs doivent contacter l’assistance pour obtenir les adresses IP.

**Erreur :** INVALID_TYPE\
**Catégorie :** Accès/Validation\
**Message :** CreatedDate, (SELECT Id FROM Tasks) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Colonne : 53sType d’objet &quot;Lead&quot; n’est pas pris en charge. Si vous essayez d’utiliser un objet personnalisé, assurez-vous d’ajouter « __c » après le nom de l’entité. Référencez votre WSDL ou l’appel de description pour connaître les noms appropriés.
**Ce qui se passe :** Nous tentons d’interroger un type d’objet de Salesforce auquel l’utilisateur n’a pas accès. Cela est probablement lié au fait que l’utilisateur n’a pas le droit d’accéder à l’objet de piste.\
**Étapes de dépannage :** Accordez l’accès en lecture et en mise à jour à l’objet Lead dans Salesforce ou désactivez la journalisation des emails et la journalisation des activités les plus récentes pour créer des enregistrements de piste.

**Erreur :** QUERY_TIMEOUT\
**Catégorie :** Intermittent\
**Message :** Votre requête était trop longue.\
**Ce qui se passe :** Voir ci-dessus.\
**Étapes de dépannage :** La logique de reprise doit gérer cela. Si cela ne fonctionne toujours pas, travaillez avec votre administrateur Salesforce pour résoudre un problème de déclencheur.

**Erreur :** REQUEST_LIMIT_EXCEEDED\
**Catégorie :** Intermittent\
**Message :**
1 - Dépassement de la limite concurrentPerOrgLongTxn\
2 - Limite totale des demandes dépassée\
3 - ConcurrentRequest\
**Ce qui se passe :**
1 - Dépassement de la limite de requête simultanée, probablement en raison d’un code de déclenchement inefficace.\
2 - Trop d&#39;intégrations placent l&#39;organisation au-delà de la fenêtre déroulante de 24 heures.\
**Étapes de dépannage :**
1 - Examinez les déclencheurs existants sur les objets concernés. Désactivation potentielle de la journalisation de cumul pour un ou plusieurs objets.\
2 - Achetez d’autres appels API de Salesforce. Désactivation potentielle de la journalisation de cumul pour un ou plusieurs objets.

**Erreur :** REQUIRED_FIELD_MISSING\
**Catégorie :** Accès/Validation\
**Message :** Les champs obligatoires sont manquants : `[Amount_Committed_Private_Capital__c]`
**Ce qui se passe :** Cela se produit généralement pour la journalisation de l’activité la plus récente. Les champs personnalisés ont été configurés pour être obligatoires, mais contiennent des valeurs vides. Cela peut se produire si l’enregistrement a été créé avec une valeur vide du champ personnalisé et a ensuite été rendu obligatoire. L’exigence est appliquée lorsque nous tentons de mettre à jour l’enregistrement, même si nous ne touchons pas au champ personnalisé.\
**Étapes de dépannage :** Mettez à jour manuellement les valeurs des champs manquants. Vous pouvez ensuite réessayer le message à partir de ToutApp.

**Erreur :** SERVER_UNAVAILABLE\
**Catégorie :** Intermittent\
**Message :** serveur trop occupé\
**Ce qui se passe :** Problème de performance avec Salesforce, probablement en raison de déclencheurs sous-optimaux par le client\
**Étapes de dépannage :** La logique de reprise doit gérer cela. Si cela ne fonctionne toujours pas, travaillez avec votre administrateur Salesforce pour tirer sur un déclencheur problématique.

**Erreur :** TXN_SECURITY_NO_ACCESS\
**Catégorie :** Accès/Validation\
**Message :** L’opération que vous avez demandée n’est pas autorisée en raison d’une stratégie de sécurité de votre entreprise. Contactez l’administration.<br/>
**Ce qui se passe :** Une certaine restriction de sécurité a été configurée - voir https://developer.salesforce.com/forums/?id=&quot;enregistrement ID&quot;\
**Étapes de dépannage :** Adressez-vous à votre administrateur Salesforce pour voir quelle est la restriction spécifique.

**Erreur :** UNABLE_TO_LOCK_ROW\
**Catégorie :** Intermittent\
**Message :** impossible d&#39;obtenir un accès exclusif à cet enregistrement ou à 1 enregistrement : &quot;enregistrement ID&quot;\
**Ce qui se passe :** Il est probable qu’un déclencheur provoque plusieurs tentatives d’accès au même enregistrement, éventuellement dans le cas d’un email de groupe.\
**Étapes de dépannage :** La logique de reprise doit gérer cela. Si cela ne fonctionne toujours pas, travaillez avec votre administrateur Salesforce pour résoudre un problème de déclencheur.

**Erreur :** UNKNOWN_EXCEPTION
**Catégorie :** Autre\
**Message :** Une exception inconnue s’est produite\
**Ce qui se passe :** Exception non gérée dans Salesforce.\
**Étapes de dépannage :** Placez une casse avec Salesforce et copiez les valeurs numériques dans le message d’erreur. Ce code Salesforce ne gère pas correctement une erreur.
