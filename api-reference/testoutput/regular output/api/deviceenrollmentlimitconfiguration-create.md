---
title: "Create deviceEnrollmentLimitConfiguration"
description: "Create a new deviceEnrollmentLimitConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create deviceEnrollmentLimitConfiguration

Create a new [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) object.

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
POST ** Collection URI for microsoft.graph.deviceEnrollmentLimitConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.

The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|description|String| Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|priority|Int32| Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|createdDateTime|DateTimeOffset| Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|version|Int32| Inherited from [deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|
|limit|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/deviceenrollmentlimitconfiguration.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceenrollmentlimitconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.deviceEnrollmentLimitConfiguration not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceenrollmentlimitconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "3ab8cc48-cc48-3ab8-48cc-b83a48ccb83a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2016-12-31T23:57:22.3554145+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:09.8413999+03:00",
  "version": 7,
  "limit": 5
}
```

