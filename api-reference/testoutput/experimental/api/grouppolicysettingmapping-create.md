---
title: "Create groupPolicySettingMapping"
description: "Create a new groupPolicySettingMapping object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create groupPolicySettingMapping

Namespace: microsoft.graph

Create a new [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.

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
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.

The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|parentId|String|Parent Id of the group policy setting.|
|childIdList|String collection|List of Child Ids of the group policy setting.|
|settingName|String|The name of this group policy setting.|
|settingValue|String|The value of this group policy setting.|
|settingValueType|String|The value type of this group policy setting.|
|settingDisplayName|String|The display name of this group policy setting.|
|settingDisplayValue|String|The display value of this group policy setting.|
|settingDisplayValueType|String|The display value type of this group policy setting.|
|settingValueDisplayUnits|String|The display units of this group policy setting value|
|settingCategory|String|The category the group policy setting is in.|
|mdmCspName|String|The CSP name this group policy setting maps to.|
|mdmSettingUri|String|The MDM CSP URI this group policy setting maps to.|
|mdmMinimumOSVersion|Int32|The minimum OS version this mdm setting supports.|
|settingType|Enumeration|The setting type (security or admx) of the Group Policy. Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|isMdmSupported|Boolean|Indicates if the setting is supported by Intune or not|
|mdmSupportedState|Enumeration|Indicates if the setting is supported in Mdm or not. Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.|
|settingScope|Enumeration|The scope of the setting. Possible values are: `unknown`, `device`, `user`.|
|intuneSettingUriList|String collection|The list of Intune Setting URIs this group policy setting maps to|



## Response
If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouppolicysettingmapping_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
Content-type: application/json
Content-length: 884

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
  ]
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
Content-Length: 933

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "20835d7c-5d7c-2083-7c5d-83207c5d8320",
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
  ]
}
```

