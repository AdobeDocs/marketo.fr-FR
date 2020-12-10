---
unique-page-id: 2949469
description: Etapes de configuration - Documents marketing - Documentation du produit
title: Etapes de configuration
translation-type: tm+mt
source-git-commit: 0a4050545c5c956001c9c299cfbcf59e9cffd39c
workflow-type: tm+mt
source-wordcount: '2143'
ht-degree: 0%

---


# Etapes de configuration {#setup-steps}

**Bienvenue sur le marché !**

Avant de vous plonger dans l&#39;utilisation de Marketo, vous devez effectuer quelques étapes.

Ces étapes comprennent :

* configuration de compte de base
* personnaliser vos URL de landing page et vos liens de courriel pour améliorer la confiance et la délivrabilité
* synchronisation de la gestion de la relation client
* ajout d’un code de suivi à votre site Web d’entreprise

>[!NOTE]
>
>Vous devez effectuer ces étapes uniquement si votre société est **nouvelle sur Marketing**. Si ce n&#39;est pas le cas, la configuration peut déjà être effectuée.

Certaines étapes nécessitent l&#39;aide de votre équipe informatique.

>[!TIP]
>
>Si vous [imprimez cette liste](/help/marketo/getting-started/setup-steps/setup-checklist.md), vous pouvez cocher les éléments au fur et à mesure que vous les terminez.

1. Connexion et création d’autres utilisateurs du marketing

