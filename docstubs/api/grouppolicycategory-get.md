---
title: "Get groupPolicyCategory"
description: "Read properties and relationships of the groupPolicyCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupPolicyCategory

Namespace: microsoft.graph

Read properties and relationships of the [groupPolicyCategory](../resources/grouppolicycategory.md) object.

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
GET /deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
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
If successful, this method returns a `200 OK` response code and [groupPolicyCategory](../resources/grouppolicycategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicycategory"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyCategory"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyCategory",
    "id": "42a52978-2978-42a5-7829-a5427829a542",
    "displayName": "Display Name value",
    "isRoot": true,
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
  }
}
```

