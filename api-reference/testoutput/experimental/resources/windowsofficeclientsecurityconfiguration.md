---
title: "windowsOfficeClientSecurityConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsOfficeClientSecurityConfiguration resource type


Namespace: microsoft.graph




Inherits from [officeClientConfiguration](../resources/officeclientconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsOfficeClientSecurityConfigurations](../api/windowsofficeclientsecurityconfiguration-list.md)|[windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) collection|List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) objects.|
|[Get windowsOfficeClientSecurityConfiguration](../api/windowsofficeclientsecurityconfiguration-get.md)|[windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md)|Read properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) object.|
|[Create windowsOfficeClientSecurityConfiguration](../api/windowsofficeclientsecurityconfiguration-create.md)|[windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md)|Create a new [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) object.|
|[Delete windowsOfficeClientSecurityConfiguration](../api/windowsofficeclientsecurityconfiguration-delete.md)|None|Deletes a [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md).|
|[Update windowsOfficeClientSecurityConfiguration](../api/windowsofficeclientsecurityconfiguration-update.md)|[windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md)|Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/windowsofficeclientsecurityconfiguration.md) object.|
|[assign](../api/windowsofficeclientsecurityconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) collection||
|[List assignments](../api/windowsofficeclientsecurityconfiguration-list-assignments.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) collection|Get the officeClientConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsofficeclientsecurityconfiguration-post-assignments.md)|[officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

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

