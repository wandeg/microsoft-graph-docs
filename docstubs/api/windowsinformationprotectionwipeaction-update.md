---
title: "Update windowsInformationProtectionWipeAction"
description: "Update the properties of a windowsInformationProtectionWipeAction object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsInformationProtectionWipeAction

Namespace: microsoft.graph

Update the properties of a [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|targetedUserId|String||
|targetedDeviceRegistrationId|String||
|targetedDeviceName|String||
|targetedDeviceMacAddress|String||
|lastCheckInDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsinformationprotectionwipeaction"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 412

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "String",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2017-01-01T00:00:25.9723659+03:00"
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
Content-Length: 461

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "73a354bb-54bb-73a3-bb54-a373bb54a373",
  "status": "String",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2017-01-01T00:00:25.9723659+03:00"
}
```

