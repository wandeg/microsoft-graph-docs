---
title: "Update templates"
description: "Update the properties of a templates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update templates

Namespace: microsoft.graph

Update the properties of a templates object.

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
PATCH /deviceManagement/templates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object.

The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/devicemanagementtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|versionInfo|String|**TODO: Add Description**|
|isDeprecated|Boolean|**TODO: Add Description**|
|intentCount|Int32|**TODO: Add Description**|
|templateType|deviceManagementTemplateType|**TODO: Add Description**. Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.|
|platformType|policyPlatformType|**TODO: Add Description**. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|publishedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_templates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates
Content-Type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": "Boolean",
  "intentCount": "Integer",
  "templateType": "String",
  "platformType": "String",
  "publishedDateTime": "String (timestamp)"
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
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "287cab18-ab18-287c-18ab-7c2818ab7c28",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": "Boolean",
  "intentCount": "Integer",
  "templateType": "String",
  "platformType": "String",
  "publishedDateTime": "String (timestamp)"
}
```

