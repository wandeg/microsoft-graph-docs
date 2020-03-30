---
title: "List telecomExpenseManagementPartners"
description: "Get the telecomExpenseManagementPartners from the telecomExpenseManagementPartners navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List telecomExpenseManagementPartners

Namespace: microsoft.graph

Get the telecomExpenseManagementPartners from the telecomExpenseManagementPartners navigation property.

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
GET /deviceManagement/telecomExpenseManagementPartners
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
If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_telecomexpensemanagementpartner"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.telecomexpensemanagementpartner)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "d7e10a84-0a84-d7e1-840a-e1d7840ae1d7",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:57:31.9036997+03:00"
    }
  ]
}
```

