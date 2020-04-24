---
title: "Create administrativeUnit"
description: "Create a new administrativeUnit object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create administrativeUnit

Namespace: microsoft.graph

Create a new [administrativeUnit](../resources/administrativeunit.md) object.

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
POST /administrativeUnits
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [administrativeUnit](../resources/administrativeunit.md) object.

The following table shows the properties that are required when you create the [administrativeUnit](../resources/administrativeunit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|visibility|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}
-->
``` http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-Type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "visibility": "Visibility value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "64381005-1005-6438-0510-386405103864",
  "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "visibility": "Visibility value"
}
```

