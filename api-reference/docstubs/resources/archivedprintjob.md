---
title: "archivedPrintJob resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# archivedPrintJob resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|acquiredByPrinter|Boolean||
|acquiredDateTime|DateTimeOffset||
|blackAndWhitePageCount|Int32||
|colorPageCount|Int32||
|completionDateTime|DateTimeOffset||
|copiesPrinted|Int32||
|createdBy|[userIdentity](../resources/useridentity.md)||
|createdDateTime|DateTimeOffset||
|duplexPageCount|Int32||
|id|String||
|pageCount|Int32||
|printerId|String||
|processingState|Enumeration| Possible values are: `unknown`, `pending`, `pendingHeld`, `processing`, `paused`, `stopped`, `completed`, `canceled`, `aborted`.|
|simplexPageCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.archivedPrintJob"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.archivedPrintJob",
  "id": "String (identifier)",
  "printerId": "String",
  "processingState": "String",
  "createdDateTime": "String (timestamp)",
  "acquiredDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "acquiredByPrinter": true,
  "copiesPrinted": 1024,
  "pageCount": 1024,
  "blackAndWhitePageCount": 1024,
  "colorPageCount": 1024,
  "simplexPageCount": 1024,
  "duplexPageCount": 1024,
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "String",
    "displayName": "String",
    "ipAddress": "String",
    "userPrincipalName": "String"
  }
}
```

