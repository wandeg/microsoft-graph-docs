---
title: "provisioningObjectSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# provisioningObjectSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get provisioningObjectSummary](../api/provisioningobjectsummary-get.md)|[provisioningObjectSummary](../resources/provisioningobjectsummary.md)|Read properties and relationships of the [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.|
|[Update provisioningObjectSummary](../api/provisioningobjectsummary-update.md)|[provisioningObjectSummary](../resources/provisioningobjectsummary.md)|Update the properties of a [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|String||
|activityDateTime|DateTimeOffset||
|changeId|String||
|cycleId|String||
|durationInMilliseconds|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|initiatedBy|[initiator](../resources/initiator.md)||
|jobId|String||
|modifiedProperties|[modifiedProperty](../resources/modifiedproperty.md) collection||
|provisioningSteps|[provisioningStep](../resources/provisioningstep.md) collection||
|sourceIdentity|[provisionedIdentity](../resources/provisionedidentity.md)||
|sourceSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)||
|statusInfo|[statusBase](../resources/statusbase.md)||
|targetIdentity|[provisionedIdentity](../resources/provisionedidentity.md)||
|targetSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)||
|tenantId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisioningObjectSummary",
  "id": "String (identifier)",
  "activityDateTime": "String (timestamp)",
  "tenantId": "String",
  "jobId": "String",
  "cycleId": "String",
  "changeId": "String",
  "action": "String",
  "durationInMilliseconds": 1024,
  "initiatedBy": {
    "@odata.type": "microsoft.graph.initiator"
  },
  "sourceSystem": {
    "@odata.type": "microsoft.graph.provisioningSystemDetails"
  },
  "targetSystem": {
    "@odata.type": "microsoft.graph.provisioningSystemDetails"
  },
  "sourceIdentity": {
    "@odata.type": "microsoft.graph.provisionedIdentity"
  },
  "targetIdentity": {
    "@odata.type": "microsoft.graph.provisionedIdentity"
  },
  "statusInfo": {
    "@odata.type": "microsoft.graph.statusBase"
  },
  "provisioningSteps": [
    {
      "@odata.type": "microsoft.graph.provisioningStep"
    }
  ],
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.modifiedProperty"
    }
  ]
}
```

