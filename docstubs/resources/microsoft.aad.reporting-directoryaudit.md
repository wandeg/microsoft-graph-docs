---
title: "directoryAudit resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# directoryAudit resource type


Namespace: Microsoft.AAD.Reporting



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get directoryAudit](../api/microsoft.aad.reporting-directoryaudit-get.md)|[directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md)|Read properties and relationships of the [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object.|
|[Update directoryAudit](../api/microsoft.aad.reporting-directoryaudit-update.md)|[directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md)|Update the properties of a [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityDateTime|DateTimeOffset||
|activityDisplayName|String||
|additionalDetails|[keyValue](../resources/microsoft.aad.reporting-keyvalue.md) collection||
|category|String||
|correlationId|String||
|id|String||
|initiatedBy|[auditActivityInitiator](../resources/microsoft.aad.reporting-auditactivityinitiator.md)||
|loggedByService|String||
|operationType|String||
|result|Enumeration| Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.|
|resultReason|String||
|targetResources|[targetResource](../resources/microsoft.aad.reporting-targetresource.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.directoryAudit",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.directoryAudit",
  "id": "String (identifier)",
  "category": "String",
  "correlationId": "String",
  "result": "String",
  "resultReason": "String",
  "activityDisplayName": "String",
  "activityDateTime": "String (timestamp)",
  "loggedByService": "String",
  "operationType": "String",
  "initiatedBy": {
    "@odata.type": "Microsoft.AAD.Reporting.auditActivityInitiator"
  },
  "targetResources": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.targetResource"
    }
  ],
  "additionalDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.keyValue"
    }
  ]
}
```

