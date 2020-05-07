---
title: "Update unsupportedGroupPolicyExtensions"
description: "Update the properties of an unsupportedGroupPolicyExtensions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update unsupportedGroupPolicyExtensions

Namespace: microsoft.graph

Update the properties of an unsupportedGroupPolicyExtensions object.

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
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object.

The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settingScope|groupPolicySettingScope|**TODO: Add Description**. Possible values are: `unknown`, `device`, `user`.|
|namespaceUrl|String|**TODO: Add Description**|
|extensionType|String|**TODO: Add Description**|
|nodeName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unsupportedgrouppolicyextensions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
Content-Type: application/json
Content-length: 186

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "settingScope": "String",
  "namespaceUrl": "String",
  "extensionType": "String",
  "nodeName": "String"
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
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "dfe4bd34-bd34-dfe4-34bd-e4df34bde4df",
  "settingScope": "String",
  "namespaceUrl": "String",
  "extensionType": "String",
  "nodeName": "String"
}
```

