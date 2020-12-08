---
unique-page-id: 14745730
description: Diagnostics Salesforce - Docs marketing - Documentation du produit
title: Diagnostics Salesforce
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---


# Diagnostics Salesforce {#salesforce-diagnostics}

Une partie de notre intégration Salesforce inclut une page de diagnostic Salesforce dans l&#39;application Web. Cette page capture les erreurs provenant de l&#39;échec de la journalisation des données dans Salesforce. Les erreurs peuvent être utiles, mais ne sont pas toujours lisibles. En tant que tel, nous avons mis en place une feuille de tricherie qui aide à expliquer les messages d&#39;erreur.

**Erreur :** API_CURRENTLY_DISABLED\
**Catégorie :** Accès/Validation\
**Message :** L&#39;API est désactivée pour cet utilisateur\
**Ce qui se passe :** L&#39;utilisateur n&#39;a pas accès à l&#39;API\
**Procédure de dépannage :** L’administrateur Salesforce doit accorder l’accès à l’API de l’utilisateur.

<br> 

**Erreur :** AUTHENTICATION_FAILURE\
**Catégorie :** Authentification\
**Message :** Invalid_grant: échec d&#39;authentification\
**Ce qui se passe :** Échec de l&#39;authentification\
**Procédure de dépannage :** Déconnectez-vous de Salesforce, puis reconnectez-vous.

<br> 

**Erreur :** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Catégorie :** Accès/Validation\
**Message :** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Session expirée or Invalid&quot;}\
**Ce qui se passe :**

1 - Le code du déclencheur provoque l’échec de la mise à jour.\
2 - L&#39;utilisateur ne dispose pas d&#39;autorisations d&#39;écriture au niveau de l&#39;objet sur l&#39;objet donné.

**Procédure de dépannage :**

1 - Révision du déclencheur qui échoue.\
2 - Accordez à l&#39;utilisateur l&#39;accès en écriture pour l&#39;objet OU désactivez la fonction qui tente d&#39;écrire sur l&#39;objet.

<br> 

