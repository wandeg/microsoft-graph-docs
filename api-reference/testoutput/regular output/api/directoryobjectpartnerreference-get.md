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

## HTTP Request
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

## Example

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
    "id": "0850d6c0-d6c0-0850-c0d6-5008c0d65008",
    "deletedDateTime": "2017-01-01T00:02:06.0464622+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "externalPartnerTenantId": "2064428a-428a-2064-8a42-64208a426420",
    "objectType": "Object Type value"
  }
}
```

