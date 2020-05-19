---
title: "List people"
description: "Get the people from the people navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List people

Namespace: microsoft.graph

Get the people from the people navigation property.

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
GET /me/people
GET /users/{usersId}/people
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

If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_person"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/people
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.person)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.person",
      "id": "84a6069c-069c-84a6-9c06-a6849c06a684",
      "displayName": "String",
      "givenName": "String",
      "surname": "String",
      "birthday": "String",
      "personNotes": "String",
      "isFavorite": "Boolean",
      "scoredEmailAddresses": [
        {
          "@odata.type": "microsoft.graph.scoredEmailAddress"
        }
      ],
      "phones": [
        {
          "@odata.type": "microsoft.graph.phone"
        }
      ],
      "postalAddresses": [
        {
          "@odata.type": "microsoft.graph.location"
        }
      ],
      "websites": [
        {
          "@odata.type": "microsoft.graph.website"
        }
      ],
      "jobTitle": "String",
      "companyName": "String",
      "yomiCompany": "String",
      "department": "String",
      "officeLocation": "String",
      "profession": "String",
      "personType": {
        "@odata.type": "microsoft.graph.personType"
      },
      "userPrincipalName": "String",
      "imAddress": "String"
    }
  ]
}
```

