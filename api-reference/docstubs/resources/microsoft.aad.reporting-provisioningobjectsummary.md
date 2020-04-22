---
title: "provisioningObjectSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# provisioningObjectSummary resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get provisioningObjectSummary](../api/microsoft.aad.reporting-provisioningobjectsummary-get.md)|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md)|Read properties and relationships of a [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.|
|[Update provisioningObjectSummary](../api/microsoft.aad.reporting-provisioningobjectsummary-update.md)|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md)|Update the properties of a [provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|String|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|changeId|String|**TODO: Add Description**|
|cycleId|String|**TODO: Add Description**|
|durationInMilliseconds|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|initiatedBy|[initiator](../resources/microsoft.aad.reporting-initiator.md)|**TODO: Add Description**|
|jobId|String|**TODO: Add Description**|
|modifiedProperties|[modifiedProperty](../resources/microsoft.aad.reporting-modifiedproperty.md) collection|**TODO: Add Description**|
|provisioningSteps|[provisioningStep](../resources/microsoft.aad.reporting-provisioningstep.md) collection|**TODO: Add Description**|
|servicePrincipal|[provisioningServicePrincipal](../resources/microsoft.aad.reporting-provisioningserviceprincipal.md)|**TODO: Add Description**|
|sourceIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)|**TODO: Add Description**|
|sourceSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)|**TODO: Add Description**|
|statusInfo|[statusBase](../resources/microsoft.aad.reporting-statusbase.md)|**TODO: Add Description**|
|targetIdentity|[provisionedIdentity](../resources/microsoft.aad.reporting-provisionedidentity.md)|**TODO: Add Description**|
|targetSystem|[provisioningSystemDetails](../resources/microsoft.aad.reporting-provisioningsystemdetails.md)|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|

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
  "servicePrincipal": {
    "@odata.type": "Microsoft.AAD.Reporting.provisioningServicePrincipal"
  },
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

