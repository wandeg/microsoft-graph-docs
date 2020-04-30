---
title: "directoryAudit resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directoryAudit resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get directoryAudit](../api/microsoft.aad.reporting-directoryaudit-get.md)|[directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md)|Read properties and relationships of a [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object.|
|[Update directoryAudit](../api/microsoft.aad.reporting-directoryaudit-update.md)|[directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md)|Update the properties of a [directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|activityDisplayName|String|**TODO: Add Description**|
|additionalDetails|[keyValue](../resources/microsoft.aad.reporting-keyvalue.md) collection|**TODO: Add Description**|
|category|String|**TODO: Add Description**|
|correlationId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|initiatedBy|[auditActivityInitiator](../resources/microsoft.aad.reporting-auditactivityinitiator.md)|**TODO: Add Description**|
|loggedByService|String|**TODO: Add Description**|
|operationType|String|**TODO: Add Description**|
|result|operationResult|**TODO: Add Description**. Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.|
|resultReason|String|**TODO: Add Description**|
|targetResources|[targetResource](../resources/microsoft.aad.reporting-targetresource.md) collection|**TODO: Add Description**|

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

