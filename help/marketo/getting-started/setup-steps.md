---
unique-page-id: 2949469
description: Procédure de configuration - Documents Marketo - Documentation du produit
title: Étapes de configuration
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
source-git-commit: 865486a0ce31297d8cc96e5fbd97275d045664b2
workflow-type: tm+mt
source-wordcount: '2005'
ht-degree: 0%

---

# Étapes de configuration {#setup-steps}

**Bienvenue sur Marketo!**

Avant d’utiliser Marketo, vous devez effectuer quelques étapes.

Ces étapes incluent :

* configuration de compte de base
* valorisation de la marque des URL de votre landing page et des liens d&#39;email pour améliorer la confiance et la délivrabilité
* Synchronisation de votre CRM
* ajout de code de suivi au site web de votre entreprise ;

>[!NOTE]
>
>Vous devez effectuer ces étapes uniquement si votre société est **nouvel accès à Marketo**. Si ce n’est pas le cas, la configuration peut déjà être effectuée.

Certaines étapes nécessitent l’aide de votre équipe informatique.

>[!TIP]
>
>Si vous [imprimer cette liste de contrôle](/help/marketo/getting-started/setup-steps/setup-checklist.md){target=&quot;_blank&quot;}, vous pouvez désactiver les éléments lorsque vous les terminez.

## Connexion et création d’utilisateurs Marketo supplémentaires {#log-in-and-create-additional-marketo-users}

