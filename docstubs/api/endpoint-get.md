---
title: "Get endpoint"
description: "Read properties and relationships of the endpoint object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get endpoint

Namespace: microsoft.graph

Read properties and relationships of the [endpoint](../resources/endpoint.md) object.

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
GET /groups/{groupsId}/endpoints/{endpointId}
GET /me/joinedGroups/{groupId}/endpoints/{endpointId}
GET /servicePrincipals/{servicePrincipalsId}/endpoints/{endpointId}
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
If successful, this method returns a `200 OK` response code and [endpoint](../resources/endpoint.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}
-->
``` http
GET https://graph.microsoft.com/beta/groups/{groupsId}/endpoints/{endpointId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 388

{
  "value": {
    "@odata.type": "#microsoft.graph.endpoint",
    "id": "0db78d66-8d66-0db7-668d-b70d668db70d",
    "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
    "capability": "Capability value",
    "providerId": "Provider Id value",
    "providerName": "Provider Name value",
    "uri": "Uri value",
    "providerResourceId": "Provider Resource Id value"
  }
}
```

