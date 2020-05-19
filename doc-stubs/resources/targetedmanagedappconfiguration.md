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
|[assign](../api/targetedmanagedappconfiguration-assign.md)|None|**TODO: Add Description**|
|[targetApps](../api/targetedmanagedappconfiguration-targetapps.md)|None|**TODO: Add Description**|
|[List apps](../api/targetedmanagedappconfiguration-list-apps.md)|[managedMobileApp](../resources/intune-managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Create apps](../api/targetedmanagedappconfiguration-post-apps.md)|[managedMobileApp](../resources/intune-managedmobileapp.md)|Create a new apps object.|
|[Delete apps](../api/targetedmanagedappconfiguration-delete-apps.md)|None|Delete a [managedMobileApp](../resources/intune-managedmobileapp.md) object.|
|[Update apps](../api/targetedmanagedappconfiguration-update-apps.md)|[managedMobileApp](../resources/intune-managedmobileapp.md)|Update the properties of an apps object.|
|[Get apps](../api/targetedmanagedappconfiguration-get-managedmobileapp.md)|[managedMobileApp](../resources/intune-managedmobileapp.md)|Read the properties and relationships of a [managedMobileApp](../resources/intune-managedmobileapp.md) object.|
|[List deploymentSummary](../api/targetedmanagedappconfiguration-list-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/intune-managedapppolicydeploymentsummary.md) collection|Get the managedAppPolicyDeploymentSummaries from the deploymentSummary navigation property.|
|[Create deploymentSummary](../api/targetedmanagedappconfiguration-post-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/intune-managedapppolicydeploymentsummary.md)|Create a new deploymentSummary object.|
|[Delete deploymentSummary](../api/targetedmanagedappconfiguration-delete-deploymentsummary.md)|None|Delete a [managedAppPolicyDeploymentSummary](../resources/intune-managedapppolicydeploymentsummary.md) object.|
|[Update deploymentSummary](../api/targetedmanagedappconfiguration-update-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/intune-managedapppolicydeploymentsummary.md)|Update the properties of a deploymentSummary object.|
|[Get deploymentSummary](../api/targetedmanagedappconfiguration-get-managedapppolicydeploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/intune-managedapppolicydeploymentsummary.md)|Read the properties and relationships of a [managedAppPolicyDeploymentSummary](../resources/intune-managedapppolicydeploymentsummary.md) object.|
|[List assignments](../api/targetedmanagedappconfiguration-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/targetedmanagedappconfiguration-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/targetedmanagedappconfiguration-delete-assignments.md)|None|Delete a [targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) object.|
|[Update assignments](../api/targetedmanagedappconfiguration-update-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/targetedmanagedappconfiguration-get-targetedmanagedapppolicyassignment.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Read the properties and relationships of a [targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/intune-keyvaluepair.md) collection|**TODO: Add Description** Inherited from [managedAppConfiguration](../resources/managedappconfiguration.md)|
|deployedAppCount|Int32|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isAssigned|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/intune-managedmobileapp.md) collection|**TODO: Add Description**|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) collection|**TODO: Add Description**|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-managedapppolicydeploymentsummary.md)|**TODO: Add Description**|

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

