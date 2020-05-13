---
title: "managedAppPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedAppPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List appliedPolicies](../api/intune-managedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Create appliedPolicies](../api/intune-managedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Create a new appliedPolicies object.|
|[Delete appliedPolicies](../api/intune-managedappregistration-delete-appliedpolicies.md)|None|Delete a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[Update appliedPolicies](../api/intune-managedappregistration-update-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Update the properties of an appliedPolicies object.|
|[Get appliedPolicies](../api/intune-managedappregistration-get-managedapppolicy.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Read the properties and relationships of a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[targetApps](../api/intune-managedapppolicy-targetapps.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "String"
}
```

