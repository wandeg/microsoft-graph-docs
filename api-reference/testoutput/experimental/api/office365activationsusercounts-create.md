---
title: "Create office365ActivationsUserCounts"
description: "Create a new office365ActivationsUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create office365ActivationsUserCounts

Namespace: microsoft.graph

Create a new [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.office365ActivationsUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object.

The following table shows the properties that are required when you create the [office365ActivationsUserCounts](../resources/office365activationsusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|productType|String||
|assigned|Int64||
|activated|Int64||
|sharedComputerActivation|Int64||



## Response
If successful, this method returns a `201 Created` response code and a [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_office365activationsusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.office365ActivationsUserCounts not found
Content-type: application/json
Content-length: 215

{
  "@odata.type": "#microsoft.graph.office365ActivationsUserCounts",
  "reportRefreshDate": "Date",
  "productType": "Product Type value",
  "assigned": 8,
  "activated": 9,
  "sharedComputerActivation": 8
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365activationsusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.office365ActivationsUserCounts",
  "id": "ef8be27a-e27a-ef8b-7ae2-8bef7ae28bef",
  "reportRefreshDate": "Date",
  "productType": "Product Type value",
  "assigned": 8,
  "activated": 9,
  "sharedComputerActivation": 8
}
```

