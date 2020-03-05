---
title: "Update editionUpgradeConfiguration"
description: "Update the properties of a editionUpgradeConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update editionUpgradeConfiguration

Namespace: microsoft.graph

Update the properties of a [editionUpgradeConfiguration](../resources/editionupgradeconfiguration.md) object.

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
PATCH ** Entity URI for microsoft.graph.editionUpgradeConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/editionupgradeconfiguration.md) object.

The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/editionupgradeconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|licenseType|Enumeration|Edition Upgrade License Type. Possible values are: `productKey`, `licenseFile`.|
|targetEdition|Enumeration|Edition Upgrade Target Edition. Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.|
|license|String|Edition Upgrade License File Content.|
|productKey|String|Edition Upgrade Product Key.|



## Response
If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/editionupgradeconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_editionupgradeconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.editionUpgradeConfiguration not found
Content-type: application/json
Content-length: 292

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "String",
  "targetEdition": "String",
  "license": "License value",
  "productKey": "Product Key value"
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
Content-Length: 462

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "0b860b22-0b22-0b86-220b-860b220b860b",
  "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
  "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "String",
  "targetEdition": "String",
  "license": "License value",
  "productKey": "Product Key value"
}
```

