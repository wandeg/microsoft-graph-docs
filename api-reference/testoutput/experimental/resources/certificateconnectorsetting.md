---
title: "certificateConnectorSetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# certificateConnectorSetting resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|certExpiryTime|DateTimeOffset|Certificate expire time|
|connectorVersion|String|Version of certificate connector|
|enrollmentError|String|Certificate connector enrollment error|
|lastConnectorConnectionTime|DateTimeOffset|Last time certificate connector connected|
|lastUploadVersion|Int64|Version of last uploaded certificate connector|
|status|Int32|Certificate connector status|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```

