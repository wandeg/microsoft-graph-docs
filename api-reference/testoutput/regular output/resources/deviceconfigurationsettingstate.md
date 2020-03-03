---
title: "deviceConfigurationSettingState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceConfigurationSettingState resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|currentValue|String|Current value of setting on device|
|errorCode|Int64|Error code for the setting|
|errorDescription|String|Error description|
|instanceDisplayName|String|Name of setting instance that is being reported.|
|setting|String|The setting that is being reported|
|settingName|String|Localized/user friendly setting name that is being reported|
|sources|[settingSource](../resources/settingSource.md) collection|Contributing policies|
|state|Enumeration|The compliance state of the setting. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userEmail|String|UserEmail|
|userId|String|UserId|
|userName|String|UserName|
|userPrincipalName|String|UserPrincipalName.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```

