---
title: "Create androidWorkProfileCustomConfiguration"
description: "Create a new androidWorkProfileCustomConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create androidWorkProfileCustomConfiguration

Namespace: microsoft.graph

Create a new [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) object.

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
POST ** Collection URI for microsoft.graph.androidWorkProfileCustomConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) object.

The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|omaSettings|[omaSetting](../resources/omasetting.md) collection|OMA settings. This collection can contain a maximum of 500 elements.|



## Response
If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_androidworkprofilecustomconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.androidWorkProfileCustomConfiguration not found
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidworkprofilecustomconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 496

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "567c17d8-17d8-567c-d817-7c56d8177c56",
  "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
  "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

