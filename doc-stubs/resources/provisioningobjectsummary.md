---
title: "provisioningObjectSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# provisioningObjectSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|String|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|changeId|String|**TODO: Add Description**|
|cycleId|String|**TODO: Add Description**|
|durationInMilliseconds|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|initiatedBy|[initiator](../resources/initiator.md)|**TODO: Add Description**|
|jobId|String|**TODO: Add Description**|
|modifiedProperties|[modifiedProperty](../resources/modifiedproperty.md) collection|**TODO: Add Description**|
|provisioningSteps|[provisioningStep](../resources/provisioningstep.md) collection|**TODO: Add Description**|
|servicePrincipal|[provisioningServicePrincipal](../resources/provisioningserviceprincipal.md)|**TODO: Add Description**|
|sourceIdentity|[provisionedIdentity](../resources/provisionedidentity.md)|**TODO: Add Description**|
|sourceSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)|**TODO: Add Description**|
|statusInfo|[statusBase](../resources/statusbase.md)|**TODO: Add Description**|
|targetIdentity|[provisionedIdentity](../resources/provisionedidentity.md)|**TODO: Add Description**|
|targetSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "baseType": "",
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
  "durationInMilliseconds": "Integer",
  "servicePrincipal": {
    "@odata.type": "microsoft.graph.provisioningServicePrincipal"
  },
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

