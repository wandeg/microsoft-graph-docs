---
title: "windowsOfficeClientConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsOfficeClientConfiguration resource type


Namespace: microsoft.graph




Inherits from [officeClientConfiguration](../resources/officeclientconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsOfficeClientConfigurations](../api/windowsofficeclientconfiguration-list.md)|[windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) collection|List properties and relationships of the [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) objects.|
|[Get windowsOfficeClientConfiguration](../api/windowsofficeclientconfiguration-get.md)|[windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md)|Read properties and relationships of the [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) object.|
|[Create windowsOfficeClientConfiguration](../api/windowsofficeclientconfiguration-create.md)|[windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md)|Create a new [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) object.|
|[Delete windowsOfficeClientConfiguration](../api/windowsofficeclientconfiguration-delete.md)|None|Deletes a [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md).|
|[Update windowsOfficeClientConfiguration](../api/windowsofficeclientconfiguration-update.md)|[windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md)|Update the properties of a [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) object.|
|[assign](../api/windowsofficeclientconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) collection||
|[List assignments](../api/windowsofficeclientconfiguration-list-assignments.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) collection|Get the officeClientConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsofficeclientconfiguration-post-assignments.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checkinStatuses|[officeClientCheckinStatus](../resources/officeclientcheckinstatus.md) collection| Inherited from [officeClientConfiguration](../resources/officeclientconfiguration.md)|
|description|String| Inherited from [officeClientConfiguration](../resources/officeclientconfiguration.md)|
|displayName|String| Inherited from [officeClientConfiguration](../resources/officeclientconfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|policyPayload|Stream| Inherited from [officeClientConfiguration](../resources/officeclientconfiguration.md)|
|priority|Int32| Inherited from [officeClientConfiguration](../resources/officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/officeusercheckinsummary.md)| Inherited from [officeClientConfiguration](../resources/officeclientconfiguration.md)|
|userPreferencePayload|Stream| Inherited from [officeClientConfiguration](../resources/officeclientconfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) collection| Inherited from [officeClientConfiguration](../resources/officeclientconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientConfiguration",
  "baseType": "microsoft.graph.officeClientConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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

