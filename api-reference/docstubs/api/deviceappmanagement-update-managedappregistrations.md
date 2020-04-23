---
title: "Update managedAppRegistrations"
description: "Update the properties of a managedAppRegistrations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update managedAppRegistrations

Namespace: microsoft.graph

Update the properties of a managedAppRegistrations object.

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
PATCH /deviceAppManagement/managedAppRegistrations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [managedAppRegistration](../resources/managedappregistration.md) object.

The following table shows the properties that are required when you create the [managedAppRegistration](../resources/managedappregistration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|Date and time of creation|
|lastSyncDateTime|DateTimeOffset|Date and time of last the app synced with management service.|
|applicationVersion|String|App version|
|managementSdkVersion|String|App management SDK version|
|platformVersion|String|Operating System version|
|deviceType|String|Host device type|
|deviceTag|String|App management SDK generated tag, which helps relate apps hosted on the same device. Not guaranteed to relate apps in all conditions.|
|deviceName|String|Host device name|
|flaggedReasons|managedAppFlaggedReason collection|Zero or more reasons an app registration is flagged. E.g. app running on rooted device. Possible values are: `none`, `rootedDevice`.|
|userId|String|The user Id to who this app registration belongs.|
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|The app package Identifier|
|version|String|Version of the entity.|



## Response
If successful, this method returns a `200 OK` response code and an updated [managedAppRegistration](../resources/managedappregistration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_managedappregistrations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-Type: application/json
Content-length: 587

{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:03:21.3080262+03:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "String"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
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
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "id": "5b188225-8225-5b18-2582-185b2582185b",
  "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
  "lastSyncDateTime": "2017-01-01T00:03:21.3080262+03:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "String"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

