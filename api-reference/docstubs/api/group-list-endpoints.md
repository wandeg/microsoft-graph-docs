---
title: "List endpoints"
description: "Get the endpoints from the endpoints navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List endpoints

Namespace: microsoft.graph

Get the endpoints from the endpoints navigation property.

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
GET /groups/{groupsId}/endpoints
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
If successful, this method returns a `200 OK` response code and a collection of [endpoint](../resources/endpoint.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}
-->
``` http
GET https://graph.microsoft.com/beta/groups/{groupsId}/endpoints
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.endpoint)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.endpoint",
      "id": "32e62bbf-2bbf-32e6-bf2b-e632bf2be632",
      "deletedDateTime": "2016-12-31T23:58:36.0226893+03:00",
      "capability": "Capability value",
      "providerId": "Provider Id value",
      "providerName": "Provider Name value",
      "uri": "Uri value",
      "providerResourceId": "Provider Resource Id value"
    }
  ]
}
```

