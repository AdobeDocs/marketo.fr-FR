---
unique-page-id: 10093188
description: Présentation des objets personnalisés Marketo - Documents Marketo - Documentation du produit
title: Présentation des objets personnalisés Marketo
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 2%

---

# Présentation des objets personnalisés Marketo {#understanding-marketo-custom-objects}

Utilisez des objets personnalisés pour effectuer le suivi de mesures propres à votre entreprise.

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus d&#39;informations.

Utilisez des objets personnalisés comme filtres et déclencheurs dans vos campagnes dynamiques. Par exemple :

* **Filtrer**: Envoyer des emails uniquement aux propriétaires d’une marque spécifique de véhicule
* **Déclencheur**: Envoyez un courrier électronique lorsqu’un objet personnalisé est ajouté à une personne ou à une entreprise.

Vous pouvez configurer des objets personnalisés dans une relation de type &quot;un à plusieurs&quot; ou &quot;plusieurs à plusieurs&quot;. Par exemple :

* **De un à plusieurs**: Une personne possède plusieurs voitures.
* **De plusieurs à plusieurs**: Plusieurs étudiants sont inscrits à plusieurs cours à partir d’un catalogue de cours

Une structure de type &quot;un à plusieurs&quot; utilise un champ de lien unique pour connecter l’objet personnalisé à une personne ou à une entreprise.

Plusieurs à plusieurs objets personnalisés utilisent deux champs de lien, faisant partie d’un objet intermédiaire. Un champ Lien est connecté à la personne ou à la société et un autre est connecté à l’objet personnalisé, tel que le catalogue de cours. Cet objet intermédiaire peut contenir des champs personnalisés supplémentaires, tels qu’un niveau de cours ou une date de présence, ce qui définit davantage la nature de la connexion.

>[!TIP]
>
>Importez des objets personnalisés à l’aide de valeurs séparées par des virgules (CSV) dans l’interface utilisateur pour tester et valider un exemple de données. Ensuite, téléchargez tous vos fichiers avec une API.

>[!CAUTION]
>
>Vous ne pouvez pas restaurer des objets personnalisés. Veillez donc à ne plus en avoir besoin avant de les supprimer.

## Accès aux objets personnalisés de Marketo {#accessing-marketo-custom-objects}

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/understanding-marketo-custom-objects-1.png)

1. Cliquez sur **[!UICONTROL Objets personnalisés Marketo]**.

   ![](assets/understanding-marketo-custom-objects-2.png)

1. L’affichage Objets personnalisés Marketo répertorie tous vos objets personnalisés à droite, mais uniquement ceux approuvés dans la grille principale.

   ![](assets/understanding-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >La grille affiche le nom de l’objet, le nombre d’enregistrements, le nombre de champs et la date de la mise à jour la plus récente.

   >[!TIP]
   >
   >Marketo met automatiquement à jour ces champs, mais vous pouvez actualiser l’affichage en cliquant sur l’icône dans la colonne Enregistrements .

1. Cliquez sur le nom de l’objet à droite pour ouvrir la page de détails.

   ![](assets/understanding-marketo-custom-objects-4.png)

## Affichage des objets personnalisés associés à une personne {#view-custom-objects-associated-to-a-person}

Après avoir créé la structure d’objet personnalisé, lorsque vous chargez les données d’objet personnalisé spécifiques, les objets personnalisés sont automatiquement associés aux personnes dans la base de données à l’aide du champ de lien de l’objet personnalisé. Vous pouvez afficher des informations à partir du [!UICONTROL Objets personnalisés] sur la page détails de la personne.

1. Accédez à **[!UICONTROL Base]**.

   ![](assets/understanding-marketo-custom-objects-5.png)

1. Ouvrez votre base de données et cliquez sur le bouton **[!UICONTROL Personnes]** . Double-cliquez sur l’enregistrement d’une personne que vous avez associée à un objet personnalisé.

   ![](assets/understanding-marketo-custom-objects-6.png)

1. Sur la page Détails de la personne, cliquez sur le **[!UICONTROL Objets personnalisés]** . Sélectionnez l’objet dans la liste déroulante.

   ![](assets/understanding-marketo-custom-objects-7.png)

1. Vous pouvez désormais afficher la liste de tous les objets personnalisés de ce type qui sont associés à cette personne.

   ![](assets/understanding-marketo-custom-objects-8.png)

## Utilisation d’objets personnalisés avec des entreprises {#using-custom-objects-with-companies}

Un objet personnalisé lié à l’entreprise fonctionne mieux si vous synchronisez les entreprises à partir du CRM ou si vous créez explicitement des entreprises à l’aide de l’API. Nous vous recommandons également d’utiliser l’ID de société comme champ de lien.

Si plusieurs personnes dans Marketo sont des enregistrements dans les enregistrements CRM ou Marketo uniquement, un objet personnalisé lié à une entreprise ne sera pas associé à plusieurs enregistrements individuels. Cela est dû au fait qu’une société comptant plusieurs personnes en-dessous est prise en charge uniquement lorsque les entreprises sont synchronisées à partir du CRM ou si vous utilisez une API pour créer explicitement des entreprises.

Les objets personnalisés ne peuvent être associés directement qu’à un seul enregistrement. Cela signifie que lorsque votre type d’objet personnalisé est lié par champ d’entreprise, vous devez vous assurer que vos enregistrements de personne sont associés à une entreprise à l’aide de la conversion de contact dans votre CRM ou à l’aide du champ externalCompanyId si vous gérez des entreprises à l’aide des API REST Marketo. Pour les enregistrements de personne qui ne sont pas liés explicitement aux enregistrements de l’entreprise, les objets personnalisés liés à l’aide de l’entreprise sont liés de manière aléatoire à un seul enregistrement, même si la valeur du champ de l’entreprise est partagée par de nombreuses personnes.

Voir [Importer des données d’objet personnalisées](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) pour plus d’informations.

>[!MORELIKETHIS]
>
>* [Créer des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [Approbation d’un objet personnalisé](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Modification et suppression d’un objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Ajout de champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Modification et suppression de champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Importer les données de l’objet personnalisé](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)
