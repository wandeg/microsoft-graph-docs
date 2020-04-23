---
title: "Update deviceConfigurations"
description: "Update the properties of a deviceConfigurations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceConfigurations

Namespace: microsoft.graph

Update the properties of a deviceConfigurations object.

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
PATCH /deviceManagement/deviceConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceConfiguration](../resources/deviceconfiguration.md) object.

The following table shows the properties that are required when you create the [deviceConfiguration](../resources/deviceconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|displayName|String|Admin provided name of the device configuration.|
|version|Int32|Version of the device configuration.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceConfiguration](../resources/deviceconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deviceconfigurations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-Type: application/json
Content-length: 157

{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
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
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "7a06d112-d112-7a06-12d1-067a12d1067a",
  "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
  "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

