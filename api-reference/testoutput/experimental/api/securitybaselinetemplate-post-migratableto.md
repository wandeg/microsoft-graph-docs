---
title: "Add migratableTo"
description: "Add migratableTo by posting to the migratableTo collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add migratableTo

Namespace: microsoft.graph

Add migratableTo by posting to the migratableTo collection.

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
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object.

The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/devicemanagementtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The template's display name|
|description|String|The template's description|
|versionInfo|String|The template's version information|
|isDeprecated|Boolean|The template is deprecated or not. Intents cannot be created from a deprecated template.|
|intentCount|Int32|Number of Intents created from this template.|
|templateType|Enumeration|The template's type. Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.|
|platformType|Enumeration|The template's platform. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|publishedDateTime|DateTimeOffset|When the template was published|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementtemplate_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
Content-type: application/json
Content-length: 351

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementtemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 400

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "3139fa01-fa01-3139-01fa-393101fa3931",
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

