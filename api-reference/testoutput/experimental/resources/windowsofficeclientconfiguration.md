---
title: "windowsOfficeClientConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsOfficeClientConfiguration resource type




Inherits from [officeClientConfiguration](../resources/officeClientConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsOfficeClientConfigurations](../api/windowsofficeclientconfiguration-list.md)|[windowsOfficeClientConfiguration](../resources/windowsOfficeClientConfiguration.md) collection|List properties and relationships of the [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) objects.|
|[Get windowsOfficeClientConfiguration](../api/windowsofficeclientconfiguration-get.md)|[windowsOfficeClientConfiguration](../resources/windowsOfficeClientConfiguration.md)|Read properties and relationships of the [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) object.|
|[Create windowsOfficeClientConfiguration](../api/windowsofficeclientconfiguration-create.md)|[windowsOfficeClientConfiguration](../resources/windowsOfficeClientConfiguration.md)|Create a new [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) object.|
|[Delete windowsOfficeClientConfiguration](../api/windowsofficeclientconfiguration-delete.md)|None|Deletes a [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md).|
|[Update windowsOfficeClientConfiguration](../api/windowsofficeclientconfiguration-update.md)|[windowsOfficeClientConfiguration](../resources/windowsOfficeClientConfiguration.md)|Update the properties of a [windowsOfficeClientConfiguration](../resources/windowsofficeclientconfiguration.md) object.|
|[assign](../api/windowsofficeclientconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md) collection||
|[List assignments](../api/windowsofficeclientconfiguration-list-assignments.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md) collection|Get the officeClientConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsofficeclientconfiguration-post-assignments.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checkinStatuses|[officeClientCheckinStatus](../resources/officeClientCheckinStatus.md) collection| Inherited from [officeClientConfiguration](../resources/officeClientConfiguration.md)|
|description|String| Inherited from [officeClientConfiguration](../resources/officeClientConfiguration.md)|
|displayName|String| Inherited from [officeClientConfiguration](../resources/officeClientConfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|policyPayload|Stream| Inherited from [officeClientConfiguration](../resources/officeClientConfiguration.md)|
|priority|Int32| Inherited from [officeClientConfiguration](../resources/officeClientConfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/officeUserCheckinSummary.md)| Inherited from [officeClientConfiguration](../resources/officeClientConfiguration.md)|
|userPreferencePayload|Stream| Inherited from [officeClientConfiguration](../resources/officeClientConfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md) collection| Inherited from [officeClientConfiguration](../resources/officeClientConfiguration.md)|

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

