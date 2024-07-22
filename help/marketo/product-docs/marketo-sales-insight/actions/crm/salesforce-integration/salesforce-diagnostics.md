---
description: Diagnostics Salesforce - Documents Marketo - Documentation du produit
title: Diagnostics Salesforce
exl-id: c449f938-9615-47cb-b232-613ec29068a3
feature: Sales Insight Actions
source-git-commit: 9384d72b335a4b975b190816ea999ad067fddeda
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 1%

---

# Diagnostics Salesforce {#salesforce-diagnostics}

Une partie de notre intégration Salesforce inclut une page de diagnostic Salesforce dans l’application web. Cette page capture les erreurs provenant de la journalisation des données ayant échoué dans Salesforce. Les erreurs peuvent s’avérer utiles, mais ne sont pas toujours lisibles. Ainsi, nous avons mis en place une feuille de tricherie qui aide à expliquer les messages d&#39;erreur.

## Diagnostics d’accès {#access-diagnostics}

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/salesforce-diagnostics-1.png)

1. Sous Intégrations, cliquez sur **Diagnostics**.

   ![](assets/salesforce-diagnostics-2.png)

## Aide-mémoire sur les erreurs {#error-cheat-sheet}

**Erreur :** API_CURRENTLY_DISABLED\
**Catégorie :** Accès/Validation\
L’API **Message:** est désactivée pour cet utilisateur\
**Ce qui se passe :** L’utilisateur n’a pas accès à l’API\
**Étapes de dépannage :** L’administrateur Salesforce doit accorder l’accès à l’API de l’utilisateur.

**Erreur :** AUTHENTICATION_FAILURE\
**Catégorie :** Authentification\
**Message :** invalid_grant : échec de l’authentification\
**Ce qui se passe :** Échec de l’authentification\
**Étapes de dépannage :** Déconnectez-vous de Salesforce, puis reconnectez-vous.

**Erreur :** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Catégorie :** Accès/Validation\
**Message:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Session expirée ou non valide&quot;}\
**Ce qui se passe :**

1 - Le code du déclencheur provoque l’échec de la mise à jour.\
2 - L’utilisateur ne dispose pas d’autorisations d’écriture au niveau de l’objet sur l’objet donné.

**Étapes de dépannage :**

1 - Déclencheur de révision qui échoue.\
2 - Accordez à l’utilisateur l’accès en écriture pour l’objet OU désactivez la fonction qui tente d’écrire sur l’objet.

