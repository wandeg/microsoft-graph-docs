---
title: "Create enrollmentTroubleshootingEvent"
description: "Create a new enrollmentTroubleshootingEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create enrollmentTroubleshootingEvent

Namespace: microsoft.graph

Create a new [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.

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
POST ** Collection URI for microsoft.graph.enrollmentTroubleshootingEvent not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.

The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|eventDateTime|DateTimeOffset|Time when the event occurred . Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|correlationId|String|Id used for tracing the failure in the service. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|managedDeviceIdentifier|String|Device identifier created or collected by Intune.|
|operatingSystem|String|Operating System.|
|osVersion|String|OS Version.|
|userId|String|Identifier for the user that tried to enroll the device.|
|deviceId|String|Azure AD device identifier.|
|enrollmentType|Enumeration|Type of the enrollment. Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|failureCategory|Enumeration|Highlevel failure category. Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.|
|failureReason|String|Detailed failure reason.|



## Response
If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_enrollmenttroubleshootingevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.enrollmentTroubleshootingEvent not found
Content-type: application/json
Content-length: 493

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2017-01-01T00:02:42.1849461+03:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "Failure Reason value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.enrollmenttroubleshootingevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 542

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "446f3087-3087-446f-8730-6f4487306f44",
  "eventDateTime": "2017-01-01T00:02:42.1849461+03:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "Failure Reason value"
}
```

