---
title: "officeClientConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# officeClientConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get officeClientConfiguration](../api/officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/officeclientconfiguration.md)|Read the properties and relationships of an [officeClientConfiguration](../resources/officeclientconfiguration.md) object.|
|[assign](../api/officeclientconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) collection|**TODO: Add Description**|
|[updatePriorities](../api/officeclientconfiguration-updatepriorities.md)|None|**TODO: Add Description**|
|[List assignments](../api/officeclientconfiguration-list-assignments.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) collection|Get the officeClientConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/officeclientconfiguration-post-assignments.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/officeclientconfiguration-delete-assignments.md)|None|Delete an [officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) object.|
|[Update assignments](../api/officeclientconfiguration-update-assignments.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get officeClientConfigurationAssignment](../api/officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md)|Read the properties and relationships of an [officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checkinStatuses|[officeClientCheckinStatus](../resources/officeclientcheckinstatus.md) collection|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|policyPayload|Stream|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|userCheckinSummary|[officeUserCheckinSummary](../resources/officeusercheckinsummary.md)|**TODO: Add Description**|
|userPreferencePayload|Stream|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) collection|**TODO: Add Description**|

## JSON representation
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

