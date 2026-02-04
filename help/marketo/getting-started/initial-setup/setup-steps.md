---
description: Étapes de configuration - Documents Marketo - Documentation du produit
short-description: Vous débutez avec Adobe Marketo Engage ? Découvrez les étapes à suivre avant de vous lancer.
title: Étapes de configuration
feature: Getting Started
exl-id: 5f37da48-b2ed-4e48-a5a2-429149745085
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '1687'
ht-degree: 100%

---

# Étapes de configuration {#setup-steps}

**Bienvenue dans Adobe Marketo Engage.**

Avant de vous lancer, vous devez effectuer quelques étapes.

Ces étapes sont les suivantes :

* Application de votre image de marque à vos URL de page de destination et à vos liens d’e-mail pour améliorer la confiance et la délivrabilité
* Configuration de protocoles pour Marketo Engage
* Synchronisation de votre CRM
* Ajout d’un code de suivi au site web de votre entreprise

>[!NOTE]
>
>Vous devez effectuer ces étapes uniquement si votre société **débute avec Marketo**. Si ce n’est pas le cas, la configuration est peut-être déjà effectuée.

Certaines étapes nécessitent l’aide de votre équipe informatique.

## Assurer la délivrabilité des e-mails {#ensure-email-deliverability}

>[!NOTE]
>
>Êtes-vous client ou cliente d’un pack de lancement ? Vous pouvez ignorer cette étape. Votre consultant ou votre consultante vous fournira un document d’instructions de configuration informatique lors de votre appel de lancement.

Vous pouvez prendre plusieurs mesures pour vous assurer que les e-mails atteignent le plus grand nombre possible de personnes.

