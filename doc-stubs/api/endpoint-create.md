---
title: "Create endpoint"
description: "Create a new endpoint object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create endpoint
Namespace: microsoft.graph

Create a new [endpoint](../resources/endpoint.md) object.

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
POST /groups/{groupsId}/endpoints
POST /servicePrincipals/{servicePrincipalsId}/endpoints
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [endpoint](../resources/endpoint.md) object.

The following table shows the properties that are required when you create the [endpoint](../resources/endpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|capability|String|**TODO: Add Description**|
|providerId|String|**TODO: Add Description**|
|providerName|String|**TODO: Add Description**|
|uri|String|**TODO: Add Description**|
|providerResourceId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [endpoint](../resources/endpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_endpoint_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/endpoints
Content-Type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.endpoint",
  "deletedDateTime": "String (timestamp)",
  "capability": "String",
  "providerId": "String",
  "providerName": "String",
  "uri": "String",
  "providerResourceId": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.endpoint",
  "id": "1d9bdbda-dbda-1d9b-dadb-9b1ddadb9b1d",
  "deletedDateTime": "String (timestamp)",
  "capability": "String",
  "providerId": "String",
  "providerName": "String",
  "uri": "String",
  "providerResourceId": "String"
}
```

