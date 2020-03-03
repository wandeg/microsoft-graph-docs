---
title: "Update office365ActivationCounts"
description: "Update the properties of a office365ActivationCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update office365ActivationCounts

Namespace: microsoft.graph

Update the properties of a [office365ActivationCounts](../resources/office365activationcounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.office365ActivationCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [office365ActivationCounts](../resources/office365activationcounts.md) object.

The following table shows the properties that are required when you create the [office365ActivationCounts](../resources/office365activationcounts.md).

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
If successful, this method returns a `200 OK` response code and an updated [office365ActivationCounts](../resources/office365activationcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_office365activationcounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.office365ActivationCounts not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "@odata.type": "#microsoft.graph.office365ActivationCounts",
  "id": "fe8928b4-28b4-fe89-b428-89feb42889fe",
  "reportRefreshDate": "Date",
  "productType": "Product Type value",
  "windows": 7,
  "mac": 3,
  "android": 7,
  "ios": 3,
  "windows10Mobile": 15
}
```

