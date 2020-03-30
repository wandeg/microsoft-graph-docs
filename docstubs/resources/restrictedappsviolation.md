---
title: "restrictedAppsViolation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# restrictedAppsViolation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get restrictedAppsViolation](../api/restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Read properties and relationships of the [restrictedAppsViolation](../resources/restrictedappsviolation.md) object.|
|[Update restrictedAppsViolation](../api/restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Update the properties of a [restrictedAppsViolation](../resources/restrictedappsviolation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceConfigurationId|String||
|deviceConfigurationName|String||
|deviceName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceId|String||
|platformType|Enumeration| Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|restrictedApps|[managedDeviceReportedApp](../resources/manageddevicereportedapp.md) collection||
|restrictedAppsState|Enumeration| Possible values are: `prohibitedApps`, `notApprovedApps`.|
|userId|String||
|userName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp"
    }
  ]
}
```