* **Appliquez votre image de marque à vos liens de suivi**. Vous pouvez choisir un CNAME pour utiliser votre propre domaine (au lieu de celui de Marketo) dans les liens que vous incluez dans les e-mails provenant de Marketo. Cela renforce l’image de marque de votre domaine et accroît la confiance et la délivrabilité pour vos personnes destinataires.
* **Ajoutez Marketo à la liste autorisée de votre messagerie professionnelle**. Il est recommandé d’envoyer des e-mails de test à vos comptes de test avant d’envoyer des e-mails à des personnes réelles. En ajoutant Marketo à votre liste autorisée, vous pouvez empêcher le blocage de ces e-mails de test ou leur désignation en tant que spam.
* **Configurez SPF et DKIM**. Ces technologies garantissent à vos personnes destinataires que vos e-mails Marketo ne sont pas du spam. Pour empêcher les filtres de spam des personnes destinataires de rejeter vos e-mails Marketo, procédez comme suit pour [configurer un SPF et un DKIM pour la délivrabilité de vos e-mails](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Configurez un enregistrement MX pour votre domaine.** Un enregistrement MX vous permet de recevoir des e-mails du domaine depuis lequel vous envoyez des e-mails afin de traiter les réponses et les répondeurs automatiques. Si vous effectuez un envoi à partir de votre domaine d’entreprise, il est probable que ce paramètre soit déjà configuré. Si ce n’est pas le cas, vous pouvez généralement le configurer pour qu’il soit mappé à votre enregistrement MX de domaine d’entreprise.
* **Paramètres recommandés pour l’adresse d’expédition.** Vous devez utiliser un domaine d’e-mail valide, existant et fonctionnel dans l’adresse d’expédition dans toutes les campagnes par e-mail. Il peut s’avérer bénéfique de configurer un sous-domaine de votre domaine d’entreprise plutôt que d’effectuer des envois à partir de votre domaine d’entreprise. Vous aurez ainsi la garantie que les problèmes de votre flux de messagerie d’entreprise n’auront pas d’impact sur votre flux de messagerie Marketo et vice versa. De plus, l’envoi d’e-mails à partir de `something@nonexistentdomain.com` entraîne le filtrage ou le blocage des e-mails. Tout domaine utilisé dans l’adresse d’expédition de l’expéditeur ou de l’expéditrice doit disposer d’un compte postmaster@ et abuse@ valide et fonctionnel.

Si vous utilisez des applications Google pour héberger les e-mails de votre entreprise, vous ne pourrez pas créer d’e-mails abuse@ ou postmaster@ sous votre domaine. Pour contourner ce problème, vous devez créer des groupes nommés « abuse » et « postmaster ». Les utilisateurs et utilisatrices qui sont membres de ces groupes recevront des e-mails envoyés à ces adresses (par exemple, <postmaster@domain.com>). Vous trouverez des instructions détaillées sur la création de groupes [ici](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Choisissez un CNAME pour les liens de suivi des e-mails (choisissez-en un _différent_ à partir du CNAME de la page de destination que vous avez choisi à l’étape 3). Voici quelques exemples :

* go2.[DomaineEntreprise].com
* em.[DomaineEntreprise].com
* wow.[DomaineEntreprise].com

La première partie est le CNAME de suivi de l’e-mail, `[EmailTrackingCNAME]`. Vous devrez le communiquer au service informatique.

>[!CAUTION]
>
>Les CNAME d’e-mail et de page de destination doivent être différents. Évitez également les CNAME tels que « suivi » ou « lien ». Ils sont souvent marqués comme spam.

Pour trouver votre lien de suivi Marketo, accédez à la zone **[!UICONTROL Admin]**.

![](assets/setup-steps-1.png)

Cliquez sur **[!UICONTROL E-mail]**.

![](assets/setup-steps-2.png)

Copiez le [!UICONTROL lien de suivi] à partir de vos paramètres d’e-mail.

Le [!UICONTROL lien de suivi] se présente sous la forme : `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-3.png)

Voici votre `[MktoTrackingLink]`. Enregistrez-le. Vous devrez le communiquer au service informatique à l’étape 5.

Récupérez les domaines « From ». Créez une liste de tous les domaines « From » (par exemple, `[Sender]@[FromDomain].com`) que vous prévoyez d’utiliser pour envoyer des e-mails à partir de Marketo. Pour la plupart, il n’y en a qu’un.

Par exemple, « marketo.com », « info.marketo.com ». Il s’agit de `[FromDomain1]`, `[FromDomain2]`, etc. Enregistrez-les. Vous devrez les communiquer au service informatique à l’étape 5.

Vous disposez maintenant de toutes les informations nécessaires pour envoyer votre demande au service informatique.

## Personnaliser vos URL de page de destination avec un CNAME {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>Êtes-vous client ou cliente d’un pack de lancement ? Vous pouvez ignorer cette étape. Votre consultant ou votre consultante vous fournira un document d’instructions de configuration informatique lors de votre appel de lancement.

>[!NOTE]
>
>**Autorisations d’administration requises**

Choisissez un CNAME pour vos pages de destination. Voici quelques exemples :

    * **go**.[DomaineEntreprise].com
    * **www2**.[DomaineEntreprise].com
    * **lp**.[DomaineEntreprise].com

>[!TIP]
>
>Faites preuve de concision. Les URL plus courtes sont plus faciles à mémoriser. Nous suggérons d’utiliser le domaine « go ».

La première partie (en gras) correspond au `[LandingPageCNAME]`. Vous en aurez besoin à l’étape 5.

Pour récupérer l’identifiant Munchkin que vous allez remplacer par le CNAME de votre page de destination, accédez à la zone **Admin**.

![](assets/setup-steps-4.png)

Cliquez sur **Mon compte**.

![](assets/setup-steps-5.png)

Copiez la [!UICONTROL chaîne de compte] depuis les paramètres de la page de destination.

![](assets/setup-steps-6.png)

Voici l’`[Munchkin ID]`. Enregistrez-le. Vous devrez le communiquer au service informatique à l’étape 5.

Configurez les paramètres de votre domaine afin que les pages de destination utilisent le domaine de votre société au lieu de celui de Marketo (où elles sont hébergées).

## Demander au service informatique de configurer les protocoles {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Êtes-vous client ou cliente d’un pack de lancement ? Vous pouvez ignorer cette étape. Votre consultant ou votre consultante vous fournira un document d’instructions de configuration informatique lors de votre appel de lancement.

Une fois que vous avez rassemblé toutes les informations nécessaires, il est temps d’envoyer une demande au service informatique. Vous pouvez utiliser le texte ci-dessous comme modèle, en remplaçant le texte en gras par vos propres informations.

[Incluez un lien vers cet article](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

Collez ce texte dans l’e-mail et remplacez les espaces réservés en gras :

>[!NOTE]
>
>Reportez-vous aux étapes 3 et 4 ci-dessus pour déterminer le texte à remplacer par les espaces réservés. Souvenez-vous que `[LandingPageCNAME]` et `[EmailTrackingCNAME]` doivent être différents.

`----------------------------------------------`

Chère équipe d’administration informatique,

Notre équipe marketing utilise désormais la plateforme Marketo pour communiquer avec nos équipes. Pour garantir une délivrabilité optimale des e-mails, nous devons effectuer les modifications suivantes :

`1)` Pour nos pages de destination, ajoutez une entrée DNS (CNAME) pour **[CNAMEPageDestination]**.**[DomaineEntreprise]**.com, pointant vers **[Identifiant Munchkin]**.mktoweb.com.

`2)` Pour nos liens de suivi dans les e-mails, ajoutez une entrée DNS (CNAME) pour **[CNAMESuiviE-mail]**.**[DomaineEntreprise]**.com, pointant vers **[LienSuiviMkto]**.

`3)` Ajoutez Marketo à votre liste autorisée.

    * Si nous utilisons des adresses IP dans notre liste autorisée d’e-mails, ajoutez les adresses IP répertoriées ci-dessous :
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    94.236.119.0/26

>[!NOTE]
>
>Contactez l’assistance Marketo si vous souhaitez obtenir une liste abrégée d’adresses IP à placer sur la liste autorisée spécifique à votre environnement.

    * Si notre système anti-spam utilise des domaines De, ajoutez les éléments suivants :

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Nous devons configurer SPF et DKIM pour que Marketo soit autorisé à envoyer des e-mails signés en notre nom.

`a.` Pour configurer SPF, ajoutez la ligne suivante à nos entrées DNS :

IN  TXT **[From Domain]**:  v=spf1 mx ip4:**[Corporate IP(s)]**
<br/>include: mktomail.com ~all

Si nous avons déjà un enregistrement SPF existant dans notre entrée DNS, ajoutez-y simplement ce qui suit :

include:mktomail.com

`[`Remplacez **From Domain** par votre adresse e-mail de domaine (entreprise.com, par exemple) et **CorpIP** par l’adresse IP du serveur de messagerie de votre entreprise (255.255.255.255, par exemple).  Si vous prévoyez d’envoyer des e-mails à partir de plusieurs domaines via Marketo, demandez à votre personnel informatique d’ajouter cette ligne pour chaque domaine (sur une seule ligne).`]`

`b.` Pour DKIM, créez des enregistrements de ressources DNS pour chaque domaine que nous voulons configurer. Vous trouverez ci-dessous les enregistrements d’hôtes et les valeurs TXT pour chaque domaine soumis à une connexion :

**`[DKIMDomain1]`** : l’enregistrement hôte est **`[HostRecord1]`** et la valeur TXT est **`[TXTValue1]`**.

**`[DKIMDomain2]`** : l’enregistrement hôte est **`[HostRecord2]`** et la valeur TXT est **`[TXTValue2]`**.

`[`Copiez les éléments **HostRecord** et **TXTValue** pour chaque **DKIMDomain** que vous avez configuré après avoir suivi les [instructions ici](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). N’oubliez pas de vérifier chaque domaine dans **Admin > E-mail > DKIM** une fois que votre personnel informatique a terminé cette étape.`]`

`5)` Nous devons nous assurer qu’il existe un enregistrement MX valide pour nos domaines FROM **`[FromDomain1]`**, **`[FromDomain2]`**, etc. Pouvez-vous confirmer ? Si ce n’est pas le cas, configurez pour mapper notre enregistrement MX de domaine d’entreprise. Nous pourrons ainsi traiter les réponses/répondeurs automatiques à nos publipostages Marketo.

Prévenez-moi lorsque vous avez terminé ces étapes, afin que je puisse terminer le processus de configuration avec Marketo.

Merci, vous êtes la crème de la crème !

Cordialement,

**`[Your Name]`**

`----------------------------------------------`

Envoyez l’e-mail au service informatique. Nous comprenons que le service informatique puisse prendre un certain temps pour effectuer ces tâches. Vous pouvez passer à l’étape suivante, mais n’oubliez pas que vous devez revenir à cette étape pour terminer votre configuration de Marketo Engage.

## Terminez votre configuration de Marketo une fois que l’équipe informatique aura terminé. {#complete-your-marketo-setup-after-it-finishes}

Une fois que le service informatique a terminé ses tâches, procédez comme suit pour ajouter vos CNAME de page de destination et d’e-mail, ainsi que pour activer la signature DKIM.

Accédez à la zone **[!UICONTROL Admin]** pour ajouter votre CNAME de page de destination.

![](assets/setup-steps-7.png)

Sélectionnez Pages de destination et cliquez sur **[!UICONTROL Modifier]** dans la zone [!UICONTROL Paramètres].

![](assets/setup-steps-8.png)

Saisissez votre nouveau nom de domaine dans le champ **[!UICONTROL Nom de domaine pour les pages de destination]**. Il doit se présenter comme suit :

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-9.png)

Dans le champ Page de **[!UICONTROL secours]**, saisissez l’URL à laquelle les personnes doivent accéder si une page de destination n’est pas disponible. Vous pouvez utiliser la page d’accueil de votre entreprise si vous ne disposez pas d’une page de secours. Dans le champ **[!UICONTROL Page d’accueil]**, saisissez le site web de votre société.

![](assets/setup-steps-10.png)

Dans la zone [!UICONTROL Admin], sélectionnez **[!UICONTROL E-mail]** pour ajouter votre CNAME d’e-mail.

![](assets/setup-steps-11.png)

Faites défiler jusqu’à [!UICONTROL Noms des domaines]. Sélectionnez votre domaine et cliquez sur **[!UICONTROL Modifier]**.

![](assets/setup-steps-12.png)

Dans le champ Domaine, saisissez votre domaine de suivi d’e-mail. Il doit se présenter comme suit :

`[EmailTrackingCNAME].[CompanyDomain].com`. Cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/setup-steps-13.png)

## Intégrer votre CRM {#integrate-your-crm}

Il s’agit probablement de la partie la plus passionnante de votre configuration. Il est temps de remplir Marketo avec tous ces prospects et contacts que vous avez stockés dans votre CRM.

Choisissez l’une des options suivantes, en fonction du CRM utilisé par votre entreprise.

* [Intégrer Marketo Engage à  [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
* [Intégrer Marketo Engage à  [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

  >[!NOTE]
  >
  >Vous avez besoin de l’aide de l’administrateur ou de l’administratrice CRM de votre entreprise pour effectuer ces étapes.

## Ajouter le code de suivi à votre site web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Êtes-vous un client ou une cliente [!DNL Launch Pack] ? Vous pouvez ignorer cette étape. Votre consultant ou consultante vous fournira des instructions de code [!DNL Munchkin] dans votre document d’instructions de configuration informatique.

Marketo Engage dispose d’un JavaScript de suivi personnalisé ([!DNL Munchkin]) que vous pouvez utiliser pour effectuer le suivi des activités des personnes sur n’importe quelle page web. [!DNL Munchkin] est nécessaire pour intégrer votre site web à Marketo. Pour [ajouter le code de suivi  [!DNL Munchkin]  à votre site web](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}, procédez comme suit.

>[!NOTE]
>
>Une certaine expérience avec HTML est requise pour ajouter le code de suivi.

## Attentes en matière de performances {#performance-expectations}

À quoi pouvez-vous vous attendre en matière de performances de la part de Marketo ? Cela peut varier en fonction de la taille et de la complexité de vos campagnes marketing. Mais vous pouvez vous attendre à des niveaux de performances comparables à ceux indiqués dans la colonne « Standard » de plusieurs tableaux figurant dans la description du produit [Marketo Engage](https://helpx.adobe.com/fr/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. Les colonnes « Performance » et « Performance Plus » font référence aux packages de niveau de performances qui fournissent des [niveaux de performances supérieurs](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Configurer les protocoles pour Marketo Engage](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md)
>
>* [Configuration de l’utilisateur ou de l’utilisatrice](/help/marketo/getting-started/initial-setup/user-setup.md)
