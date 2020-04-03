---
title: "deviceComplianceSettingState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceSettingState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceComplianceSettingState](../api/devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Read properties and relationships of the [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|
|[Update deviceComplianceSettingState](../api/devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Update the properties of a [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|complianceGracePeriodExpirationDateTime|DateTimeOffset||
|deviceId|String||
|deviceModel|String||
|deviceName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|platformType|Enumeration| Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.|
|setting|String||
|settingName|String||
|state|Enumeration| Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userEmail|String||
|userId|String||
|userName|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "platformType": "String",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```

