---
title: "deviceCompliancePolicySettingState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceCompliancePolicySettingState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|currentValue|String|**TODO: Add Description**|
|errorCode|Int64|**TODO: Add Description**|
|errorDescription|String|**TODO: Add Description**|
|instanceDisplayName|String|**TODO: Add Description**|
|setting|String|**TODO: Add Description**|
|settingInstanceId|String|**TODO: Add Description**|
|settingName|String|**TODO: Add Description**|
|sources|[settingSource](../resources/settingsource.md) collection|**TODO: Add Description**|
|state|complianceStatus|**TODO: Add Description**. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userEmail|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": "Integer",
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```

