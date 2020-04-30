---
title: "List agreementAcceptances"
description: "Get the agreementAcceptances from the agreementAcceptances navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List agreementAcceptances

Namespace: microsoft.graph

Get the agreementAcceptances from the agreementAcceptances navigation property.

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
GET ** Collection URI for microsoft.graph.agreementAcceptance not found
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
If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptance"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.agreementAcceptance not found
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
      "id": "221346aa-46aa-2213-aa46-1322aa461322",
      "agreementId": "String",
      "userId": "String",
      "agreementFileId": "String",
      "recordedDateTime": "String (timestamp)",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userEmail": "String",
      "state": "String"
    }
  ]
}
```

