---
unique-page-id: 2949469
description: Procédure de configuration - Documents Marketo - Documentation du produit
title: Étapes de configuration
hide: true
hidefromtoc: true
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
feature: Getting Started
source-git-commit: d41a43d7579775c0c866e867f778962ff61ff044
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 0%

---

# Étapes de configuration {#setup-steps}

**Bienvenue dans Adobe Marketo Engage !**

Avant d’utiliser Marketo, vous devez effectuer quelques étapes.

Ces étapes incluent :

* Configuration de compte de base
* Identifier les URL de votre landing page et les liens des emails pour améliorer la confiance et la délivrabilité
* Synchronisation de votre CRM
* Ajout de code de suivi au site web de votre entreprise

>[!NOTE]
>
>Vous devez effectuer ces étapes uniquement si votre société est **nouvelle version de Marketo**. Si ce n’est pas le cas, la configuration peut déjà être effectuée.

Certaines étapes nécessitent l’aide de votre équipe informatique.

>[!TIP]
>
>Si vous [imprimez cette liste de contrôle](/help/marketo/getting-started/initial-setup/setup-checklist.md){target="_blank"}, vous pouvez désactiver les éléments lorsque vous les terminez.

## Connexion et création d’utilisateurs Marketo supplémentaires {#log-in-and-create-additional-marketo-users}

