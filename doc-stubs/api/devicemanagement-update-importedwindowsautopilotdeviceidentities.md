---
title: "Update importedWindowsAutopilotDeviceIdentities"
description: "Update the properties of an importedWindowsAutopilotDeviceIdentities object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update importedWindowsAutopilotDeviceIdentities

Namespace: microsoft.graph

Update the properties of an importedWindowsAutopilotDeviceIdentities object.

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
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) object.

The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|orderIdentifier|String|**TODO: Add Description**|
|groupTag|String|**TODO: Add Description**|
|serialNumber|String|**TODO: Add Description**|
|productKey|String|**TODO: Add Description**|
|importId|String|**TODO: Add Description**|
|hardwareIdentifier|Binary|**TODO: Add Description**|
|state|[importedWindowsAutopilotDeviceIdentityState](../resources/importedwindowsautopilotdeviceidentitystate.md)|**TODO: Add Description**|
|assignedUserPrincipalName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_importedwindowsautopilotdeviceidentities"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-Type: application/json
Content-length: 397

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "String",
  "groupTag": "String",
  "serialNumber": "String",
  "productKey": "String",
  "importId": "String",
  "hardwareIdentifier": "Binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
  },
  "assignedUserPrincipalName": "String"
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
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "50bf005f-005f-50bf-5f00-bf505f00bf50",
  "orderIdentifier": "String",
  "groupTag": "String",
  "serialNumber": "String",
  "productKey": "String",
  "importId": "String",
  "hardwareIdentifier": "Binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
  },
  "assignedUserPrincipalName": "String"
}
```

