---
title: "List embeddedSIMActivationCodePools"
description: "Get the embeddedSIMActivationCodePools from the embeddedSIMActivationCodePools navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List embeddedSIMActivationCodePools

Namespace: microsoft.graph

Get the embeddedSIMActivationCodePools from the embeddedSIMActivationCodePools navigation property.

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
GET /deviceManagement/embeddedSIMActivationCodePools
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

If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_embeddedsimactivationcodepool"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.embeddedsimactivationcodepool)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
      "id": "9e9ed176-d176-9e9e-76d1-9e9e76d19e9e",
      "displayName": "String",
      "createdDateTime": "String (timestamp)",
      "modifiedDateTime": "String (timestamp)",
      "activationCodes": [
        {
          "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
        }
      ],
      "activationCodeCount": "Integer"
    }
  ]
}
```

