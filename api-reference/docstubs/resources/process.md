---
title: "process resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# process resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountName|String|**TODO: Add Description**|
|commandLine|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|fileHash|[fileHash](../resources/filehash.md)|**TODO: Add Description**|
|integrityLevel|processIntegrityLevel|**TODO: Add Description**. Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`, `unknownFutureValue`.|
|isElevated|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|parentProcessCreatedDateTime|DateTimeOffset|**TODO: Add Description**|
|parentProcessId|Int32|**TODO: Add Description**|
|parentProcessName|String|**TODO: Add Description**|
|path|String|**TODO: Add Description**|
|processId|Int32|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.process"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.process",
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {
    "@odata.type": "microsoft.graph.fileHash",
    "hashType": "String",
    "hashValue": "String"
  },
  "integrityLevel": "String",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}
```

