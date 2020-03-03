---
title: "managedAppPolicyDeploymentSummary resource type"
description: "The ManagedAppEntity is the base entity type for all other entity types under app management workflow."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedAppPolicyDeploymentSummary resource type

The ManagedAppEntity is the base entity type for all other entity types under app management workflow.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAppPolicyDeploymentSummaries](../api/managedapppolicydeploymentsummary-list.md)|[managedAppPolicyDeploymentSummary](../resources/managedAppPolicyDeploymentSummary.md) collection|List properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) objects.|
|[Get managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/managedAppPolicyDeploymentSummary.md)|Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|
|[Create managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-create.md)|[managedAppPolicyDeploymentSummary](../resources/managedAppPolicyDeploymentSummary.md)|Create a new [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|
|[Delete managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-delete.md)|None|Deletes a [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md).|
|[Update managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-update.md)|[managedAppPolicyDeploymentSummary](../resources/managedAppPolicyDeploymentSummary.md)|Update the properties of a [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationDeployedUserCount|Int32||
|configurationDeploymentSummaryPerApp|[managedAppPolicyDeploymentSummaryPerApp](../resources/managedAppPolicyDeploymentSummaryPerApp.md) collection||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastRefreshTime|DateTimeOffset||
|version|String|Version of the entity.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "configurationDeployedUserCount": 1024,
  "lastRefreshTime": "String (timestamp)",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
    }
  ],
  "version": "String"
}
```

