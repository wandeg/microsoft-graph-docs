---
title: "auditLogRoot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# auditLogRoot resource type


Namespace: Microsoft.AAD.Reporting



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get auditLogRoot](../api/microsoft.aad.reporting-auditlogroot-get.md)|[auditLogRoot](../resources/microsoft.aad.reporting-auditlogroot.md)|Read properties and relationships of the [auditLogRoot](../resources/microsoft.aad.reporting-auditlogroot.md) object.|
|[Update auditLogRoot](../api/microsoft.aad.reporting-auditlogroot-update.md)|[auditLogRoot](../resources/microsoft.aad.reporting-auditlogroot.md)|Update the properties of a [auditLogRoot](../resources/microsoft.aad.reporting-auditlogroot.md) object.|
|[List signIns](../api/microsoft.aad.reporting-auditlogroot-list-signins.md)|[signIn](../resources/microsoft.aad.reporting-signin.md) collection|Get the signIns from the signIns navigation property.|
|[Add signIns](../api/microsoft.aad.reporting-auditlogroot-post-signins.md)|[signIn](../resources/microsoft.aad.reporting-signin.md)|Add signIns by posting to the signIns collection.|
|[List directoryAudits](../api/microsoft.aad.reporting-auditlogroot-list-directoryaudits.md)|[directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) collection|Get the directoryAudits from the directoryAudits navigation property.|
|[Add directoryAudits](../api/microsoft.aad.reporting-auditlogroot-post-directoryaudits.md)|[directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md)|Add directoryAudits by posting to the directoryAudits collection.|
|[List restrictedSignIns](../api/microsoft.aad.reporting-auditlogroot-list-restrictedsignins.md)|[restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) collection|Get the restrictedSignIns from the restrictedSignIns navigation property.|
|[Add restrictedSignIns](../api/microsoft.aad.reporting-auditlogroot-post-restrictedsignins.md)|[restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md)|Add restrictedSignIns by posting to the restrictedSignIns collection.|
|[List directoryProvisioning](../api/microsoft.aad.reporting-auditlogroot-list-directoryprovisioning.md)|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) collection|Get the provisioningObjectSummaries from the directoryProvisioning navigation property.|
|[Add directoryProvisioning](../api/microsoft.aad.reporting-auditlogroot-post-directoryprovisioning.md)|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md)|Add directoryProvisioning by posting to the directoryProvisioning collection.|
|[List provisioning](../api/microsoft.aad.reporting-auditlogroot-list-provisioning.md)|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) collection|Get the provisioningObjectSummaries from the provisioning navigation property.|
|[Add provisioning](../api/microsoft.aad.reporting-auditlogroot-post-provisioning.md)|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md)|Add provisioning by posting to the provisioning collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directoryAudits|[directoryAudit](../resources/microsoft.aad.reporting-directoryaudit.md) collection||
|directoryProvisioning|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) collection||
|provisioning|[provisioningObjectSummary](../resources/microsoft.aad.reporting-provisioningobjectsummary.md) collection||
|restrictedSignIns|[restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) collection||
|signIns|[signIn](../resources/microsoft.aad.reporting-signin.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.auditLogRoot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.auditLogRoot"
}
```

