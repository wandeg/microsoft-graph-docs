---
title: "targetedManagedAppConfiguration resource type"
description: "Configuration used to deliver a set of custom settings as-is to all users in the targeted security group"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# targetedManagedAppConfiguration resource type


Namespace: microsoft.graph

Configuration used to deliver a set of custom settings as-is to all users in the targeted security group


Inherits from [managedAppConfiguration](../resources/managedappconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get targetedManagedAppConfiguration](../api/targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md)|Read the properties and relationships of a [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.|
|[Update targetedManagedAppConfiguration](../api/targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md)|Update the properties of a [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.|
|[hasPayloadLinks](../api/targetedmanagedappconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[assign](../api/targetedmanagedappconfiguration-assign.md)|None|**TODO: Add Description**|
|[targetApps](../api/targetedmanagedappconfiguration-targetapps.md)|None|**TODO: Add Description**|
|[List apps](../api/targetedmanagedappconfiguration-list-apps.md)|[managedMobileApp](../resources/managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Create apps](../api/targetedmanagedappconfiguration-post-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Create a new apps object.|
|[Delete apps](../api/targetedmanagedappconfiguration-delete-apps.md)|None|Delete an [managedMobileApp](../resources/managedmobileapp.md) object.|
|[Update apps](../api/targetedmanagedappconfiguration-update-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Update the properties of an apps object.|
|[Get managedMobileApp](../api/managedmobileapp-get.md)|[managedMobileApp](../resources/managedmobileapp.md)|Read the properties and relationships of a [managedMobileApp](../resources/managedmobileapp.md) object.|
|[List deploymentSummary](../api/targetedmanagedappconfiguration-list-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) collection|Get the managedAppPolicyDeploymentSummaries from the deploymentSummary navigation property.|
|[Create deploymentSummary](../api/targetedmanagedappconfiguration-post-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Create a new deploymentSummary object.|
|[Delete deploymentSummary](../api/targetedmanagedappconfiguration-delete-deploymentsummary.md)|None|Delete a [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|
|[Update deploymentSummary](../api/targetedmanagedappconfiguration-update-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Update the properties of a deploymentSummary object.|
|[Get managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Read the properties and relationships of a [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|
|[List assignments](../api/targetedmanagedappconfiguration-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/targetedmanagedappconfiguration-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/targetedmanagedappconfiguration-delete-assignments.md)|None|Delete an [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|
|[Update assignments](../api/targetedmanagedappconfiguration-update-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Update the properties of an assignments object.|
|[Get targetedManagedAppPolicyAssignment](../api/targetedmanagedapppolicyassignment-get.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Read the properties and relationships of a [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the policy was created. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/managedappconfiguration.md)|
|deployedAppCount|Int32|Count of apps to which the current policy is deployed.|
|description|String|The policy's description. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|displayName|String|Policy display name. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