>[!IMPORTANT]
>
>Si votre abonnement Marketo a été créé le ou après le 31 juillet 2023 ou a déjà été migré vers [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}, les étapes d’ajout d’un utilisateur décrites ci-dessous ne s’appliquent pas à vous. Veuillez plutôt consulter [cet article](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"} .

Connectez-vous à Marketo [ici](https://app.marketo.com/){target="_blank"} à l’aide des informations d’identification que vous avez reçues par courrier électronique.

![](assets/setup-steps-1.png)

Félicitations ! Vous êtes maintenant dans Marketo et pouvez commencer à explorer. Vous pouvez inviter vos collègues de l’équipe marketing à vous rejoindre. Pour ce faire, ajoutez de nouveaux utilisateurs.

Accédez à la zone **[!UICONTROL Admin]**.

>[!TIP]
>
>Pendant que vous êtes là, vous pouvez cliquer sur **[!UICONTROL Mon compte]** pour modifier les paramètres de votre compte et de votre emplacement, ainsi que définir un nouveau nom d’abonnement.

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

![](assets/setup-steps-3.png)

Cliquez sur **[!UICONTROL Inviter un nouvel utilisateur]**.

![](assets/setup-steps-4.png)

Renseignez l’adresse électronique, le prénom et le nom de votre collègue. _La définition d&#39;une date d&#39;expiration d&#39;accès est facultative_. Cliquez sur **[!UICONTROL Suivant]**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>Une date d’expiration est idéale pour les parties prenantes externes à court terme ou les consultants qui n’ont besoin de l’accès à Marketo que pour une courte période.

>[!NOTE]
>
>Lorsque la date d’expiration arrive, l’utilisateur reçoit une notification d’expiration et le compte est verrouillé.

Sélectionnez un rôle et cliquez sur **[!UICONTROL Suivant]**. Les utilisateurs standard ont accès à toutes les zones, à l’exception d’Admin.

![](assets/setup-steps-6.png)

>[!NOTE]
>
>Outre les cinq rôles intégrés, vous pouvez également créer des rôles personnalisés. En savoir plus sur la [gestion des rôles et autorisations des utilisateurs](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.

N’hésitez pas à modifier le texte de l’invitation. Cliquez sur **Send**.

![](assets/setup-steps-7.png)

Le nouvel utilisateur est maintenant répertorié dans l’onglet **[!UICONTROL Utilisateurs]** et doit recevoir un courrier électronique contenant un lien pour créer un mot de passe et un identifiant. Étape suivante !

![](assets/setup-steps-8.png)

## Configuration des contacts d’assistance autorisés {#set-up-your-authorized-support-contacts}

Vous avez peut-être reçu un courrier électronique du service clientèle de Marketo vous indiquant que vous êtes l’administrateur du service clientèle de Marketo pour votre entreprise. Si c&#39;est le cas, vous pouvez configurer des **contacts d&#39;assistance autorisés** pour votre équipe. Seuls les contacts d’assistance autorisés peuvent contacter le service clientèle de Marketo directement via le [Portail d’assistance de Marketo](https://support.marketo.com){target="_blank"}.

>[!NOTE]
>
>Le nombre de contacts d’assistance que vous pouvez créer est déterminé par le package que vous avez acheté. Cette limite est spécifiée dans votre email auprès du support Marketo.

Les documents de contact de l’assistance autorisés ont été déplacés dans la communauté Marketo. Consultez [cet article](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}.

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

La première partie (en gras) est le `[LandingPageCNAME]`. Vous en aurez besoin à l’étape 5.

Pour récupérer l’ID Munchkin que vous allez remplacer par votre CNAME de page d’entrée, accédez à la zone d’administration.

![](assets/setup-steps-9.png)

Cliquez sur **Mon compte**.

![](assets/setup-steps-10.png)

Copiez la [!UICONTROL chaîne de compte] des paramètres de la page d’entrée.

![](assets/setup-steps-11.png)

Il s’agit du `[Munchkin ID]`. Enregistrez-le. Vous devrez le donner au service informatique à l’étape 5.

Configurez les paramètres de votre domaine de sorte que les landing pages utilisent le domaine de votre entreprise au lieu de Marketo (où elles sont hébergées).

## Assurer la délivrabilité des emails {#ensure-email-deliverability}

>[!NOTE]
>
>Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d’instructions de configuration informatique pendant votre appel de lancement.

Vous pouvez prendre plusieurs mesures pour vous assurer que les emails atteignent le plus grand nombre possible de vos destinataires.

* **Marquez vos liens de suivi**. Vous pouvez choisir un CNAME pour utiliser votre propre domaine (au lieu de Marketo) dans les liens que vous incluez dans les courriers électroniques de Marketo. Cela renforce la marque de votre domaine et accroît la confiance et la délivrabilité de vos destinataires.
* **Ajoutez Marketo à la liste autorisée de messagerie de votre entreprise.** Il est généralement recommandé d’envoyer des emails de test à vos comptes de test avant d’envoyer des emails à des personnes réelles. En plaçant sur la liste autorisée Marketo, vous pouvez empêcher que ces emails de test ne soient bloqués ou marqués comme spam.
* **Configurez SPF et DKIM.** Ces technologies assurent vos destinataires que vos emails Marketo ne sont pas des spams. Pour empêcher les filtres de spam des destinataires de rejeter vos emails Marketo, procédez comme suit pour [Configurer un SPF et DKIM pour votre délivrabilité des emails](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Configurez un enregistrement MX pour votre domaine.** Un enregistrement MX vous permet de recevoir du courrier électronique vers le domaine à partir duquel vous envoyez le courrier électronique pour traiter les réponses et les réponses automatiques. Si vous envoyez depuis votre domaine d’entreprise, il est probable que celui-ci soit déjà configuré. Si ce n’est pas le cas, vous pouvez généralement configurer pour mapper l’enregistrement MX de votre domaine d’entreprise.
* **Paramètres recommandés pour l’adresse de l’expéditeur.** Vous devez utiliser un domaine de messagerie valide, existant et opérationnel dans l’adresse de l’expéditeur de toutes les campagnes par e-mail. Il peut être bénéfique de configurer un sous-domaine de votre domaine d’entreprise plutôt que de l’envoyer depuis votre domaine d’entreprise. Cela permet de s’assurer que les problèmes provenant de votre flux de messagerie d’entreprise n’ont pas d’incidence sur votre flux de messagerie Marketo et vice versa. De plus, l’envoi de courrier à partir de `something@nonexistentdomain.com` entraînera le filtrage ou le blocage des emails. Tout domaine utilisé dans l’adresse de l’expéditeur doit disposer d’un compte Postmaster@ et abuse@ valide.

Si vous utilisez les applications Google pour héberger votre adresse électronique d’entreprise, vous ne pourrez pas créer d’adresse électronique abuse@ ou postmaster@ sous votre domaine. Pour contourner ce problème, vous devez créer des groupes nommés &quot;abus&quot; et &quot;postmaster&quot;. Les utilisateurs membres de ces groupes recevront des emails envoyés à ces adresses (par exemple, postmaster@domain.com). Vous trouverez des instructions détaillées sur la création de groupes [ici](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Choisissez un CNAME pour les liens de suivi des emails (choisissez un CNAME _différent_ de la page d’entrée CNAME que vous avez choisie à l’étape 3). Quelques exemples :

* go2.[CompanyDomain].com
* em.[CompanyDomain].com
* wow.[CompanyDomain].com

La première partie est le CNAME de suivi des emails, `[EmailTrackingCNAME]`. Vous devrez le donner au service informatique à l’étape 5.

>[!CAUTION]
>
>Les CNAME de courrier électronique et de page d’entrée doivent être différents. Évitez également les CNAME tels que &quot;track&quot; ou &quot;link&quot;. Il est souvent signalé comme indésirable

Pour trouver votre lien de suivi Marketo, accédez à la zone **[!UICONTROL Admin]**.

![](assets/setup-steps-12.png)

Cliquez sur **[!UICONTROL Email]**.

![](assets/setup-steps-13.png)

Copiez le [!UICONTROL Lien de suivi] de vos paramètres de courrier électronique.

Le [!UICONTROL Lien de suivi] se présente sous la forme : `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Il s’agit de votre `[MktoTrackingLink]`. Enregistrez-le. Vous devrez le donner au service informatique à l’étape 5.

Collectez les domaines &quot;From&quot;. Faites la liste de tous les domaines &quot;De&quot; (comme dans `[Sender]@[FromDomain].com`) que vous prévoyez d’utiliser pour envoyer des emails à partir de Marketo. Pour la plupart, il n&#39;y en a qu&#39;un.

Par exemple, &quot;marketo.com&quot;, &quot;info.marketo.com&quot;. Il s’agit de `[FromDomain1]`,`[FromDomain2]`, etc. Enregistrez-les. Vous devrez les transmettre à l’informatique à l’étape 5.

Vous disposez maintenant de toutes les informations dont vous avez besoin pour envoyer votre demande à l’informatique !

## Demander à l’informatique de configurer des protocoles {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Êtes-vous client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d’instructions de configuration informatique pendant votre appel de lancement.

Une fois que vous avez collecté toutes les informations nécessaires, vous êtes prêt à envoyer une demande au service informatique. Vous pouvez utiliser le texte ci-dessous comme modèle, en remplaçant le texte en gras par vos propres informations.

[Incluez un lien vers cet article](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

Collez ce texte dans l’email et remplacez les espaces réservés en gras :

>[!NOTE]
>
>Voir les étapes 3 et 4 ci-dessus pour déterminer le texte à remplacer par les espaces réservés. N’oubliez pas que `[LandingPageCNAME]` et `[EmailTrackingCNAME]` doivent être différents.

`----------------------------------------------`

Cher administrateur informatique génial,

Notre équipe marketing utilise désormais la plateforme Marketo pour communiquer avec nos clients. Pour garantir une bonne délivrabilité des emails, nous devons apporter les modifications suivantes :

`1)` Pour nos landing pages, ajoutez une entrée DNS (CNAME) pour **[LandingPageCNAME]**.**[CompanyDomain]**.com, pointant vers **[Munchkin ID]**.mktoweb.com.

`2)` Pour les liens de suivi dans le courrier électronique, ajoutez une entrée DNS (CNAME) pour **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, pointant vers **[MktoTrackingLink]**.

`3)` Liste autorisée Marketo.

    * Si nous utilisons des adresses IP dans notre Liste autorisée de courriel, ajoutez les adresses IP répertoriées ci-dessous :
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    9}4.htm

>[!NOTE]
>
>Contactez l’assistance Marketo si vous souhaitez obtenir une liste abrégée d’adresses IP à placer sur la liste autorisée spécifique à votre environnement.

    * Si notre système anti-spam utilise des domaines From, ajoutez ces éléments :

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Nous devons configurer SPF et DKIM afin que Marketo soit autorisé à envoyer des emails signés en notre nom.

`a.` Pour configurer SPF, ajoutez la ligne suivante à nos entrées DNS :

DANS TXT **[From Domain]**: v=spf1 mx ip4:**[Corporate IP(s)]**
<br/>include : mktomail.com ~all

Si nous avons déjà un enregistrement SPF existant dans notre entrée DNS, ajoutez-y simplement les éléments suivants :

include:mktomail.com

`[`Remplacez **From Domain** par votre Email From Domain (ex : company.com) et **CorpIP** par l’adresse IP de votre serveur de messagerie d’entreprise (ex : 255.255.255.255).  Si vous allez envoyer des emails de plusieurs domaines via Marketo, votre personnel informatique doit ajouter cette ligne pour chaque domaine (sur une ligne).`]`

`b.` Pour DKIM, créez des enregistrements de ressources DNS pour chaque domaine que nous souhaitez configurer. Vous trouverez ci-dessous les enregistrements d’hôte et les valeurs TXT pour chaque domaine pour lequel nous allons signer :

**`[DKIMDomain1]`** : l’enregistrement hôte est **`[HostRecord1]`** et la valeur TXT est **[TXTValue1]**.

**`[DKIMDomain2]`** : l’enregistrement hôte est **`[HostRecord2]`** et la valeur TXT est **`[TXTValue2]`**.

`[` Copiez les **HostRecord** et **TXTValue** pour chaque **DKIMDomain** que vous avez configuré après avoir suivi les [instructions ici](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). N’oubliez pas de vérifier chaque domaine dans **Admin > Email > DKIM** après avoir terminé cette étape.`]`

`5)` Nous devons nous assurer qu’il existe un enregistrement MX valide pour nos domaines FROM **[FromDomain1]**, **[FromDomain2]**, etc. Pouvez-vous confirmer ? Si ce n’est pas le cas, configurez pour mapper à notre enregistrement MX de domaine d’entreprise. Cela nous permettra de traiter les réponses/réponses aux messages Marketo.

Faites-moi savoir quand vous avez terminé ces étapes, de sorte que je puisse terminer le processus de configuration avec Marketo.

Merci ! Tu es la meilleure !

L&#39;amour,

**`[Your Name]`**

`----------------------------------------------`

Envoyez l’e-mail au service informatique. Nous comprenons qu’il peut s’écouler un certain temps avant que l’informatique puisse réaliser ces tâches. Vous pouvez passer à l’étape 7, mais n’oubliez pas que vous devez renvoyer l’étape 6 pour terminer la configuration de Marketo.

## Terminer la configuration de Marketo une fois l’informatique terminée {#complete-your-marketo-setup-after-it-finishes}

Une fois les tâches du service informatique terminées, procédez comme suit pour ajouter votre landing page et vos CNAME de messagerie, et activer la signature DKIM.

Accédez à la zone **[!UICONTROL Admin]** pour ajouter votre CNAME de page d’entrée

![](assets/setup-steps-15.png)

Sélectionnez Landing Pages et cliquez sur **[!UICONTROL Modifier]** dans la zone [!UICONTROL Paramètres].

![](assets/setup-steps-16.png)

Saisissez votre nouveau nom de domaine dans le champ **[!UICONTROL Nom de domaine pour les landing pages]**. Cela doit se présenter comme suit :

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

Dans le champ de page **[!UICONTROL Page de secours]** , saisissez l’URL à laquelle vous souhaitez que les visiteurs accèdent en cas d’indisponibilité d’une page d’entrée. Vous pouvez utiliser la page d’accueil de votre société si vous ne disposez pas d’une page de secours. Dans le champ **[!UICONTROL Page d&#39;accueil]**, saisissez le site Web de votre société.

![](assets/setup-steps-18.png)

Dans la zone [!UICONTROL Admin], sélectionnez **[!UICONTROL Email]** pour ajouter votre CNAME de messagerie

![](assets/setup-steps-19.png)

Faites défiler l’écran jusqu’à [!UICONTROL Domaines de marque]. Sélectionnez votre domaine et cliquez sur **[!UICONTROL Modifier]**.

![](assets/setup-steps-20.png)

Dans le champ Domaine , saisissez votre domaine de tracking email. Cela doit se présenter comme suit :

`[EmailTrackingCNAME].[CompanyDomain].com`. Cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/setup-steps-21.png)

## Intégration de votre CRM {#integrate-your-crm}

C’est probablement l’étape la plus passionnante de votre configuration. Il est temps de remplir Marketo avec tous les contacts et prospects que vous avez stockés dans votre CRM !

Choisissez l’un des éléments suivants, en fonction du CRM utilisé par votre entreprise.

    * [Intégrer Marketo avec [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Intégrer Marketo avec [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Pour effectuer ces étapes, vous avez besoin de l’aide de l’administrateur CRM de votre entreprise.

## Ajout du code de suivi à votre site web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Êtes-vous un client [!DNL Launch Pack] ? Vous pouvez ignorer cette étape. Votre consultant vous fournira des instructions de code [!DNL Munchkin] dans votre document d’instructions de configuration informatique.

Marketo dispose d’un JavaScript de suivi personnalisé (appelé [!DNL Munchkin]) que vous pouvez utiliser pour effectuer le suivi des activités de personnes sur n’importe quelle page web. [!DNL Munchkin] est nécessaire pour intégrer votre site web à Marketo. Suivez ces étapes pour [Ajouter [!DNL Munchkin] Code de suivi à votre site Web](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>Expérience avec HTML requise pour ajouter le code de suivi.

## Attentes en termes de performances {#performance-expectations}

À quoi pouvez-vous vous attendre en termes de performances de Marketo ? Il peut varier en fonction de la taille et de la complexité de vos campagnes marketing. Mais vous pouvez vous attendre à des niveaux de performances équivalents à ceux décrits dans la colonne &quot;Standard&quot; dans plusieurs des tables figurant dans la [description du produit Marketo Engage](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. Les colonnes &quot;Performance&quot; et &quot;Performance Plus&quot; se rapportent aux packages de niveau de performance qui fournissent des [ niveaux de performance supérieurs](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

Toutes les étapes de configuration sont terminées. Il ne reste plus qu&#39;à plonger et à utiliser Marketo !
