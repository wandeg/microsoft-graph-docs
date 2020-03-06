---
title: "deviceManagementExchangeAccessRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementExchangeAccessRule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessLevel|Enumeration|Access Level for Exchange granted by this rule. Possible values are: `none`, `allow`, `block`, `quarantine`.|
|deviceClass|[deviceManagementExchangeDeviceClass](../resources/devicemanagementexchangedeviceclass.md)|Device Class which will be impacted by this rule.|

## Relationships
None

## JSON representation
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

