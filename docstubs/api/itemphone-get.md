---
title: "Get itemPhone"
description: "Read properties and relationships of the itemPhone object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get itemPhone

Namespace: microsoft.graph

Read properties and relationships of the [itemPhone](../resources/itemphone.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/phones/{itemPhoneId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [itemPhone](../resources/itemphone.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_itemphone"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/phones/{itemPhoneId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1020

{
  "value": {
    "@odata.type": "#microsoft.graph.itemPhone",
    "id": "6e81f6ce-f6ce-6e81-cef6-816ecef6816e",
    "allowedAudiences": "String",
    "inference": {
      "@odata.type": "microsoft.graph.inferenceData",
      "confidenceScore": "Double",
      "userHasVerifiedAccuracy": true
    },
    "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "displayName": "Display Name value",
    "type": "String",
    "number": "Number value"
  }
}
```

