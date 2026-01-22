---
description: Demandes d’accès à des informations personnelles - Documents Marketo - Documentation du produit
title: Demandes d’accès à des informations personnelles
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 0105c6480f75f8daf3db61cd400a4956698839d9
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 16%

---

# Demandes d’accès à des informations personnelles {#privacy-requests}

Ce document offre une vue d’ensemble de la gestion des demandes individuelles de confidentialité des données que vous pouvez envoyer à Marketo Engage par le biais de l’interface utilisateur de Privacy Service et de l’API Privacy Service.

>[!NOTE]
>
>Les demandes d’accès à des informations personnelles envoyées via l’interface utilisateur ou l’API Privacy Service pour Marketo Engage s’appliquent uniquement aux éléments suivants :
>
>* Utilisateurs de Marketo Engage ayant intégré le système Adobe Identity Management
>
>**-ou-**
>
>* les utilisateurs de Marketo Engage qui utilisent un autre produit Experience Cloud déjà présent dans le système Adobe Identity Management (par exemple, les éditions RT-CDP, B2B et B2P, Audience Manager).

Vous pouvez envoyer des requêtes individuelles pour accéder aux données des clients et les supprimer de Marketo Engage de deux manières :

* Via l’interface utilisateur de Privacy Service : `https://experience.adobe.com/#/@YOURCOMPANYNAME/privacy`. Consultez la documentation [ici](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=fr){target="_blank"}.
* Via l’API Privacy Service. Consultez la documentation [ici](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"} et les informations sur l’API [ici](https://developer.adobe.com/experience-platform-apis/){target="_blank"}.

[Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=fr){target="_blank"} prend en charge deux types de demandes : l&#39;accès aux données et la suppression des données.

Voyons comment créer des demandes d’accès et de suppression.

## Configuration requise pour envoyer des demandes pour Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Pour envoyer des demandes d’accès et de suppression de données pour Marketo Engage, vous devez :

1. Identifier les éléments suivants :

   a. ID d’organisation IMS<br/>
b. Adresse e-mail de la personne sur laquelle vous souhaitez agir

   Un identifiant de l’organisation IMS est une chaîne alphanumérique de 24 caractères à laquelle est ajouté @AdobeOrg. Si votre équipe marketing ou votre administrateur système interne Adobe ne connaît pas l’ID d’organisation IMS de votre organisation, contactez l’assistance clientèle d’Adobe à l’adresse `gdprsupport@adobe.com`. Vous avez besoin de l’identifiant d’organisation IMS pour envoyer des requêtes à l’API Privacy.

1. Dans Privacy Service, vous pouvez envoyer des demandes d’accès et de suppression à Marketo Engage et vérifier le statut des demandes existantes.

## Valeurs de champ obligatoires dans les requêtes JSON Marketo Engage {#required-field-values-in-marketo-engage-json-requests}

« companyContexts » :

* « namespace » : **imsOrgID**
* « value » : `<Your IMS Org ID Value>`

&quot;users&quot; :

* &quot;action&quot; : **accès** « access » ou **suppression** « delete »
* « userIDs » :
   * « namespace » : **Email**
   * « type » : **standard**
   * « value » : `<Data Subject's Email Address>`

« include » :

* **marketo** (qui est le produit Adobe qui s’applique à la requête)

« règlement » :

* **rgpd**, **ccpa**, **pdpa**, **lgpd_bra** ou **nzpa_nzl** (qui est le règlement sur la confidentialité qui s’applique à la demande)

## Exemple 1 : demande de suppression en vertu du RGPD {#gdpr-delete-request}

Requête JSON

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "Email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

Réponse JSON

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "Email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## Exemple 2 : demande d’accès au CCPA {#ccpa-access-request}

Requête JSON

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "Email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

Réponse JSON

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "Email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

>[!MORELIKETHIS]
>
>[Gestion de la confidentialité](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
