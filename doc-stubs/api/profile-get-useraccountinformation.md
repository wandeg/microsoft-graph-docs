---
title: "Get account"
description: "Read the properties and relationships of a userAccountInformation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get account

Namespace: microsoft.graph

Read the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.

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
GET /user/{userId}/profile/account
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

If successful, this method returns a `200 OK` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/user/{userId}/profile/account
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.userAccountInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.userAccountInformation",
    "id": "9eef3022-3022-9eef-2230-ef9e2230ef9e",
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
    "ageGroup": "String",
    "countryCode": "String",
    "preferredLanguageTag": {
      "@odata.type": "microsoft.graph.localeInfo"
    },
    "userPrincipalName": "String"
  }
}
```

