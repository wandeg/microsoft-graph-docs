---
title: "targetedManagedAppConfiguration resource type"
description: "Configuration used to deliver a set of custom settings as-is to all users in the targeted security group"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# targetedManagedAppConfiguration resource type


Namespace: microsoft.graph

Configuration used to deliver a set of custom settings as-is to all users in the targeted security group


Inherits from [managedAppConfiguration](../resources/managedappconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List targetedManagedAppConfigurations](../api/targetedmanagedappconfiguration-list.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) collection|List properties and relationships of the [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) objects.|
|[Get targetedManagedAppConfiguration](../api/targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md)|Read properties and relationships of the [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.|
|[Create targetedManagedAppConfiguration](../api/targetedmanagedappconfiguration-create.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md)|Create a new [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.|
|[Delete targetedManagedAppConfiguration](../api/targetedmanagedappconfiguration-delete.md)|None|Deletes a [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md).|
|[Update targetedManagedAppConfiguration](../api/targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md)|Update the properties of a [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.|
|[hasPayloadLinks](../api/targetedmanagedappconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection||
|[assign](../api/targetedmanagedappconfiguration-assign.md)|None||
|[targetApps](../api/targetedmanagedappconfiguration-targetapps.md)|None||
|[List apps](../api/targetedmanagedappconfiguration-list-apps.md)|[managedMobileApp](../resources/managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Add apps](../api/targetedmanagedappconfiguration-post-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Add apps by posting to the apps collection.|
|[Get managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|
|[List assignments](../api/targetedmanagedappconfiguration-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/targetedmanagedappconfiguration-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Add assignments by posting to the assignments collection.|
|[List targetedManagedAppConfigurations](../api/intune-apps-deviceappmanagement-list-targetedmanagedappconfigurations.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) collection|Get the targetedManagedAppConfigurations from the targetedManagedAppConfigurations navigation property.|
|[Add targetedManagedAppConfigurations](../api/intune-apps-deviceappmanagement-post-targetedmanagedappconfigurations.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md)|Add targetedManagedAppConfigurations by posting to the targetedManagedAppConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the policy was created. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/managedappconfiguration.md)|
|deployedAppCount|Int32|Count of apps to which the current policy is deployed.|
|description|String|The policy's description. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|displayName|String|Policy display name. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isAssigned|Boolean|Indicates if the policy is deployed to any inclusion groups or not.|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String|Version of the entity. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/managedmobileapp.md) collection|List of apps to which the policy is deployed.|
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Navigation property to list of inclusion and exclusion groups to which the policy is deployed.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Navigation property to deployment summary of the configuration.|

## JSON Representation
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

