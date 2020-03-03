---
title: "auditLogRoot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# auditLogRoot resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List auditLogRoots](../api/auditlogroot-list.md)|[auditLogRoot](../resources/auditLogRoot.md) collection|List properties and relationships of the [auditLogRoot](../resources/auditlogroot.md) objects.|
|[Get auditLogRoot](../api/auditlogroot-get.md)|[auditLogRoot](../resources/auditLogRoot.md)|Read properties and relationships of the [auditLogRoot](../resources/auditlogroot.md) object.|
|[Create auditLogRoot](../api/auditlogroot-create.md)|[auditLogRoot](../resources/auditLogRoot.md)|Create a new [auditLogRoot](../resources/auditlogroot.md) object.|
|[Delete auditLogRoot](../api/auditlogroot-delete.md)|None|Deletes a [auditLogRoot](../resources/auditlogroot.md).|
|[Update auditLogRoot](../api/auditlogroot-update.md)|[auditLogRoot](../resources/auditLogRoot.md)|Update the properties of a [auditLogRoot](../resources/auditlogroot.md) object.|
|[List signIns](../api/auditlogroot-list-signins.md)|[signIn](../resources/signIn.md) collection|Get the signIns from the signIns navigation property.|
|[Add signIns](../api/auditlogroot-post-signins.md)|[signIn](../resources/signIn.md)|Add signIns by posting to the signIns collection.|
|[List directoryAudits](../api/auditlogroot-list-directoryaudits.md)|[directoryAudit](../resources/directoryAudit.md) collection|Get the directoryAudits from the directoryAudits navigation property.|
|[Add directoryAudits](../api/auditlogroot-post-directoryaudits.md)|[directoryAudit](../resources/directoryAudit.md)|Add directoryAudits by posting to the directoryAudits collection.|
|[List restrictedSignIns](../api/auditlogroot-list-restrictedsignins.md)|[restrictedSignIn](../resources/restrictedSignIn.md) collection|Get the restrictedSignIns from the restrictedSignIns navigation property.|
|[Add restrictedSignIns](../api/auditlogroot-post-restrictedsignins.md)|[restrictedSignIn](../resources/restrictedSignIn.md)|Add restrictedSignIns by posting to the restrictedSignIns collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directoryAudits|[directoryAudit](../resources/directoryAudit.md) collection||
|restrictedSignIns|[restrictedSignIn](../resources/restrictedSignIn.md) collection||
|signIns|[signIn](../resources/signIn.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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

