---
title: "Create office365ActivationCounts"
description: "Create a new office365ActivationCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create office365ActivationCounts

Create a new [office365ActivationCounts](../resources/office365activationcounts.md) object.

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
POST ** Collection URI for microsoft.graph.office365ActivationCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the office365ActivationCounts object.

The following table shows the properties that are required when you create the office365ActivationCounts.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|productType|String||
|windows|Int64||
|mac|Int64||
|android|Int64||
|ios|Int64||
|windows10Mobile|Int64||



## Response
If successful, this method returns a `201 Created` response code and a [office365ActivationCounts](../resources/office365activationcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_office365activationcounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.office365ActivationCounts not found
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.office365ActivationCounts",
  "reportRefreshDate": "Date",
  "productType": "Product Type value",
  "windows": 7,
  "mac": 3,
  "android": 7,
  "ios": 3,
  "windows10Mobile": 15
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365activationcounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 274

{
  "@odata.type": "#microsoft.graph.office365ActivationCounts",
  "id": "fb5316b0-16b0-fb53-b016-53fbb01653fb",
  "reportRefreshDate": "Date",
  "productType": "Product Type value",
  "windows": 7,
  "mac": 3,
  "android": 7,
  "ios": 3,
  "windows10Mobile": 15
}
```

