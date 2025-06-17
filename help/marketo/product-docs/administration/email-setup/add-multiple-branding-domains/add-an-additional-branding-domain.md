---
unique-page-id: 11377395
description: Ajout d’un domaine de marque supplémentaire - Documents Marketo - Documentation du produit
title: Ajout d’un domaine de marque supplémentaire
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: dafac137a6c626794f3b9b2bfaa2fc2de9f2cb75
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 3%

---

# Ajout d’un domaine de marque supplémentaire {#add-an-additional-branding-domain}

Ajoutez un domaine de branding supplémentaire lorsque vous exécutez plusieurs marques à partir d’une seule instance Marketo et souhaitez que chacune d’elles ait ses propres liens de suivi de branding.

>[!PREREQUISITES]
>
>Vous devez [remplacer le lien de suivi générique](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} par un domaine de marque avant d’ajouter d’autres domaines de marque.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Cliquez sur **[!UICONTROL Ajouter]** pour ajouter un domaine de marque supplémentaire.

   ![](assets/add-an-additional-branding-domain-3.png)

1. Saisissez le nom de votre nouveau domaine de marque, sélectionnez _Créer un domaine de Principal_ et/ou _Générer un certificat SSL_ (tous deux facultatifs), puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Définir comme domaine de Principal_ : définissez ce domaine comme votre domaine principal et tous les e-mails non envoyés existants définis sur « Par défaut » ainsi que tous les nouveaux e-mails seront définis par défaut sur le domaine principal. Vous pouvez [remplacer ce paramètre par e-mail](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _Générer un certificat SSL_ : vous pouvez créer un protocole SSL (Secure Sockets Layer) avec la création du domaine. Le premier domaine de suivi lance une configuration unique de l’infrastructure qui peut prendre quelques heures. Vous recevrez une notification à la fin de l’opération, puis vous pourrez configurer le premier domaine. Pour ajouter SSL à vos domaines existants, contactez l’assistance technique de [Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Message d&#39;erreur {#error-messages}

<table><thead>
  <tr>
    <th>Erreur</th>
    <th>Détails</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>Erreur inattendue lors de la création d'un domaine. Contactez l’assistance pour obtenir de l’aide.</i></td>
    <td>Une erreur inattendue s’est produite. Veuillez rassembler les journaux et les détails de l'erreur, puis signaler le problème à l'assistance de <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo</a>.</td>
  </tr>
  <tr>
    <td><i>Le certificat SSL a déjà été émis.</i></td>
    <td>Un certificat SSL existe déjà pour ce domaine personnalisé. Aucune autre action n’est nécessaire, sauf si le certificat a expiré ou doit être réémis.</td>
  </tr>
  <tr>
    <td><i>Le domaine n’est pas mappé au domaine par défaut.</i></td>
    <td>Le domaine personnalisé n’est pas correctement mappé au domaine par défaut. Vérifiez les paramètres de mappage de domaine et assurez-vous que la configuration DNS pointe vers le domaine par défaut correct.</td>
  </tr>
  <tr>
    <td><i>La configuration de Cloudflare a été lancée. Réessayez plus tard.</i></td>
    <td>Lorsque vous créez le premier domaine de suivi pour l’instance, une configuration ponctuelle de l’infrastructure est effectuée dans Cloudfare. Ce message indique que la configuration a été lancée et peut prendre jusqu’à trois heures.</td>
  </tr>
  <tr>
    <td><i>La configuration de Cloudflare est toujours en cours. Réessayez plus tard.</i></td>
    <td>voir ci-dessus</td>
  </tr>
  <tr>
    <td><i>La configuration de Cloudflare a échoué en raison d’une erreur inattendue. Veuillez contacter le service clientèle.</i></td>
    <td>Échec de la configuration initiale de l’infrastructure Cloudfare. Veuillez contacter le support technique de <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo</a> pour obtenir de l'aide.</td>
  </tr>
</tbody></table>

## Éléments à noter {#things-to-note}

* **Mappage DNS du domaine vers Marketo Engage** : avant d’ajouter des domaines dans l’interface utilisateur, vous devez [mapper des CNAME à un domaine fourni par Marketo](https://experienceleague.adobe.com/fr/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSL personnalisés** : si vous avez besoin d’un SSL personnalisé, envoyez un ticket [Support technique](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. N’utilisez pas la case à cocher en libre-service pour la création SSL.

* **SSL préexistants** : lors de l’ajout d’un domaine, le système recherche les SSL préexistants, qui peuvent avoir été créés manuellement au préalable. Si vous rencontrez cette validation, créez votre domaine sans sélectionner la création SSL, et nous les connecterons pour vous. [Contactez l’assistance](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} plus d’informations/d’options.

* **Premier domaine de suivi** : la première création des domaines de liens de suivi des e-mails nécessitera une intervention manuelle de la part de l’assistance [Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. La création ultérieure de sous-domaines sous le même domaine est autorisée dans l’interface utilisateur.

* **Ajout de certificats à des domaines existants** : l’ajout de certificats à des domaines existants n’est pas pris en charge pour le moment. Pour les domaines préexistants ou dans les cas où vous n’avez pas coché la case de certificat SSL, vous devez contacter [l’assistance Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} pour obtenir le certificat ajouté.

* **Modification ou suppression de certificats sur des domaines existants** : si vous devez mettre à jour ou supprimer un protocole SSL existant, contactez l’assistance technique de [Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* **Suppression de domaines** : la suppression d’un domaine ne supprime pas automatiquement le certificat SSL pour le moment. Ce problème sera résolu dans une version ultérieure.

>[!MORELIKETHIS]
>
>[Modifiez Votre Domaine De Branding Par Défaut](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
