---
title: "windowsOfficeClientSecurityConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsOfficeClientSecurityConfiguration resource type




Inherits from [officeClientConfiguration](../resources/officeClientConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsOfficeClientSecurityConfigurations](../api/windowsofficeclientsecurityconfiguration-list.md)|[windowsOfficeClientSecurityConfiguration](../resources/windowsOfficeClientSecurityConfiguration.md) collection|List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) objects.|
|[Get windowsOfficeClientSecurityConfiguration](../api/windowsofficeclientsecurityconfiguration-get.md)|[windowsOfficeClientSecurityConfiguration](../resources/windowsOfficeClientSecurityConfiguration.md)|Read properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) object.|
|[Create windowsOfficeClientSecurityConfiguration](../api/windowsofficeclientsecurityconfiguration-create.md)|[windowsOfficeClientSecurityConfiguration](../resources/windowsOfficeClientSecurityConfiguration.md)|Create a new [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) object.|
|[Delete windowsOfficeClientSecurityConfiguration](../api/windowsofficeclientsecurityconfiguration-delete.md)|None|Deletes a [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md).|
|[Update windowsOfficeClientSecurityConfiguration](../api/windowsofficeclientsecurityconfiguration-update.md)|[windowsOfficeClientSecurityConfiguration](../resources/windowsOfficeClientSecurityConfiguration.md)|Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) object.|
|[assign](../api/windowsofficeclientsecurityconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md) collection||
|[List assignments](../api/windowsofficeclientsecurityconfiguration-list-assignments.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md) collection|Get the officeClientConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsofficeclientsecurityconfiguration-post-assignments.md)|[officeClientConfigurationAssignment](../resources/officeClientConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|

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
  "@odata.type": "microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "baseType": "microsoft.graph.officeClientConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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

