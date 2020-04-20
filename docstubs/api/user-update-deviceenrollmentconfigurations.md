---
title: "Update deviceEnrollmentConfigurations"
description: "Update the properties of a deviceEnrollmentConfigurations object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceEnrollmentConfigurations

Namespace: microsoft.graph

Update the properties of a deviceEnrollmentConfigurations object.

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
PATCH /me/deviceEnrollmentConfigurations
PATCH /users/{usersId}/deviceEnrollmentConfigurations
PATCH /invitations/{invitationsId}/invitedUser/deviceEnrollmentConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object.

The following table shows the properties that are required when you create the [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The display name of the device enrollment configuration|
|description|String|The description of the device enrollment configuration|
|priority|Int32|Priority is used when a user exists in multiple groups that are assigned enrollment configuration. Users are subject only to the configuration with the lowest priority value.|
|createdDateTime|DateTimeOffset|Created date time in UTC of the device enrollment configuration|
|lastModifiedDateTime|DateTimeOffset|Last modified date time in UTC of the device enrollment configuration|
|version|Int32|The version of the device enrollment configuration|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deviceenrollmentconfigurations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/deviceEnrollmentConfigurations
Content-Type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "897585fc-85fc-8975-fc85-7589fc857589",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2016-12-31T23:57:02.5240758+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:44.3371159+03:00",
  "version": 7
}
```

