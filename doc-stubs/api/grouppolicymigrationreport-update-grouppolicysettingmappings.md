---
title: "Update groupPolicySettingMappings"
description: "Update the properties of a groupPolicySettingMappings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update groupPolicySettingMappings

Namespace: microsoft.graph

Update the properties of a groupPolicySettingMappings object.

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
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.

The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|parentId|String|**TODO: Add Description**|
|childIdList|String collection|**TODO: Add Description**|
|settingName|String|**TODO: Add Description**|
|settingValue|String|**TODO: Add Description**|
|settingValueType|String|**TODO: Add Description**|
|settingDisplayName|String|**TODO: Add Description**|
|settingDisplayValue|String|**TODO: Add Description**|
|settingDisplayValueType|String|**TODO: Add Description**|
|settingValueDisplayUnits|String|**TODO: Add Description**|
|settingCategory|String|**TODO: Add Description**|
|mdmCspName|String|**TODO: Add Description**|
|mdmSettingUri|String|**TODO: Add Description**|
|mdmMinimumOSVersion|Int32|**TODO: Add Description**|
|settingType|groupPolicySettingType|**TODO: Add Description**. Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|isMdmSupported|Boolean|**TODO: Add Description**|
|mdmSupportedState|mdmSupportedState|**TODO: Add Description**. Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.|
|settingScope|groupPolicySettingScope|**TODO: Add Description**. Possible values are: `unknown`, `device`, `user`.|
|intuneSettingUriList|String collection|**TODO: Add Description**|
|intuneSettingDefinitionId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_grouppolicysettingmappings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
Content-Type: application/json
Content-length: 714

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": "Integer",
  "settingType": "String",
  "isMdmSupported": "Boolean",
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ],
  "intuneSettingDefinitionId": "String"
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
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "80962cfe-2cfe-8096-fe2c-9680fe2c9680",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": "Integer",
  "settingType": "String",
  "isMdmSupported": "Boolean",
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ],
  "intuneSettingDefinitionId": "String"
}
```

