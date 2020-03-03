---
title: "process resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# process resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountName|String||
|commandLine|String||
|createdDateTime|DateTimeOffset||
|fileHash|[fileHash](../resources/fileHash.md)||
|integrityLevel|Enumeration|. Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`, `unknownFutureValue`.|
|isElevated|Boolean||
|name|String||
|parentProcessCreatedDateTime|DateTimeOffset||
|parentProcessId|Int32||
|parentProcessName|String||
|path|String||
|processId|Int32||

## Relationships
None

## JSON Representation
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

