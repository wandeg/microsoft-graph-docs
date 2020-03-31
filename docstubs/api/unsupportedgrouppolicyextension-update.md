---
title: "Update unsupportedGroupPolicyExtension"
description: "Update the properties of a unsupportedGroupPolicyExtension object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update unsupportedGroupPolicyExtension

Namespace: microsoft.graph

Update the properties of a [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object.

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
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object.

The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settingScope|Enumeration| Possible values are: `unknown`, `device`, `user`.|
|namespaceUrl|String||
|extensionType|String||
|nodeName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_unsupportedgrouppolicyextension"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "settingScope": "String",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
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
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "87afa649-a649-87af-49a6-af8749a6af87",
  "settingScope": "String",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```

