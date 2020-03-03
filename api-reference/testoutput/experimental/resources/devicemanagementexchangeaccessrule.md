---
title: "deviceManagementExchangeAccessRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementExchangeAccessRule resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessLevel|Enumeration|Access Level for Exchange granted by this rule. Possible values are: `none`, `allow`, `block`, `quarantine`.|
|deviceClass|[deviceManagementExchangeDeviceClass](../resources/deviceManagementExchangeDeviceClass.md)|Device Class which will be impacted by this rule.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```

