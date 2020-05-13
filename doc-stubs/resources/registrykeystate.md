---
title: "registryKeyState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# registryKeyState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|hive|registryHive|**TODO: Add Description**. Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`, `unknownFutureValue`.|
|key|String|**TODO: Add Description**|
|oldKey|String|**TODO: Add Description**|
|oldValueData|String|**TODO: Add Description**|
|oldValueName|String|**TODO: Add Description**|
|operation|registryOperation|**TODO: Add Description**. Possible values are: `unknown`, `create`, `modify`, `delete`, `unknownFutureValue`.|
|processId|Int32|**TODO: Add Description**|
|valueData|String|**TODO: Add Description**|
|valueName|String|**TODO: Add Description**|
|valueType|registryValueType|**TODO: Add Description**. Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.registryKeyState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.registryKeyState",
  "hive": "String",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "String",
  "processId": "Integer",
  "valueData": "String",
  "valueName": "String",
  "valueType": "String"
}
```

