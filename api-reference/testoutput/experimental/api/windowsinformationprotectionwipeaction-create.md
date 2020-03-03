---
title: "Create windowsInformationProtectionWipeAction"
description: "Create a new windowsInformationProtectionWipeAction object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create windowsInformationProtectionWipeAction

Namespace: microsoft.graph

Create a new [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.

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
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|Wipe action status. Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|targetedUserId|String|The UserId being targeted by this wipe action.|
|targetedDeviceRegistrationId|String|The DeviceRegistrationId being targeted by this wipe action.|
|targetedDeviceName|String|Targeted device name.|
|targetedDeviceMacAddress|String|Targeted device Mac address.|
|lastCheckInDateTime|DateTimeOffset|Last checkin time of the device that was targeted by this wipe action.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsinformationprotectionwipeaction_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/windowsInformationProtectionWipeActions
Content-type: application/json
Content-length: 412

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "String",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:58:23.4652469+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsinformationprotectionwipeaction"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 461

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "925020d3-20d3-9250-d320-5092d3205092",
  "status": "String",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:58:23.4652469+03:00"
}
```

