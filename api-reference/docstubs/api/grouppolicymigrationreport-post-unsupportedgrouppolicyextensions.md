---
title: "Create unsupportedGroupPolicyExtensions"
description: "Create a new unsupportedGroupPolicyExtensions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create unsupportedGroupPolicyExtensions

Namespace: microsoft.graph

Create a new unsupportedGroupPolicyExtensions object.

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
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object.

The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settingScope|groupPolicySettingScope|Setting Scope of the unsupported extension. Possible values are: `unknown`, `device`, `user`.|
|namespaceUrl|String|Namespace Url of the unsupported extension.|
|extensionType|String|ExtensionType of the unsupported extension.|
|nodeName|String|Node name of the unsupported extension.|



## Response
If successful, this method returns a `201 Created` response code and an [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_unsupportedgrouppolicyextension_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unsupportedgrouppolicyextension"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "ca59d819-d819-ca59-19d8-59ca19d859ca",
  "settingScope": "String",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```

