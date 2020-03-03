---
title: "officeClientConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# officeClientConfiguration resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get officeClientConfiguration](../api/officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/officeClientConfiguration.md)|Read properties and relationships of the [officeClientConfiguration](../resources/officeclientconfiguration.md) object.|
|[assign](../api/officeclientconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md) collection||
|[updatePriorities](../api/officeclientconfiguration-updatepriorities.md)|None||
|[List assignments](../api/officeclientconfiguration-list-assignments.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md) collection|Get the officeClientConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/officeclientconfiguration-post-assignments.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List clientConfigurations](../api/officeconfiguration-list-clientconfigurations.md)|[officeClientConfiguration](../resources/officeClientConfiguration.md) collection|Get the officeClientConfigurations from the clientConfigurations navigation property.|
|[Add clientConfigurations](../api/officeconfiguration-post-clientconfigurations.md)|[officeClientConfiguration](../resources/officeClientConfiguration.md)|Add clientConfigurations by posting to the clientConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checkinStatuses|[officeClientCheckinStatus](../resources/officeClientCheckinStatus.md) collection||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|policyPayload|Stream||
|priority|Int32||
|userCheckinSummary|[officeUserCheckinSummary](../resources/officeUserCheckinSummary.md)||
|userPreferencePayload|Stream||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "Stream",
  "policyPayload": "Stream",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```

