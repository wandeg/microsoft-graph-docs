---
title: "Create endpoints"
description: "Create a new endpoints object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create endpoints

Namespace: microsoft.graph

Create a new endpoints object.

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
POST /print/services/{printServiceId}/endpoints
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [printServiceEndpoint](../resources/printserviceendpoint.md) object.

The following table shows the properties that are required when you create the [printServiceEndpoint](../resources/printserviceendpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|uri|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printserviceendpoint_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/services/{printServiceId}/endpoints
Content-Type: application/json
Content-length: 110

{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "displayName": "String",
  "uri": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printserviceendpoint"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "1a4a8a35-8a35-1a4a-358a-4a1a358a4a1a",
  "displayName": "String",
  "uri": "String"
}
```