**Erreur :** CANNOT_UPDATE_CONVERTED_LEAD\
**Catégorie :** Autre\
**Message :** impossible de référencer un prospect converti\
**Ce qui se passe :** Nous essayons de nous connecter à une piste convertie lors de la consignation des dernières Activités pour les contacts et les pistes. J&#39;en ai aussi vu quelques-uns pour des pas.\
**Procédure de dépannage :** Veuillez en informer notre équipe [d&#39;](http://nation.marketo.com/community/support_solutions)assistance.

<br> 

**Erreur :** ENTITY_IS_LOCKED\
**Catégorie :** Accès/Validation\
**Message :** l&#39;entité est verrouillée pour modification\
**Ce qui se passe :** L&#39;enregistrement est en cours de processus d&#39;approbation où il est verrouillé de toute modification supplémentaire jusqu&#39;à ce qu&#39;il soit approuvé ou refusé par une personne qui détient l&#39;approbation.\
**Procédure de dépannage :** Voir ci-dessus.

<br> 

**Erreur :** EXPIRED_ACCESS **Catégorie :** Message d&#39;authentification **:** Invalid_grant: jeton **d&#39;accès/d&#39;actualisation expiré Ce qui se passe :** Le jeton d’accès ou d’actualisation a expiré. Les jetons expirent en fonction des paramètres de [session dans Salesforce](http://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Procédure de dépannage :** Vous devrez vous réauthentifier. Déconnectez la connexion Salesforce et reconnectez-la.

<br> 

**Erreur :** FAILED_WRITE\
**Catégorie :** Intermittent\
**Message :** fin de fichier atteinte\
**Ce qui se passe :** Problème de performances avec Salesforce, probablement en raison de déclencheurs sous-optimaux côté client.\
**Procédure de dépannage :** La logique de nouvelle tentative doit gérer cette situation. Si cela ne fonctionne toujours pas, demandez à votre administrateur Salesforce de résoudre les problèmes liés à un trigger.

<br> 

**Erreur :** FIELD_CUSTOM_VALIDATION_EXCEPTION **Catégorie :** Message d&#39;accès/de validation **:** Varie d’un client à l’autre.
**Ce qui se passe :** Echec d’une règle de validation personnalisée pour l’objet.
**Procédure de dépannage :** Vérifiez la règle de validation personnalisée à l’origine de cette erreur. Comme il s&#39;agit d&#39;une règle personnalisée, l&#39;erreur doit être traitée de façon ponctuelle.

<br> 

**Erreur :** FIELD_FILTER_VALIDATION_EXCEPTION\
**Catégorie :** Accès/Validation\
**Message :** La valeur n&#39;existe pas ou ne correspond pas aux critères de filtre\
**Ce qui se passe :** Données incorrectes existantes dans Salesforce appliquées à la mise à jour.\
**Procédure de dépannage :** Voir ci-dessus.

<br> 

**Erreur :** FIELD_INTEGRITY_EXCEPTION\
**Catégorie :** Accès/Validation\
**Message :** Le pays/territoire existant ne reconnaît pas la valeur d’état pour le champ : Code d&#39;état/de province\
**Ce qui se passe :** Données incorrectes existantes dans Salesforce appliquées à la mise à jour.\
**Procédure de dépannage :** Voir ci-dessus.

<br> 

**Erreur :** INACTIVE_ORGANIZATION\
**Catégorie :** Authentification\
**Message :** Invalid_grant: organisation inactive\
**Ce qui se passe :** Votre organisation Salesforce n&#39;est plus principale.\
**Procédure de dépannage :** Déconnectez-vous puis reconnectez-vous de Salesforce.

**Erreur :** INACTIVE_USER **Catégorie :** Message d&#39;authentification **:** Invalid_grant: utilisateur **inactif Ce qui se passe :** L&#39;utilisateur Salesforce n&#39;est plus la principale **Procédure de dépannage :** Déconnectez-vous puis reconnectez-vous de Salesforce.

**Erreur :** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Catégorie :** Intermittent\
**Message :** (aucun message supplémentaire)\
**Ce qui se passe :** L&#39;instance Salesforce est en mode de maintenance.\
**Procédure de dépannage :** Patientez jusqu&#39;à ce que la maintenance du système soit terminée, puis recommencez la journalisation.

**Erreur :** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY **Catégorie :** Message d&#39;accès/de validation **:** droits d&#39;accès insuffisants sur l&#39;ID **d&#39;objet Ce qui se passe :** Accès impossible à l&#39;enregistrement parent pour une tâche.
**Procédure de dépannage :** Voir ci-dessus.

<br> 

**Erreur :** INSUFFICIENT_ACCESS_OR_READONLY\
**Catégorie :** Accès/Validation** ****Message :** droits d&#39;accès insuffisants sur l&#39;ID d&#39;objet** ****Que se passe-t-il ?** La consignation des Activités les plus récentes ne peut pas modifier l&#39;enregistrement spécifique, car l&#39;utilisateur n&#39;a pas accès en écriture.\
**Procédure de dépannage :** Accordez à l&#39;utilisateur l&#39;accès dans Salesforce OU désactivez la journalisation de l&#39;Activité la plus récente pour cet objet pour cet utilisateur.

**Erreur :** INVALID_FIELD\
**Catégorie :** Intermittent\
**Message :** Net::ReadTimeout\
**Ce qui se passe :** La demande arrive à expiration. Cela est probablement dû à un trop grand nombre de transactions lentes.\
**Procédure de dépannage :** Examinez les personnalisations existantes pour identifier les coupables potentiels des problèmes de latence et/ou désactivez la journalisation des Activités les plus récentes pour un ou tous les objets afin de réduire la charge.

**Erreur :** INVALID_FIELD_FOR_INSERT_UPDATE\
**Catégorie :** Accès/Validation\
**Message :** Impossible de créer/mettre à jour les champs : ToutApp__Tout_Last_Replied__c. Veuillez vérifier les paramètres de sécurité de ce champ.\
**Ce qui se passe :** Les utilisateurs n’ont pas accès en écriture aux champs personnalisés Tout nécessaires pour effectuer la transaction de consignation des Activités les plus récentes. L&#39;équipe a peut-être installé le package mais n&#39;a pas activé les champs appropriés pour les utilisateurs.\
**Procédure de dépannage :** L&#39;administrateur Salesforce doit accorder l&#39;accès aux champs personnalisés OU désactiver la journalisation des Activités les plus récentes.

**Erreur :** INVALID_GRANT\
**Catégorie :** Authentification\
**Message :** Invalid_grant: ip restreint\
**Ce qui se passe :** Nous essayons d&#39;accéder à votre Salesforce, mais vous avez des restrictions d&#39;accès à Internet qui nous empêchent de le faire.\
**Procédure de dépannage :** Votre administrateur Salesforce devra placer sur la liste autorisée nos adresses IP. Les utilisateurs doivent contacter l’assistance pour obtenir les adresses IP.

**Erreur :** INVALID_TYPE\
**Catégorie :** Accès/Validation\
**Message :** CreatedDate, (SELECT Id FROM Tâches) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Column:53sLe type d&#39;objet &quot;Lead&quot; n&#39;est pas pris en charge. Si vous tentez d&#39;utiliser un objet personnalisé, veillez à ajouter le signe &quot;__c&quot; après le nom de l&#39;entité. Veuillez référencer votre fichier WSDL ou l&#39;appel de description pour connaître les noms appropriés.\
**Ce qui se passe :** Nous essayons de requête un type d&#39;objet de Salesforce auquel l&#39;utilisateur n&#39;a pas accès. Cela est probablement lié au fait que l&#39;utilisateur n&#39;a pas le droit d&#39;accès à l&#39;objet de piste.\
**Procédure de dépannage :** Accordez l&#39;accès en lecture et en mise à jour à l&#39;objet Lead dans Salesforce, ou désactivez la journalisation des courriers électroniques et la journalisation de l&#39;Activité la plus récente pour créer des enregistrements de piste.

**Erreur :** REQUÊTE_TIMEOUT\
**Catégorie :** Intermittent\
**Message :** Votre demande de requête était en cours d&#39;exécution trop long\
**Ce qui se passe :** Voir ci-dessus.\
**Procédure de dépannage :** La logique de nouvelle tentative doit gérer cette situation. Si cela ne fonctionne toujours pas, demandez à votre administrateur Salesforce de résoudre les problèmes liés à un trigger.

**Erreur :** REQUEST_LIMIT_EXCEEDED\
**Catégorie :** Intermittent\
**Message :**
1 - Limite concurrentPerOrgLongTxn dépassée\
2 - Limite totale des requêtes dépassée\
3 - Demande simultanée\
**Ce qui se passe :**
1 - Limite de requête simultanée dépassée, probablement en raison d&#39;un code de déclenchement inefficace.\
2 - Trop d&#39;intégrations placent l&#39;organisation au-delà de la fenêtre de roulement de 24 heures.\
**Procédure de dépannage :**
1 - Examinez les déclencheurs existants sur les objets concernés. Désactivation potentielle de la journalisation de cumul pour un ou plusieurs objets.\
2 - Achetez d&#39;autres appels d&#39;API de Salesforce. Désactivation potentielle de la journalisation de cumul pour un ou plusieurs objets.

**Erreur :** REQUIRED_FIELD_MISSING\
**Catégorie :** Accès/Validation\
**Message :** Les champs obligatoires sont manquants : [Amount_Committed_Private_Capital__c]\
**Ce qui se passe :** Cela se produit généralement pour la journalisation des Activités les plus récentes. Les champs personnalisés ont été configurés pour être obligatoires, mais leurs valeurs sont vides. Cela peut se produire si l’enregistrement a été créé avec une valeur vide du champ personnalisé, puis s’il a été rendu obligatoire. La nécessité est appliquée lorsque nous tentons de mettre à jour l’enregistrement, même si nous ne touchons pas au champ personnalisé.\
**Procédure de dépannage :** Mettez à jour manuellement les valeurs des champs manquants. Vous pouvez ensuite réessayer le message à partir de ToutApp.

**Erreur :** SERVER_UNAVAILABLE\
**Catégorie :** Intermittent\
**Message :** serveur trop occupé\
**Ce qui se passe :** Problème de performances avec Salesforce, probablement en raison de déclencheurs sous-optimaux par le client\
**Procédure de dépannage :** La logique de nouvelle tentative doit gérer cette situation. Si cela ne fonctionne toujours pas, demandez à votre administrateur Salesforce de résoudre le problème en déclenchant un trigger problématique.

**Erreur :** TXN_SECURITY_NO_ACCESS\
**Catégorie :** Accès/Validation\
**Message :** L&#39;opération que vous avez demandée n&#39;est pas autorisée en raison d&#39;une stratégie de sécurité de votre entreprise. Contactez votre administrateur.\
**Ce qui se passe :** Une sorte de restriction de sécurité a été définie - voir `https://developer.salesforce.com/forums/?id="record` ID&quot;\
**Procédure de dépannage :** Contactez votre administrateur Salesforce et voyez quelle pourrait être la restriction spécifique.

**Erreur :** UNABLE_TO_LOCK_ROW\
**Catégorie :** Intermittent\
**Message :** impossible d&#39;obtenir un accès exclusif à cet enregistrement ou à 1 enregistrement : &quot;ID enregistrement&quot;\
**Ce qui se passe :** Il existe probablement un déclencheur qui provoque plusieurs tentatives d’accès au même enregistrement, peut-être dans le cas d’un courriel de groupe.\
**Procédure de dépannage :** La logique de nouvelle tentative doit gérer cette situation. Si cela ne fonctionne toujours pas, demandez à votre administrateur Salesforce de résoudre les problèmes liés à un trigger.

**Erreur :** UNKNOWN_EXCEPTION\
**Catégorie :** Autre\
**Message :** Une exception inconnue est survenue\
**Ce qui se passe :** Exception non gérée dans Salesforce.\
**Procédure de dépannage :** Placez une casse avec Salesforce et copiez les valeurs numériques dans le message d’erreur. Il s&#39;agit du code Salesforce qui ne gère pas correctement une erreur.
