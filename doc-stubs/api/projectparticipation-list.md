---
title: "List projectParticipations"
description: "Get a list of the projectParticipation objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List projectParticipations

Namespace: microsoft.graph

Get a list of the [projectParticipation](../resources/projectparticipation.md) objects and their properties.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/projects
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [projectParticipation](../resources/projectparticipation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_projectparticipation"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/projects
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.projectparticipation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.projectParticipation",
      "id": "5cbcb1f6-b1f6-5cbc-f6b1-bc5cf6b1bc5c",
      "allowedAudiences": "String",
      "inference": {
        "@odata.type": "microsoft.graph.inferenceData"
      },
      "createdDateTime": "String (timestamp)",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "source": {
        "@odata.type": "microsoft.graph.personDataSource"
      },
      "categories": [
        "String"
      ],
      "client": {
        "@odata.type": "microsoft.graph.companyDetail"
      },
      "displayName": "String",
      "detail": {
        "@odata.type": "microsoft.graph.positionDetail"
      },
      "colleagues": [
        {
          "@odata.type": "microsoft.graph.relatedPerson"
        }
      ],
      "sponsors": [
        {
          "@odata.type": "microsoft.graph.relatedPerson"
        }
      ],
      "collaborationTags": [
        "String"
      ]
    }
  ]
}
```

