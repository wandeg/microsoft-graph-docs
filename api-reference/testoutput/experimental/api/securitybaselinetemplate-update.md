---
title: "Update securityBaselineTemplate"
description: "Update the properties of a securityBaselineTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update securityBaselineTemplate

Namespace: microsoft.graph

Update the properties of a [securityBaselineTemplate](../resources/securitybaselinetemplate.md) object.

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
PATCH ** Entity URI for microsoft.graph.securityBaselineTemplate not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/securitybaselinetemplate.md) object.

The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/securitybaselinetemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The template's display name Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|description|String|The template's description Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|versionInfo|String|The template's version information Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|isDeprecated|Boolean|The template is deprecated or not. Intents cannot be created from a deprecated template. Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|intentCount|Int32|Number of Intents created from this template. Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|templateType|Enumeration|The template's type. Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md). Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.|
|platformType|Enumeration|The template's platform. Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md). Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|publishedDateTime|DateTimeOffset|When the template was published Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/securitybaselinetemplate.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_securitybaselinetemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.securityBaselineTemplate not found
Content-type: application/json
Content-length: 351

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "String",
  "platformType": "String",
  "publishedDateTime": "2016-12-31T23:58:08.6084682+03:00"
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
Content-Length: 400

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "c06e3ed2-3ed2-c06e-d23e-6ec0d23e6ec0",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "String",
  "platformType": "String",
  "publishedDateTime": "2016-12-31T23:58:08.6084682+03:00"
}
```