1. Connexion à Marketo [here](https://app.marketo.com/){target=&quot;_blank&quot;} à l’aide des informations d’identification que vous avez reçues par courrier électronique.

   ![](assets/new-login-screen-hand.jpg)

Félicitations ! Vous êtes maintenant dans Marketo et vous pouvez commencer à explorer. Vous pouvez inviter vos collègues de l’équipe marketing à vous rejoindre. Pour ce faire, ajoutez de nouveaux utilisateurs.

Cliquez sur l&#39;icône **Admin**.

>[!TIP]
>
>Lorsque vous êtes ici, vous pouvez cliquer sur **Mon compte** pour modifier les paramètres de votre compte et de votre emplacement, ainsi qu’un nouveau nom d’abonnement.

![](assets/admin.png)

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Cliquez sur **Utilisateurs et rôles**.

![](assets/image2015-1-6-13-3a14-3a43.png)

Cliquez sur **Inviter un nouvel utilisateur**.

![](assets/image2015-1-6-13-3a14-3a6.png)

Renseignez l’adresse électronique, le prénom et le nom de votre collègue.

![](assets/image2016-5-24-10-3a11-3a12.png)

Vous pouvez éventuellement indiquer un motif pour l’invitation et une date d’expiration d’accès à l’aide du sélecteur de calendrier. Cliquez sur **OK**.

![](assets/image2016-5-24-10-3a13-3a9.png)

Cliquez sur **Suivant**.

![](assets/image2016-5-24-10-3a14-3a9.png)

>[!TIP]
>
>Une date d’expiration est idéale pour les parties prenantes ou les consultants externes à court terme, qui n’ont besoin de l’accès à Marketo que pour une courte période.

>[!NOTE]
>
>Lorsque la date d’expiration arrive, l’utilisateur reçoit une notification d’expiration et le compte est verrouillé.

Sélectionnez un rôle et cliquez sur **Suivant**. Les utilisateurs standard ont accès à toutes les zones, à l’exception d’Admin.

![](assets/image2016-5-24-10-3a14-3a51.png)

>[!NOTE]
>
>Outre les cinq rôles intégrés, vous pouvez également créer des rôles personnalisés. En savoir plus sur [Gestion des rôles et des autorisations des utilisateurs](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target=&quot;_blank&quot;}.

N’hésitez pas à modifier le texte de l’invitation. Cliquez sur **Envoyer**.

![](assets/image2016-5-24-10-3a15-3a52.png)

Le nouvel utilisateur est maintenant répertorié dans l’onglet Utilisateurs et doit recevoir un courrier électronique contenant un lien pour créer un mot de passe et un identifiant. Étape suivante !

![](assets/image2016-5-24-10-3a23-3a10.png)

## Configuration des contacts d’assistance autorisés {#set-up-your-authorized-support-contacts}

Vous avez peut-être reçu un courrier électronique du service clientèle de Marketo vous indiquant que vous êtes l’administrateur du service clientèle de Marketo pour votre entreprise. Si tel est le cas, vous pouvez configurer **contacts d’assistance autorisés** pour votre équipe. Seuls les contacts d’assistance autorisés peuvent contacter le service clientèle de Marketo directement par l’intermédiaire du [Portail d’assistance Marketo](https://support.marketo.com){target=&quot;_blank&quot;}.

>[!NOTE]
>
>Le nombre de contacts d’assistance que vous pouvez créer est déterminé par le package que vous avez acheté. Cette limite est spécifiée dans votre email auprès du support Marketo.

Les documents de contact de l’assistance autorisés ont été déplacés dans la communauté Marketo. Veuillez consulter [cet article](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target=&quot;_blank&quot;}.

>[!NOTE]
>
>Seules les personnes qui se sont connectées à la communauté Marketo apparaissent dans la liste. Si vous ne trouvez pas la personne, assurez-vous qu’elle se connecte d’abord à la communauté.

## Personnalisation des URL de votre page d’entrée avec un CNAME {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d’instructions de configuration informatique pendant votre appel de lancement.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Sélectionnez un CNAME pour vos landing pages. Quelques exemples :

    * **go**.[CompanyDomain].com
    * **www2**.[CompanyDomain].com
    * **lp**.[CompanyDomain].com

>[!TIP]
>
>Reste court ! Les URL plus courtes sont plus faciles à mémoriser. Nous suggérons &quot;go&quot; comme domaine.

La première partie (en gras) est la `[LandingPageCNAME]`. Vous en aurez besoin à l’étape 5.

Pour récupérer la chaîne de compte que vous allez remplacer par votre CNAME de page d’entrée, accédez à la zone d’administration.

![](assets/admin.png)

Cliquez sur **Pages de destination**.

![](assets/image2015-1-6-13-3a52-3a6.png)

Copiez la chaîne de compte des paramètres de la page d’entrée.

![](assets/image2015-1-6-13-3a53-3a19.png)

Il s’agit de la variable `[AccountString]`. Enregistrez-le. Vous devrez le donner au service informatique à l’étape 5.

Configurez les paramètres de votre domaine de sorte que les pages d’entrée utilisent le domaine de votre entreprise au lieu de celui de Marketo (où elles sont hébergées).

## Assurer la délivrabilité des emails {#ensure-email-deliverability}

>[!NOTE]
>
>Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d’instructions de configuration informatique pendant votre appel de lancement.

Vous pouvez prendre plusieurs mesures pour vous assurer que les emails atteignent le plus grand nombre possible de vos destinataires.

* **Marque vos liens de suivi**. Vous pouvez choisir un CNAME pour utiliser votre propre domaine (au lieu de celui de Marketo) dans les liens que vous incluez dans les courriers électroniques de Marketo. Cela renforce la marque de votre domaine et accroît la confiance et la délivrabilité de vos destinataires.
* **Ajoutez Marketo à la liste autorisée de messagerie de votre entreprise.** Il est recommandé d’envoyer des emails de test à vos comptes de test avant d’envoyer des emails à des personnes réelles. En plaçant sur la liste autorisée Marketo, vous pouvez empêcher que ces emails de test ne soient bloqués ou marqués comme spam.
* **Configurez SPF et DKIM.** Ces technologies assurent vos destinataires que vos emails Marketo ne sont pas des spams. Pour empêcher les filtres de spam des destinataires de rejeter les emails Marketo, procédez comme suit pour [Configuration d’un SPF et DKIM pour la délivrabilité de vos emails](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Configurez un enregistrement MX pour votre domaine.** Un enregistrement MX vous permet de recevoir du courrier électronique vers le domaine à partir duquel vous envoyez le courrier électronique pour traiter les réponses et les réponses automatiques. Si vous envoyez des messages depuis votre domaine d’entreprise, il est probable que vous ayez déjà configuré ce message. Si ce n’est pas le cas, vous pouvez généralement configurer le mappage à l’enregistrement MX de votre domaine d’entreprise.
* **Paramètres recommandés pour l’adresse de l’expéditeur.** Vous devez utiliser un domaine d’adresse électronique valide, existant et opérationnel dans l’ adresse de l’expéditeur de toutes les campagnes par e-mail. Il peut être bénéfique de configurer un sous-domaine de votre domaine d’entreprise plutôt que de l’envoyer depuis votre domaine d’entreprise. Cela permet de s’assurer que les problèmes de votre flux de messagerie d’entreprise n’ont pas d’incidence sur votre flux de messagerie Marketo et vice versa. De plus, envoyer du courrier depuis `something@nonexistentdomain.com` entraînera le filtrage ou le blocage des emails. Tout domaine utilisé dans l’adresse de l’expéditeur doit disposer d’un compte Postmaster@ et abuse@ valide.

Si vous utilisez les applications Google pour héberger votre adresse électronique d’entreprise, vous ne pourrez pas créer d’adresse électronique abuse@ ou postmaster@ sous votre domaine. Pour contourner ce problème, vous devez créer des groupes nommés &quot;abus&quot; et &quot;postmaster&quot;. Les utilisateurs membres de ces groupes recevront des emails envoyés à ces adresses (par exemple, postmaster@domain.com). Vous trouverez des instructions détaillées sur la création de groupes. [here](https://support.google.com/a/answer/33343#adminconsole){target=&quot;_blank&quot;}.

Choisissez un CNAME pour les liens de suivi des emails (choisissez un CNAME) _différent_ à partir du CNAME de la page d’entrée que vous avez choisi à l’étape 3). Quelques exemples :

* go2.[CompanyDomain].com
* em.[CompanyDomain].com
* wow.[CompanyDomain].com

La première partie est le CNAME de tracking des emails, `[EmailTrackingCNAME]`. Vous devrez le donner au service informatique à l’étape 5.

>[!CAUTION]
>
>Les CNAME de courrier électronique et de page d’entrée doivent être différents. Évitez également les CNAME tels que &quot;track&quot; ou &quot;link&quot;. Il est souvent signalé comme indésirable

Pour trouver votre lien de suivi Marketo, accédez au **Administration** zone.

![](assets/admin.png)

Cliquez sur **Email**.

![](assets/image2015-1-6-13-3a55-3a32.png)

Copiez le lien de suivi dans vos paramètres de courrier électronique.

Le lien de suivi se présente comme suit : `mkto-[a-z][4 digits].com`.

![](assets/email-tracking-link-hand.jpg)

C&#39;est votre `[MktoTrackingLink]`. Enregistrez-le. Vous devrez le donner au service informatique à l’étape 5.

Collectez les domaines &quot;From&quot;. Liste de tous les domaines &quot;De&quot; (comme dans, `[Sender]@[FromDomain].com`) que vous prévoyez d’utiliser pour envoyer des emails à partir de Marketo. Pour la plupart, il n&#39;y en a qu&#39;un.

Par exemple, &quot;marketo.com&quot;, &quot;info.marketo.com,&quot;. Voici les `[FromDomain1]`,`[FromDomain2]`, etc. Enregistrez-les. Vous devrez les transmettre à l’informatique à l’étape 5.

Vous disposez maintenant de toutes les informations dont vous avez besoin pour envoyer votre demande à l’informatique !

## Demander à l’informatique de configurer des protocoles {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d’instructions de configuration informatique pendant votre appel de lancement.

Une fois que vous avez collecté toutes les informations nécessaires, vous êtes prêt à envoyer une demande au service informatique. Vous pouvez utiliser le texte ci-dessous comme modèle, en remplaçant le texte en gras par vos propres informations.

[Inclure un lien vers cet article](/help/marketo/getting-started/setup-steps/configure-protocols-for-marketo.md).

Collez ce texte dans l’email et remplacez les espaces réservés en gras :

>[!NOTE]
>
>Voir les étapes 3 et 4 ci-dessus pour déterminer le texte à remplacer par les espaces réservés. N’oubliez pas que `[LandingPageCNAME]` et `[EmailTrackingCNAME]` doit être différent.

`---------------------------------------------`

Cher administrateur informatique génial,

Notre équipe marketing utilise désormais la plateforme Marketo pour communiquer avec nos clients. Pour garantir une bonne délivrabilité des emails, nous devons apporter les modifications suivantes :

`1)` Pour nos landing pages, ajoutez une entrée DNS (CNAME) pour **[LandingPageCNAME]**.**[CompanyDomain]**.com, pointant vers **[AccountString]**.mktoweb.com.

`2)` Pour nos liens de suivi dans les emails, ajoutez une entrée DNS (CNAME) pour **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, pointant vers **[MktoTrackingLink]**.

`3)` Placez sur la liste autorisée Marketo.

    * Si nous utilisons des adresses IP dans notre Liste autorisée de courriel, ajoutez les adresses IP répertoriées ci-dessous :
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    94.236.119.0/26

>[!NOTE]
>
>Contactez l’assistance Marketo si vous souhaitez obtenir une liste abrégée d’adresses IP à placer sur la liste autorisée spécifique à votre environnement.

    * Si notre système anti-spam utilise les domaines From, ajoutez ces éléments :

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Nous devons configurer SPF et DKIM afin que Marketo soit autorisé à envoyer des emails signés en notre nom.

`a.` Pour configurer SPF, ajoutez la ligne suivante à nos entrées DNS :

DANS TXT **[De domaine]**: v=spf1 mx ip4 :**[IP d’entreprise]**
<br/>inclure : mktomail.com ~all

Si nous avons déjà un enregistrement SPF existant dans notre entrée DNS, ajoutez-y simplement les éléments suivants :

include:mktomail.com

`[`Remplacer **De domaine** avec votre Email From Domain (par exemple : company.com) et **CorpIP** avec l’adresse IP de votre serveur de messagerie d’entreprise (par exemple : 255.255.255.255).  Si vous souhaitez envoyer des emails à partir de plusieurs domaines via Marketo, demandez à votre personnel informatique d’ajouter cette ligne pour chaque domaine (sur une seule ligne).`]`

`b.` Pour DKIM, créez des enregistrements de ressource DNS pour chaque domaine que nous souhaitons configurer. Vous trouverez ci-dessous les enregistrements d’hôte et les valeurs TXT pour chaque domaine pour lequel nous allons signer :

**`[DKIMDomain1]`**: L’enregistrement de l’hôte **`[HostRecord1]`** et la valeur TXT est **[TXTValue1]**.

**`[DKIMDomain2]`**: L’enregistrement de l’hôte **`[HostRecord2]`** et la valeur TXT est **`[TXTValue2]`**.

`[`Copiez le **HostRecord** et **TXTValue** pour chaque **DKIMDomain** vous avez effectué la configuration après avoir suivi la [instructions ici](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). N’oubliez pas de vérifier chaque domaine dans **Admin > Email > DKIM** une fois que votre personnel informatique a terminé cette étape.`]`

`5)` Nous devons nous assurer qu’il existe un enregistrement MX valide pour nos domaines FROM **[FromDomain1]**, **[FromDomain2]**, etc. Pouvez-vous confirmer ? Si ce n’est pas le cas, configurez pour mapper à notre enregistrement MX de domaine d’entreprise. Cela nous permettra de traiter les réponses/réponses aux messages Marketo.

Faites-moi savoir quand vous avez terminé ces étapes, de sorte que je puisse terminer le processus de configuration avec Marketo.

Merci! Tu es la meilleure !

L&#39;amour,

**`[Your Name]`**

`---------------------------------------------`

Envoyez l’e-mail au service informatique. Nous comprenons qu’il peut s’écouler un certain temps avant que l’informatique puisse réaliser ces tâches. Vous pouvez passer à l’étape 7, mais n’oubliez pas que vous devez renvoyer l’étape 6 pour terminer la configuration de Marketo.

## Terminer la configuration de Marketo une fois l’informatique terminée {#complete-your-marketo-setup-after-it-finishes}

Une fois les tâches du service informatique terminées, procédez comme suit pour ajouter votre landing page et vos CNAME de messagerie, et activer la signature DKIM.

Accédez au **Administration** zone pour ajouter votre CNAME de page d’entrée

![](assets/admin.png)

Sélectionnez Landing Pages , puis cliquez sur **Modifier** dans la zone Paramètres .

![](assets/image2015-1-6-13-3a59-3a15.png)

Saisissez votre nouveau nom de domaine dans le champ Nom de domaine pour les landing pages. Cela doit se présenter comme suit :

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/image2015-1-6-14-3a3-3a6.png)

Dans le champ Page de secours , saisissez l’URL à laquelle vous souhaitez que les utilisateurs accèdent en cas d’indisponibilité d’une landing page. Vous pouvez utiliser la page d’accueil de votre société si vous ne disposez pas d’une page de secours. Dans le champ Page d’accueil , saisissez le site web de votre société.

![](assets/image2015-1-6-14-3a2-3a46.png)

Dans la zone Admin, sélectionnez Courrier électronique pour ajouter votre CNAME de messagerie

![](assets/image2015-1-6-14-3a5-3a3.png)

Faites défiler la page vers le bas et cliquez sur **Modifier**.

![](assets/edit-branding-domain.png)

Dans le champ Domaine , saisissez votre domaine de tracking email. Cela doit se présenter comme suit :

`[EmailTrackingCNAME].[CompanyDomain].com`. Cliquez sur **Enregistrer**.

![](assets/new-branding-domain-9-1.png)

## Intégration de votre CRM {#integrate-your-crm}

Il s’agit probablement de l’étape la plus passionnante de votre configuration. Il est temps de remplir Marketo avec tous les prospects et contacts que vous avez stockés dans votre CRM !

Choisissez l’un des éléments suivants en fonction du CRM utilisé par votre entreprise.

    * [Intégration de Marketo à Salesforce.com](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Intégration de Marketo à Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Pour effectuer ces étapes, vous avez besoin de l’aide de l’administrateur CRM de votre entreprise.

## Ajout du code de suivi à votre site web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira des instructions de code Munchkin dans votre document d’instructions de configuration informatique.

Marketo dispose d’un code JavaScript de suivi personnalisé (appelé Munchkin) que vous pouvez utiliser pour effectuer le suivi des activités de personnes sur n’importe quelle page web. Munchkin est requis pour intégrer votre site web à Marketo. Suivez ces étapes pour [Ajout du code de suivi Munchkin à votre site web](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target=&quot;_blank&quot;}.

>[!NOTE]
>
>Expérience avec HTML requise pour ajouter le code de suivi.

Toutes les étapes de configuration sont terminées. Il ne reste qu&#39;à plonger et à utiliser Marketo !
