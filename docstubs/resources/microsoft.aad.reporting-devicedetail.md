---
title: "deviceDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceDetail resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|browser|String||
|browserId|String||
|deviceId|String||
|displayName|String||
|isCompliant|Boolean||
|isManaged|Boolean||
|operatingSystem|String||
|trustType|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.deviceDetail"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.deviceDetail",
  "deviceId": "String",
  "displayName": "String",
  "operatingSystem": "String",
  "browser": "String",
  "browserId": "String",
  "isCompliant": true,
  "isManaged": true,
  "trustType": "String"
}
```

