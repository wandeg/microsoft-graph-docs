---
title: "Add groupPolicySettingMappings"
description: "Add groupPolicySettingMappings by posting to the groupPolicySettingMappings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add groupPolicySettingMappings

Namespace: microsoft.graph

Add groupPolicySettingMappings by posting to the groupPolicySettingMappings collection.

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
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.

The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|parentId|String||
|childIdList|String collection||
|settingName|String||
|settingValue|String||
|settingValueType|String||
|settingDisplayName|String||
|settingDisplayValue|String||
|settingDisplayValueType|String||
|settingValueDisplayUnits|String||
|settingCategory|String||
|mdmCspName|String||
|mdmSettingUri|String||
|mdmMinimumOSVersion|Int32||
|settingType|Enumeration| Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|isMdmSupported|Boolean||
|mdmSupportedState|Enumeration| Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.|
|settingScope|Enumeration| Possible values are: `unknown`, `device`, `user`.|
|intuneSettingUriList|String collection||
|intuneSettingDefinitionId|String||



## Response
If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouppolicysettingmapping_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
Content-type: application/json
Content-length: 954

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicysettingmapping"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1003

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "aa8e8e41-8e41-aa8e-418e-8eaa418e8eaa",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value"
}
```

