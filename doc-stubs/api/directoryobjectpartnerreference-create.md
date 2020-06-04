---
title: "Create directoryObjectPartnerReference"
description: "Create a new directoryObjectPartnerReference object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create directoryObjectPartnerReference
Namespace: microsoft.graph

Create a new [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.

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
POST ** Collection URI for microsoft.graph.directoryObjectPartnerReference not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.

The following table shows the properties that are required when you create the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|externalPartnerTenantId|Guid|**TODO: Add Description**|
|objectType|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directoryobjectpartnerreference_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.directoryObjectPartnerReference not found
Content-Type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalPartnerTenantId": "Guid",
  "objectType": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobjectpartnerreference"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "id": "f64feeb5-eeb5-f64f-b5ee-4ff6b5ee4ff6",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalPartnerTenantId": "Guid",
  "objectType": "String"
}
```

