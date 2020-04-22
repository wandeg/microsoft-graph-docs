---
title: "Get ediscoveryCase"
description: "Read properties and relationships of an ediscoveryCase object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get ediscoveryCase

Namespace: microsoft.graph

Read properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.

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
GET /cases/{casesId}
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
If successful, this method returns a `200 OK` response code and an [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_ediscoverycase"
}
-->
``` http
GET https://graph.microsoft.com/beta/cases/{casesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.ediscoveryCase",
    "id": "cb7ba1f3-a1f3-cb7b-f3a1-7bcbf3a17bcb",
    "description": "Description value",
    "createdBy": "Created By value",
    "lastModifiedBy": "Last Modified By value",
    "lastModifiedDateTime": "2016-12-31T23:58:12.0125666+00:00",
    "status": "String",
    "closedBy": "Closed By value",
    "closedDateTime": "2016-12-31T23:59:21.4265692+00:00",
    "externalId": "External Id value",
    "displayName": "Display Name value",
    "createdDateTime": "2017-01-01T00:02:14.13292+00:00"
  }
}
```

