---
title: "provisioningObjectSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# provisioningObjectSummary resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List provisioningObjectSummaries](../api/provisioningobjectsummary-list.md)|[provisioningObjectSummary](../resources/provisioningObjectSummary.md) collection|List properties and relationships of the [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects.|
|[Get provisioningObjectSummary](../api/provisioningobjectsummary-get.md)|[provisioningObjectSummary](../resources/provisioningObjectSummary.md)|Read properties and relationships of the [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.|
|[Create provisioningObjectSummary](../api/provisioningobjectsummary-create.md)|[provisioningObjectSummary](../resources/provisioningObjectSummary.md)|Create a new [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.|
|[Delete provisioningObjectSummary](../api/provisioningobjectsummary-delete.md)|None|Deletes a [provisioningObjectSummary](../resources/provisioningobjectsummary.md).|
|[Update provisioningObjectSummary](../api/provisioningobjectsummary-update.md)|[provisioningObjectSummary](../resources/provisioningObjectSummary.md)|Update the properties of a [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.|

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
|modifiedProperties|[modifiedProperty](../resources/modifiedProperty.md) collection||
|provisioningSteps|[provisioningStep](../resources/provisioningStep.md) collection||
|sourceIdentity|[provisionedIdentity](../resources/provisionedIdentity.md)||
|sourceSystem|[provisioningSystemDetails](../resources/provisioningSystemDetails.md)||
|statusInfo|[statusBase](../resources/statusBase.md)||
|targetIdentity|[provisionedIdentity](../resources/provisionedIdentity.md)||
|targetSystem|[provisioningSystemDetails](../resources/provisioningSystemDetails.md)||
|tenantId|String||

## Relationships
None

## JSON Representation
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