1. Connectez-vous à Marketo [ici](https://app.marketo.com/) à l’aide des informations d’identification que vous avez reçues par courrier électronique.

   ![](assets/new-login-screen-hand.jpg)

Félicitations ! Vous êtes maintenant à Marketo et pouvez début à explorer. Vous pouvez inviter vos collègues de l’équipe marketing à vous rejoindre. Pour ce faire, ajoutez de nouveaux utilisateurs.

Accédez à la zone **Admin** .

>[!TIP]
>
>Lorsque vous êtes ici, vous pouvez cliquer sur **Mon compte** pour modifier les paramètres de votre compte et de votre emplacement, ainsi que définir un nouveau nom d’abonnement.

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

Vous pouvez éventuellement saisir un motif pour l&#39;invitation et une date d&#39;expiration d&#39;accès à l&#39;aide du sélecteur de calendrier. Cliquez sur **OK**.

![](assets/image2016-5-24-10-3a13-3a9.png)

Cliquez sur **Suivant**.

![](assets/image2016-5-24-10-3a14-3a9.png)

>[!TIP]
>
>Une date d’expiration est idéale pour les parties prenantes externes ou les consultants à court terme, qui ont besoin de Marketing pour accéder à Markepour une courte période.

>[!NOTE]
>
>Lorsque la date d’expiration arrive, l’utilisateur reçoit une notification d’expiration et le compte est verrouillé.

Sélectionnez un rôle et cliquez sur **Suivant**. Les utilisateurs standard ont accès à toutes les zones, à l’exception de l’administrateur.

![](assets/image2016-5-24-10-3a14-3a51.png)

>[!NOTE]
>
>Outre les cinq rôles intégrés, vous pouvez également créer des rôles personnalisés. En savoir plus sur la [gestion des rôles et des autorisations](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)des utilisateurs.

N’hésitez pas à modifier le texte de l’invitation. Cliquez sur **Envoyer**.

![](assets/image2016-5-24-10-3a15-3a52.png)

Le nouvel utilisateur est désormais répertorié dans l’onglet Utilisateurs et doit recevoir un courrier électronique contenant un lien permettant de créer un mot de passe et une connexion. Prochaine étape !

![](assets/image2016-5-24-10-3a23-3a10.png)

1. Configuration de vos contacts d&#39;assistance autorisés

   Vous avez peut-être reçu un courrier électronique de l’assistance marketing vous indiquant que vous êtes l’administrateur du service clientèle de Marketo pour votre société. Si tel est le cas, vous pouvez configurer des contacts **d&#39;assistance** autorisés pour votre équipe. Seuls les contacts d&#39;assistance autorisés peuvent contacter l&#39;assistance clientèle de Marketo directement via le portail [d&#39;assistance](https://support.marketo.com)Marketo.

   >[!NOTE]
   >
   >Le nombre de contacts d&#39;assistance que vous pouvez créer est déterminé par le pack que vous avez acheté. Cette limite est spécifiée dans votre courrier électronique de la part de l’assistance marketing.

   Les documents de contact d&#39;assistance autorisés ont été déplacés vers la communauté Marketo. Veuillez consulter [cet article](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341).

   >[!NOTE]
   >
   >Seules les personnes qui se sont connectées à la communauté Marketo apparaissent dans la liste. Si vous ne trouvez pas la personne, assurez-vous qu&#39;elle se connecte d&#39;abord à la Communauté.

1. Personnaliser vos URL de Landing page avec un CNAME

   >[!NOTE]
   >
   >Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d&#39;instructions de configuration informatique pendant votre appel de lancement.

   >[!NOTE]
   >
   >**Autorisations d’administrateur requises**

   Choisissez un CNAME pour vos landings page. En voici quelques exemples :

   * **allez**.[CompanyDomain].com
   * **www2**.[CompanyDomain].com
   * **lp**.[CompanyDomain].com

   >[!TIP]
   >
   >Restez court ! Les URL plus courtes sont plus faciles à mémoriser. Nous suggérons &quot;go&quot; comme domaine.

   La première partie (en gras) est la `[LandingPageCNAME]`. Vous en aurez besoin à l’étape 5.

   Pour récupérer la chaîne de compte que vous allez remplacer par votre CNAME de landing page, accédez à la zone Admin.

   ![](assets/admin.png)

   Cliquez sur **Landings page**.

   ![](assets/image2015-1-6-13-3a52-3a6.png)

   Copiez la chaîne de compte des paramètres du landing page.

   ![](assets/image2015-1-6-13-3a53-3a19.png)

   C&#39;est le `[AccountString]`. Enregistrez-la. Vous devrez le transmettre au service informatique à l&#39;étape 5.

Configurez les paramètres de votre domaine de sorte que les landings page utilisent le domaine de votre société plutôt que celui de Marketo (où ils sont hébergés).

1. Garantir la délivrabilité du courrier électronique

   >[!NOTE]
   >
   >Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d&#39;instructions de configuration informatique pendant votre appel de lancement.

   Vous pouvez prendre plusieurs mesures pour vous assurer que les courriels atteignent le plus grand nombre possible de personnes.

   1. **Marquez vos liens** de suivi. Vous pouvez choisir un CNAME pour utiliser votre propre domaine (au lieu de celui de Marketo) dans les liens que vous incluez dans les courriers électroniques de Marketo. Cela renforce la marque de votre domaine et augmente la confiance et la délivrabilité avec vos destinataires.
   1. **Ajoutez Marketo à votre liste autorisée de messagerie d’entreprise.** Il est généralement recommandé d’envoyer des e-mails de test à vos comptes de test avant d’envoyer des e-mails à des personnes réelles. En plaçant sur la liste autorisée Marketo, vous pouvez empêcher que ces courriels de test ne soient bloqués ou marqués comme spam.
   1. **Configurez SPF et DKIM.** Ces technologies garantissent à vos destinataires que vos courriels Marketo ne sont pas des spams. Pour éviter que les filtres de spam des destinataires ne vous rejettent les courriers électroniques de Marketo, suivez ces étapes pour [configurer un SPF et un DKIM pour la diffusion](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md)de vos courriels.
   1. **Configurez un enregistrement MX pour votre domaine.** Un enregistrement MX vous permet de recevoir du courrier au domaine à partir duquel vous envoyez du courrier électronique pour traiter les réponses et les répondeurs automatiques. Si vous envoyez des données à partir de votre domaine d’entreprise, il est probable que vous ayez déjà configuré cette option. Dans le cas contraire, vous pouvez généralement configurer la mise en correspondance avec l’enregistrement MX de votre domaine d’entreprise.
   1. **Paramètres recommandés pour l’adresse de départ.** Vous devez utiliser un domaine de courriel valide, existant et fonctionnel dans l’adresse de départ de toutes les campagnes par courriel. Il peut s’avérer utile de configurer un sous-domaine de votre domaine d’entreprise plutôt que de l’envoyer à partir de votre domaine d’entreprise. Cela permet de s&#39;assurer que les problèmes provenant de votre flux de courrier d&#39;entreprise n&#39;affectent pas votre flux de courrier marketing et vice versa. En outre, l&#39;envoi de courrier à partir de something@nonexistentdomain.com entraînera le filtrage ou le blocage des courriers électroniques. Tout domaine utilisé dans l&#39;adresse de l&#39;expéditeur doit avoir un compte valide et fonctionnel de postmaster@ et abuse@.
Si vous utilisez Google Apps pour héberger vos courriels d&#39;entreprise, vous ne pourrez pas créer de courriels &quot;abuse@&quot; ou &quot;postmaster@&quot; sous votre domaine. Pour contourner ce problème, vous devez créer des groupes nommés &quot;abus&quot; et &quot;maître de poste&quot;. Les utilisateurs qui sont membres de ces groupes recevront des courriels envoyés à ces adresses (par exemple, postmaster@domain.com). Vous trouverez des instructions détaillées sur la création de groupes [ici](https://support.google.com/a/answer/33343#adminconsole).

   Choisissez un CNAME pour les liens de tracking email (choisissez un CNAME _différent_ du CNAME de landing page choisi à l’étape 3). En voici quelques exemples :

   * go2.[CompanyDomain].com
   * em.[CompanyDomain].com
   * wow.[CompanyDomain].com

   La première partie est le CNAME tracking email, `[EmailTrackingCNAME]`. Vous devrez le transmettre au service informatique à l&#39;étape 5.

   >[!CAUTION]
   >
   >Les CNAME de courriel et de Landing page doivent être différents. Evitez également les CNAME tels que &quot;track&quot; ou &quot;link&quot;. Il est souvent signalé comme indésirable

   Pour trouver votre lien de suivi Marketo, accédez à la zone **Admin** .

   ![](assets/admin.png)

   Cliquez sur **Courriel**.

   ![](assets/image2015-1-6-13-3a55-3a32.png)

   Copiez le lien de suivi de vos paramètres de courrier électronique.

   Le lien de suivi se présente sous la forme suivante : `mkto-[a-z][4 digits].com`.

   ![](assets/email-tracking-link-hand.jpg)

   C&#39;est votre `[MktoTrackingLink]`. Enregistrez-la. Vous devrez le transmettre au service informatique à l&#39;étape 5.

   Collectez &quot;De&quot; domaines. Effectuez une liste de tous les domaines &quot;De&quot; (comme dans, `[Sender]@[FromDomain].com`) que vous prévoyez d’utiliser pour envoyer des courriers électroniques à partir de Marketing Cloud. Pour la plupart, il n&#39;y en a qu&#39;un.

   Par exemple, &quot;marketo.com&quot;, &quot;info.marketo.com,&quot;. Ce sont `[FromDomain1]`,`[FromDomain2]`etc. Sauvez-les. Vous devrez les transmettre à l&#39;équipe informatique à l&#39;étape 5.

   Vous disposez maintenant de toutes les informations nécessaires pour envoyer votre demande à l&#39;informatique !

1. Demander au service informatique de configurer des protocoles

   >[!NOTE]
   >
   >Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d&#39;instructions de configuration informatique pendant votre appel de lancement.

   Une fois que vous avez collecté toutes les informations nécessaires, vous êtes prêt à envoyer une demande à l&#39;équipe informatique. Vous pouvez utiliser le texte ci-dessous comme modèle, en remplaçant le texte en gras par vos propres informations.

   [Incluez un lien vers cet article](/help/marketo/getting-started/setup-steps/configure-protocols-for-marketo.md).

   Collez ce texte dans le courrier électronique et remplacez les espaces réservés en gras :

   >[!NOTE]
   >
   >Voir les étapes 3 et 4 ci-dessus pour déterminer le texte à utiliser pour remplacer les espaces réservés. Rappelez-vous que `[LandingPageCNAME]` et `[EmailTrackingCNAME]` doit être différent.

`---------------------------------------------`

Cher administrateur informatique stupéfiant,

Notre équipe marketing utilise maintenant la plate-forme Marketo pour communiquer avec notre personnel. Pour garantir une excellente délivrabilité des courriers électroniques, nous devons apporter les modifications suivantes :

`1)` Pour nos landings page, ajoutez une entrée DNS (CNAME) pour **[LandingPageCNAME]**.**[CompanyDomain]**.com, pointant vers **[AccountString]**.mktoweb.com.

`2)` Pour nos liens de suivi dans le courrier électronique, ajoutez une entrée DNS (CNAME) pour **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, pointant vers **[MktoTrackingLink]**.

`3)` Placer sur la liste autorisée le marketing.

    * Si nous utilisons des adresses IP dans notre Liste autorisée de courriel, ajoutez les adresses IP répertoriées ci-dessous :
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.htm94.ails
    
    

REMARQUE : Contactez l’assistance marketing si vous souhaitez qu’une liste abrégée d’adresses IP place sur la liste autorisée spécifique à votre environnement.

    * Si notre système antispam utilise les domaines De, ajoutez les éléments suivants :

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Nous devons configurer SPF et DKIM pour que Marketo soit autorisé à envoyer des courriels signés en notre nom.

`a.` Pour configurer SPF, veuillez ajouter la ligne suivante à nos entrées DNS :

DANS TXT **[du domaine]**:  v=spf1 mx ip4:IP(s)**[d’entreprise]**<br/>comprennent : mktomail.com ~all

Si notre entrée DNS contient déjà un enregistrement SPF existant, il suffit d&#39;y ajouter les éléments suivants :

include:mktomail.com

`[`Remplacer **du domaine** par votre adresse électronique du domaine (ex. : société.com) et **CorpIP** avec l’adresse IP de votre serveur de messagerie d’entreprise (ex : 255.255.255.255).  Si vous souhaitez envoyer des courriers électroniques à partir de plusieurs domaines via Marketo, votre personnel informatique doit ajouter cette ligne pour chaque domaine (sur une seule ligne).`]`

`b.` Pour DKIM, créez des enregistrements de ressources DNS pour chaque domaine que nous aimerions configurer. Vous trouverez ci-dessous les enregistrements d’hôtes et les valeurs TXT pour chaque domaine pour lequel nous allons signer :

**`[DKIMDomain1]`**: L’enregistrement hôte est **`[HostRecord1]`** défini et la valeur TXT est **[TXTValue1]**.

**`[DKIMDomain2]`**: L’enregistrement hôte est **`[HostRecord2]`** défini et la valeur TXT est **`[TXTValue2]`** définie.

`[`Copiez l’enregistrement **hôte** et la valeur **** TXTV **pour chaque domaine** DKIMD [que vous avez configuré après avoir suivi lesinstructions ici. ](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md) N’oubliez pas de vérifier chaque domaine dans **Admin > Email > DKIM** une fois que votre personnel informatique a terminé cette étape.`]`

`5)` Nous devons nous assurer qu&#39;il existe un enregistrement MX valide pour nos domaines FROM **[FromDomain1]**, **[FromDomain2]**, etc. Pouvez-vous confirmer ? Si ce n&#39;est pas le cas, configurez-le pour qu&#39;il corresponde à notre enregistrement MX de domaine d&#39;entreprise. Ceci nous permettra de traiter les réponses/répondeurs automatiques à nos envois Marketo.

Dites-moi quand vous avez terminé ces étapes, afin que je puisse terminer la procédure de configuration avec Marketo.

Merci ! Tu es la meilleure !

Amour,

**`[Your Name]`**

`---------------------------------------------`

Envoyez le courriel au service informatique. Nous comprenons qu&#39;il peut s&#39;écouler un certain temps avant que l&#39;informatique puisse achever ces tâches. Vous pouvez passer à l’étape 7, mais n’oubliez pas que vous devez renvoyer l’étape 6 pour terminer la configuration de Marketing Cloud.

1. Terminer la configuration de Marketing Suite à la fin de l&#39;informatique

   Une fois que le service informatique a terminé ses tâches, procédez comme suit pour ajouter vos CNAME de landing page et de courrier électronique et pour activer la signature DKIM.

   Accédez à la zone **Admin** pour Ajouter votre CNAME de Landing page.

   ![](assets/admin.png)

   Sélectionnez Landings page, puis cliquez sur **Modifier** dans la zone Paramètres.

   ![](assets/image2015-1-6-13-3a59-3a15.png)

   Entrez votre nouveau nom de domaine dans le champ Nom de domaine pour les Landings page. Il doit se présenter comme suit :

   `[LandingPageCNAME].[CompanyDomain].com`

   ![](assets/image2015-1-6-14-3a3-3a6.png)

   Dans le champ Page de secours, saisissez l’URL à laquelle vous souhaitez que les utilisateurs accèdent en cas d’indisponibilité d’un landing page. Vous pouvez utiliser votre page d&#39;accueil de société si vous ne disposez pas d’une page de secours. Dans le champ Page d&#39;accueil, entrez votre site Web de société.

   ![](assets/image2015-1-6-14-3a2-3a46.png)

   Dans la zone Admin, sélectionnez Courriel pour Ajouter votre CNAME de messagerie.

   ![](assets/image2015-1-6-14-3a5-3a3.png)

   Faites défiler la page vers le bas et cliquez sur **Modifier**.

   ![](assets/edit-branding-domain.png)

   Dans le champ Domaine, entrez votre domaine de tracking email. Il doit se présenter comme suit :

   `[EmailTrackingCNAME].[CompanyDomain].com`. Cliquez sur **Enregistrer**.

   ![](assets/new-branding-domain-9-1.png)

1. Envoyer une URL pour les modèles de Landing page et de courriel

   Nos concepteurs créatifs peuvent vous fournir des modèles personnalisés de landing page et de courrier électronique qui vous permettent de lancer vos programmes marketing rapidement et facilement. Vous devez leur fournir certaines informations afin qu’ils puissent faire correspondre les modèles au site Web et au logo de votre société.

   >[!NOTE]
   >
   >Ces modèles personnalisés ne sont disponibles que pour les clients Launch Pack.

   Accédez au formulaire Conception et création [de modèles](http://pages2.marketo.com/CESubmit-URL-ForTemplates.html) Marketo. Renseignez les informations de votre société.

   ![](assets/image2014-9-12-11-3a4-3a55.png)

   Pour l’URL de votre Landing page, saisissez un exemple d’URL du site Web de votre société qui indique les couleurs, le logo et le style de votre société. La plupart des clients utilisent une page Contactez-nous qui inclut un formulaire.

   ![](assets/image2014-9-12-11-3a5-3a7.png)

   Pour CNAME, saisissez le landing page CNAME que vous avez sélectionné à l’étape 3 (`[LandingPageCNAME]`). Envoyez votre demande.

   ![](assets/image2014-9-12-11-3a5-3a17.png)

   >[!NOTE]
   >
   >Vos modèles ne peuvent pas être terminés tant que votre service informatique n’a pas créé un enregistrement DNS pour votre CNAME de landing page.

   C&#39;est tout ! Vos nouveaux modèles devraient s’afficher dans Marketo Design Studio dans 3 à 5 jours ouvrables.

1. Intégration de votre gestion de la relation client

   C&#39;est probablement l&#39;étape la plus excitante de votre configuration - il est temps de remplir Marketo avec tous les prospects et contacts que vous avez stockés dans votre CRM !

   Choisissez l’une des options suivantes, en fonction de la gestion de la relation client utilisée par votre société.

   * [Intégrer Marketo avec Salesforce.com](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
   * [Intégration de Marketo avec Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

   >[!NOTE]
   >
   >Vous avez besoin de l’aide de l’administrateur CRM de votre société pour effectuer ces étapes.

## 9. Ajoutez le code de suivi sur votre site Web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira des instructions de code Munchkin dans votre document d&#39;instructions de configuration informatique.

Marketo comporte un code JavaScript de suivi personnalisé (appelé Munchkin) que vous pouvez utiliser pour suivre les activités de personnes sur n’importe quelle page Web. Munchkin doit intégrer votre site Web dans Marketo. Suivez ces étapes pour [Ajouter le code de suivi Munchkin à votre site Web](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).

>[!NOTE]
>
>Expérience avec du code HTML requise pour ajouter le code de suivi.

Toutes les étapes de configuration sont terminées. Il ne reste plus qu&#39;à plonger et utiliser le Marketo !
