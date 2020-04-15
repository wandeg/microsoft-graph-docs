---
title: "provisioningObjectSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# provisioningObjectSummary resource type


Namespace: Microsoft.AAD.Reporting



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get provisioningObjectSummary](../api/microsoft.aad.reporting-provisioningobjectsummary-get.md)|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md)|Read properties and relationships of the [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.|
|[Update provisioningObjectSummary](../api/microsoft.aad.reporting-provisioningobjectsummary-update.md)|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md)|Update the properties of a [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|String||
|activityDateTime|DateTimeOffset||
|changeId|String||
|cycleId|String||
|durationInMilliseconds|Int32||
|id|String||
|initiatedBy|[initiator](../resources/microsoft.aad.reporting-initiator.md)||
|jobId|String||
|modifiedProperties|[modifiedProperty](../resources/microsoft.aad.reporting-modifiedproperty.md) collection||
|provisioningSteps|[provisioningStep](../resources/microsoft.aad.reporting-provisioningstep.md) collection||
|sourceIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)||
|sourceSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)||
|statusInfo|[statusBase](../resources/microsoft.aad.reporting-statusbase.md)||
|targetIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)||
|targetSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)||
|tenantId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.provisioningObjectSummary",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
  "id": "String (identifier)",
  "activityDateTime": "String (timestamp)",
  "tenantId": "String",
  "jobId": "String",
  "cycleId": "String",
  "changeId": "String",
  "action": "String",
  "durationInMilliseconds": 1024,
  "initiatedBy": {
    "@odata.type": "Microsoft.AAD.Reporting.initiator"
  },
  "sourceSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
  },
  "targetSystem": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
  },
  "sourceIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
  },
  "targetIdentity": {
    "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
  },
  "statusInfo": {
    "@odata.type": "Microsoft.AAD.Reporting.statusBase"
  },
  "provisioningSteps": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.provisioningStep"
    }
  ],
  "modifiedProperties": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty"
    }
  ]
}
```

