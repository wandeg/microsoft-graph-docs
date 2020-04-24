---
title: "Update endpoints"
description: "Update the properties of an endpoints object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update endpoints

Namespace: microsoft.graph

Update the properties of an endpoints object.

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
PATCH /print/services/{printServiceId}/endpoints
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [printServiceEndpoint](../resources/printserviceendpoint.md) object.

The following table shows the properties that are required when you create the [printServiceEndpoint](../resources/printserviceendpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|uri|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_endpoints"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/services/{printServiceId}/endpoints
Content-Type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "displayName": "Display Name value",
  "uri": "Uri value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "da8b6a35-6a35-da8b-356a-8bda356a8bda",
  "displayName": "Display Name value",
  "uri": "Uri value"
}
```

