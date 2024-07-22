---
description: Demandes d’accès à des informations personnelles - Documents Marketo - Documentation du produit
title: Requêtes de confidentialité
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Requêtes de confidentialité {#privacy-requests}

Ce document présente la gestion des demandes de confidentialité des données individuelles que vous pouvez envoyer à Marketo Engage par le biais de l’interface utilisateur du Privacy Service et de l’API du Privacy Service.

>[!NOTE]
>
>Les demandes d’accès à des informations personnelles envoyées par le biais de l’interface utilisateur ou de l’API du Privacy Service pour Marketo Engage s’appliquent uniquement aux éléments suivants :
>
>* Utilisateurs Marketo Engage intégrés à Adobe Identity Management System
>
>**-ou-**
>
>* Utilisateurs Marketo Engage utilisant un autre produit Experience Cloud qui se trouve déjà sur le système Identity Management Adobe (par exemple, RT-CDP, éditions B2B et B2P, Audience Manager).

Vous pouvez envoyer des requêtes individuelles pour accéder aux données des consommateurs et les supprimer du Marketo Engage de deux manières :

* Par le biais de l’ [interface utilisateur de Privacy Service](https://privacyui.cloud.adobe.io/). Consultez la documentation [ici](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=fr){target="_blank"}.
* Par le biais de l’API du Privacy Service. Consultez la documentation [ici](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"} et les informations sur l&#39;API [ici](https://developer.adobe.com/experience-platform-apis/){target="_blank"}.

Le [Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html){target="_blank"} prend en charge deux types de requêtes : l’accès aux données et la suppression des données.

Découvrez comment créer des demandes d’accès et de suppression.

## Configuration requise pour envoyer des requêtes de Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Pour envoyer des demandes d’accès et de suppression de données à Marketo Engage, vous devez :

1. Identifiez les éléments suivants :

   a. Identifiant de l’organisation IMS<br/>
b. Adresse électronique de la personne sur laquelle vous souhaitez agir

   Un identifiant de l’organisation IMS est une chaîne alphanumérique de 24 caractères annexée avec @AdobeOrg. Si votre équipe marketing ou votre administrateur système d’Adobes interne ne connaît pas l’identifiant de l’organisation IMS de votre entreprise, contactez l’assistance clientèle Adobe à l’adresse `gdprsupport@adobe.com`. Vous avez besoin de l’identifiant de l’organisation IMS pour envoyer des requêtes à l’API de confidentialité.

1. Dans Privacy Service, vous pouvez envoyer des demandes d’accès et de suppression à Marketo Engage et vérifier le statut des demandes existantes.

## Valeurs de champ requises dans les requêtes JSON Marketo Engage {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot; : **imsOrgID**
* &quot;value&quot;: `<Your IMS Org ID Value>`

&quot;users&quot; :

* &quot;action&quot; : **access** ou **delete**
* &quot;userIDs&quot; :
   * &quot;namespace&quot; : **email**
   * &quot;type&quot;: **standard**
   * &quot;value&quot;: `<Data Subject's Email Address>`

&quot;include&quot; :

* **marketo** (qui est le produit Adobe qui s’applique à la demande)

&quot;regulation&quot; :

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra** ou **nzpa_nzl** (qui est la réglementation sur la confidentialité qui s’applique à la demande)

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
          "namespace": "email",
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
              "namespace": "email",
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
          "namespace": "email",
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
              "namespace": "email",
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