**Erreur :** CANNOT_UPDATE_CONVERTED_LEAD\
**Catégorie :** Autre\
**Message :** ne peut pas référencer de piste convertie\
**Ce qui se passe :** Nous essayons de nous connecter à un prospect converti lors de la journalisation des activités les plus récentes pour les contacts et les pistes. J&#39;en ai aussi vu quelques-uns pour les terrains.\
**Étapes de dépannage :** Veuillez en signaler toute instance à notre [équipe d&#39;assistance](https://nation.marketo.com/t5/Support/ct-p/Support).

**Erreur :** ENTITY_IS_LOCKED\
**Catégorie :** Accès/Validation\
**Message :** l&#39;entité est verrouillée pour modification\
**Ce qui se passe :** L’enregistrement se trouve dans un processus d’approbation où il est verrouillé de toute modification supplémentaire jusqu’à ce qu’il soit approuvé ou refusé par une personne propriétaire de la validation.\
**Étapes de dépannage :** Voir ci-dessus.

**Erreur :** EXPIRED_ACCESS
**Catégorie :** Authentification
**Message :** invalid_grant : jeton d’accès/d’actualisation expiré
**Ce qui se passe :** Le jeton d’accès ou d’actualisation a expiré. Les jetons expirent en fonction des [paramètres de session dans Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Étapes de dépannage :** vous devrez vous reconnecter. Déconnectez la connexion Salesforce et reconnectez-vous.

**Erreur :** FAILED_WRITE\
**Catégorie :** Intermittent\
**Message :** fin de fichier atteinte\
**Ce qui se passe :** Problème de performance avec Salesforce, probablement en raison de déclencheurs sous-optimaux côté client.\
**Étapes de dépannage :** La logique de reprise doit gérer cela. Si cela ne fonctionne toujours pas, travaillez avec votre administrateur Salesforce pour résoudre un problème de déclencheur.

**Erreur :** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Catégorie :** Accès/Validation
**Message :** varie d’un client à l’autre.
**Ce qui se passe :** Échec d’une règle de validation personnalisée pour l’objet.
**Étapes de dépannage :** Vérifiez la règle de validation personnalisée qui cause cette erreur. Puisqu’il s’agit d’une règle personnalisée, l’erreur doit être traitée ponctuellement.

**Erreur :** FIELD_FILTER_VALIDATION_EXCEPTION\
**Catégorie :** Accès/Validation\
**Message:** La valeur n’existe pas ou ne correspond pas aux critères de filtre\
**Ce qui se passe :** Les données incorrectes existantes dans Salesforce sont appliquées lors de la mise à jour.\
**Étapes de dépannage :** Voir ci-dessus.

**Erreur :** FIELD_INTEGRITY_EXCEPTION\
**Catégorie :** Accès/Validation\
**Message :** Le pays/territoire existant ne reconnaît pas la valeur d’état pour le champ : Code état/province\
**Ce qui se passe :** Les données incorrectes existantes dans Salesforce sont appliquées lors de la mise à jour.\
**Étapes de dépannage :** Voir ci-dessus.

**Erreur :** INACTIVE_ORGANIZATION\
**Catégorie :** Authentification\
**Message :** invalid_grant : organisation inactive\
**Ce qui se passe :** Votre organisation Salesforce n’est plus active.
**Étapes de dépannage :** Déconnectez-vous puis reconnectez-vous de Salesforce.

**Erreur :** INACTIVE_USER
**Catégorie :** Authentification
**Message :** invalid_grant : utilisateur inactif
**Ce qui se passe :** L’utilisateur Salesforce n’est plus actif
**Étapes de dépannage :** Déconnectez-vous de Salesforce, puis reconnectez-vous.

**Erreur :** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Catégorie :** Intermittent\
**Message:** (aucun message supplémentaire)\
**Ce qui se passe :** l’instance Salesforce est en mode de maintenance.\
**Étapes de dépannage :** Patientez jusqu’à ce que la maintenance du système soit terminée, puis réessayez la journalisation.

**Erreur :** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Catégorie :** Accès/Validation
**Message :** droits d’accès insuffisants sur l’ID d’objet
**Ce qui se passe :** Accès impossible à l’enregistrement parent pour une tâche.
**Étapes de dépannage :** Voir ci-dessus.

**Erreur :** INSUFFICIENT_ACCESS_OR_READONLY\
**Catégorie :** Accès/Validation
**Message :** droits d’accès insuffisants sur l’ID d’objet
**Ce qui se passe :** La journalisation de l’activité la plus récente ne peut pas modifier l’enregistrement spécifique car l’utilisateur ne dispose pas d’un accès en écriture.\
**Étapes de dépannage :** Accordez l’accès utilisateur dans Salesforce OU désactivez la journalisation de l’activité la plus récente pour cet objet pour cet utilisateur.

**Erreur :** INVALID_FIELD\
**Catégorie :** Intermittent\
**Message:** Net::ReadTimeout\
**Ce qui se passe :** la demande expire. Cela est probablement dû à un trop grand nombre de transactions lentes.\
**Étapes de dépannage :** passez en revue les personnalisations existantes pour détecter les éventuels coupables des problèmes de latence et/ou désactivez la journalisation de l’activité la plus récente pour un ou tous les objets afin de réduire la charge.

**Erreur :** INVALID_FIELD_FOR_INSERT_UPDATE\
**Catégorie :** Accès/Validation\
**Message :** Impossible de créer/mettre à jour les champs : MSE_Replied__c. Vérifiez les paramètres de sécurité de ce champ.
**Ce qui se passe :** Les utilisateurs n’ont pas accès en écriture aux champs personnalisés Actions d’aperçu des ventes nécessaires pour effectuer la transaction de journalisation de l’activité la plus récente. L’équipe a peut-être installé le package mais n’a pas activé les champs appropriés pour les utilisateurs.\
**Étapes de dépannage :** L’administrateur Salesforce doit accorder l’accès aux champs personnalisés OU désactiver la journalisation de l’activité la plus récente.

**Erreur :** INVALID_GRANT\
**Catégorie :** Authentification\
**Message :** invalid_grant : ip restricted\
**Ce qui se passe :** Nous essayons d’accéder à votre Salesforce, mais vous disposez de restrictions d’accès aux adresses IP qui nous empêchent de le faire.\
**Étapes de dépannage :** Votre administrateur Salesforce devra placer sur la liste autorisée nos adresses IP. Les utilisateurs doivent contacter l’assistance pour obtenir les adresses IP.

**Erreur :** INVALID_TYPE\
**Catégorie :** Accès/Validation\
**Message :** CreatedDate, (SELECT Id FROM Tasks) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at `Row:1:Column:53sObject` type &#39;Lead&#39; n’est pas pris en charge. Si vous essayez d’utiliser un objet personnalisé, assurez-vous d’ajouter « __c » après le nom de l’entité. Veuillez référencer votre WSDL ou l’appel de description pour connaître les noms appropriés
**Ce qui se passe :** Nous essayons d’interroger un type d’objet de Salesforce auquel l’utilisateur n’a pas accès. Cela est probablement lié au fait que l’utilisateur n’a pas le droit d’accéder à l’objet de piste.\
**Étapes de dépannage :** Accordez l’accès en lecture et mise à jour à l’objet Lead dans Salesforce ou désactivez la journalisation des emails et de l’activité la plus récente pour créer des enregistrements de piste.

**Erreur :** QUERY_TIMEOUT\
**Catégorie :** Intermittent\
**Message :** Votre requête de requête était trop longue\
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
**Message:** Les champs obligatoires sont manquants : `[Amount_Committed_Private_Capital__c]`
**Ce qui se passe :** Cela se produit généralement pour la journalisation de l’activité la plus récente. Les champs personnalisés ont été configurés pour être obligatoires, mais contiennent des valeurs vides. Cela peut se produire si l’enregistrement a été créé avec une valeur vide du champ personnalisé et a ensuite été rendu obligatoire. L’exigence est appliquée lorsque nous tentons de mettre à jour l’enregistrement, même si nous ne touchons pas au champ personnalisé.\
**Étapes de dépannage :** mettez manuellement à jour les valeurs des champs manquants. Vous pouvez ensuite réessayer le message à partir des actions Sales Insight .

**Erreur :** SERVER_UNAVAILABLE\
**Catégorie :** Intermittent\
**Message :** serveur trop occupé\
**Ce qui se passe :** Problème de performance avec Salesforce, probablement en raison de déclencheurs sous-optimaux par le client\
**Étapes de dépannage :** La logique de reprise doit gérer cela. Si cela ne fonctionne toujours pas, travaillez avec votre administrateur Salesforce pour tirer sur un déclencheur problématique.

**Erreur :** TXN_SECURITY_NO_ACCESS\
**Catégorie :** Accès/Validation\
**Message :** L’opération que vous avez demandée n’est pas autorisée en raison d’une stratégie de sécurité dans votre organisation. Contactez votre administrateur.
**Qu’est-ce qui se passe :** Une restriction de sécurité a été configurée - voir https://developer.salesforce.com/forums/?id=&quot;enregistrement ID&quot;\
**Étapes de dépannage :** Contactez votre administrateur Salesforce et voyez quelle pourrait être la restriction spécifique.

**Erreur :** UNABLE_TO_LOCK_ROW\
**Catégorie :** Intermittent\
**Message :** impossible d’obtenir un accès exclusif à cet enregistrement ou à 1 enregistrement : &quot;ID d’enregistrement&quot;\
**Ce qui se passe :** Il est probable qu’un déclencheur provoque plusieurs tentatives d’accès au même enregistrement, éventuellement dans le cas d’un email de groupe.\
**Étapes de dépannage :** La logique de reprise doit gérer cela. Si cela ne fonctionne toujours pas, travaillez avec votre administrateur Salesforce pour résoudre un problème de déclencheur.

**Erreur :** UNKNOWN_EXCEPTION
**Catégorie :** Autre\
**Message :** Une exception inconnue s&#39;est produite\
**Ce qui se passe :** Exception non gérée dans Salesforce.\
**Étapes de dépannage :** Créez un dossier avec Salesforce et copiez les valeurs numériques dans le message d’erreur. Il s’agit du code Salesforce qui ne gère pas correctement une erreur.
