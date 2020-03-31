---
title: "targetedManagedAppConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# targetedManagedAppConfiguration resource type


Namespace: microsoft.graph




Inherits from [managedAppConfiguration](../resources/managedappconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get targetedManagedAppConfiguration](../api/targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md)|Read properties and relationships of the [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.|
|[Update targetedManagedAppConfiguration](../api/targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md)|Update the properties of a [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.|
|[hasPayloadLinks](../api/targetedmanagedappconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection||
|[assign](../api/targetedmanagedappconfiguration-assign.md)|None||
|[targetApps](../api/targetedmanagedappconfiguration-targetapps.md)|None||
|[List apps](../api/targetedmanagedappconfiguration-list-apps.md)|[managedMobileApp](../resources/managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Add apps](../api/targetedmanagedappconfiguration-post-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Add apps by posting to the apps collection.|
|[Get managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|
|[List assignments](../api/targetedmanagedappconfiguration-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/targetedmanagedappconfiguration-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection| Inherited from [managedAppConfiguration](../resources/managedappconfiguration.md)|
|deployedAppCount|Int32||
|description|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|displayName|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isAssigned|Boolean||
|lastModifiedDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/managedmobileapp.md) collection||
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection||
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration",
  "baseType": "microsoft.graph.managedAppConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```

