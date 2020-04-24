---
title: "List agreementAcceptances"
description: "Get a list of the agreementAcceptance objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List agreementAcceptances

Namespace: microsoft.graph

Get a list of the [agreementAcceptance](../resources/agreementacceptance.md) objects and their properties.

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
GET /agreementAcceptances
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptance"
}
-->
``` http
GET https://graph.microsoft.com/beta/agreementAcceptances
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.agreementacceptance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.agreementAcceptance",
      "id": "63a0f9ec-f9ec-63a0-ecf9-a063ecf9a063",
      "agreementId": "Agreement Id value",
      "userId": "User Id value",
      "agreementFileId": "Agreement File Id value",
      "recordedDateTime": "2016-12-31T23:56:35.2919298+03:00",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "userEmail": "User Email value",
      "state": "String"
    }
  ]
}
```

