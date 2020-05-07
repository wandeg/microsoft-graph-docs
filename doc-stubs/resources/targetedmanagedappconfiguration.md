---
title: "targetedManagedAppConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# targetedManagedAppConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [managedAppConfiguration](../resources/managedappconfiguration.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
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
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description** Inherited from [managedAppConfiguration](../resources/managedappconfiguration.md)|
|deployedAppCount|Int32|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isAssigned|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/managedmobileapp.md) collection|**TODO: Add Description**|
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|**TODO: Add Description**|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "deployedAppCount": "Integer",
  "isAssigned": "Boolean"
}
```

