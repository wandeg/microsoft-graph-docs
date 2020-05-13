---
title: "List secureScores"
description: "Get the secureScores from the secureScores navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List secureScores

Namespace: microsoft.graph

Get the secureScores from the secureScores navigation property.

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
GET /Security/secureScores
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

If successful, this method returns a `200 OK` response code and a collection of [secureScore](../resources/securescore.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/Security/secureScores
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.securescore)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.secureScore",
      "id": "ed74a1ec-a1ec-ed74-eca1-74edeca174ed",
      "activeUserCount": "Integer",
      "averageComparativeScores": [
        {
          "@odata.type": "microsoft.graph.averageComparativeScore"
        }
      ],
      "azureTenantId": "String",
      "controlScores": [
        {
          "@odata.type": "microsoft.graph.controlScore"
        }
      ],
      "createdDateTime": "String (timestamp)",
      "currentScore": "Double",
      "enabledServices": [
        "String"
      ],
      "licensedUserCount": "Integer",
      "maxScore": "Double",
      "vendorInformation": {
        "@odata.type": "microsoft.graph.securityVendorInformation"
      }
    }
  ]
}
```

