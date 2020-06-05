---
title: "Create policyBase"
description: "Create a new policyBase object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create policyBase
Namespace: microsoft.graph

Create a new [policyBase](../resources/policybase.md) object.

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
POST ** Collection URI for microsoft.graph.policyBase not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [policyBase](../resources/policybase.md) object.

The following table shows the properties that are required when you create the [policyBase](../resources/policybase.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [policyBase](../resources/policybase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_policybase_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.policyBase not found
Content-Type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.policyBase",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.policybase"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.policyBase",
  "id": "4a310157-0157-4a31-5701-314a5701314a",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```

