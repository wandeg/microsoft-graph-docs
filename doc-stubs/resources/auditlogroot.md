---
title: "auditLogRoot resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# auditLogRoot resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List signIns](../api/auditlogroot-list-signins.md)|[signIn](../resources/signin.md) collection|Get the signIns from the signIns navigation property.|
|[Create signIns](../api/auditlogroot-post-signins.md)|[signIn](../resources/signin.md)|Create a new signIns object.|
|[Delete signIns](../api/auditlogroot-delete-signins.md)|None|Delete a [signIn](../resources/signin.md) object.|
|[Update signIns](../api/auditlogroot-update-signins.md)|[signIn](../resources/signin.md)|Update the properties of a signIns object.|
|[Get signIns](../api/auditlogroot-get-signin.md)|[signIn](../resources/signin.md)|Read the properties and relationships of a [signIn](../resources/signin.md) object.|
|[List directoryAudits](../api/auditlogroot-list-directoryaudits.md)|[directoryAudit](../resources/directoryaudit.md) collection|Get the directoryAudits from the directoryAudits navigation property.|
|[Create directoryAudits](../api/auditlogroot-post-directoryaudits.md)|[directoryAudit](../resources/directoryaudit.md)|Create a new directoryAudits object.|
|[Delete directoryAudits](../api/auditlogroot-delete-directoryaudits.md)|None|Delete a [directoryAudit](../resources/directoryaudit.md) object.|
|[Update directoryAudits](../api/auditlogroot-update-directoryaudits.md)|[directoryAudit](../resources/directoryaudit.md)|Update the properties of a directoryAudits object.|
|[Get directoryAudits](../api/auditlogroot-get-directoryaudit.md)|[directoryAudit](../resources/directoryaudit.md)|Read the properties and relationships of a [directoryAudit](../resources/directoryaudit.md) object.|
|[List restrictedSignIns](../api/auditlogroot-list-restrictedsignins.md)|[restrictedSignIn](../resources/restrictedsignin.md) collection|Get the restrictedSignIns from the restrictedSignIns navigation property.|
|[Create restrictedSignIns](../api/auditlogroot-post-restrictedsignins.md)|[restrictedSignIn](../resources/restrictedsignin.md)|Create a new restrictedSignIns object.|
|[Delete restrictedSignIns](../api/auditlogroot-delete-restrictedsignins.md)|None|Delete a [restrictedSignIn](../resources/restrictedsignin.md) object.|
|[Update restrictedSignIns](../api/auditlogroot-update-restrictedsignins.md)|[restrictedSignIn](../resources/restrictedsignin.md)|Update the properties of a restrictedSignIns object.|
|[Get restrictedSignIns](../api/auditlogroot-get-restrictedsignin.md)|[restrictedSignIn](../resources/restrictedsignin.md)|Read the properties and relationships of a [restrictedSignIn](../resources/restrictedsignin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directoryAudits|[directoryAudit](../resources/directoryaudit.md) collection|**TODO: Add Description**|
|restrictedSignIns|[restrictedSignIn](../resources/restrictedsignin.md) collection|**TODO: Add Description**|
|signIns|[signIn](../resources/signin.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditLogRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditLogRoot",
  "id": "String (identifier)"
}
```

