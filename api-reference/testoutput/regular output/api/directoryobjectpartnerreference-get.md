---
title: "Get directoryObjectPartnerReference"
description: "Read properties and relationships of the directoryObjectPartnerReference object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get directoryObjectPartnerReference

Namespace: microsoft.graph

Read properties and relationships of the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.

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
GET ** Entity URI for microsoft.graph.directoryObjectPartnerReference not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryobjectpartnerreference"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.directoryObjectPartnerReference not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": {
    "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
    "id": "42c43b87-3b87-42c4-873b-c442873bc442",
    "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "externalPartnerTenantId": "189e00e4-00e4-189e-e400-9e18e4009e18",
    "objectType": "Object Type value"
  }
}
```

