---
title: "Update deviceEnrollmentLimitConfiguration"
description: "Update the properties of a deviceEnrollmentLimitConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceEnrollmentLimitConfiguration

Namespace: microsoft.graph

Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) object.

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
PATCH ** Entity URI for microsoft.graph.deviceEnrollmentLimitConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) object.

The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|description|String| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|priority|Int32| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|version|Int32| Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|
|limit|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_deviceenrollmentlimitconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.deviceEnrollmentLimitConfiguration not found
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
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
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "cc2bc06b-c06b-cc2b-6bc0-2bcc6bc02bcc",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:01:25.3917672+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:55.6908839+03:00",
  "version": 7,
  "limit": 5
}
```

