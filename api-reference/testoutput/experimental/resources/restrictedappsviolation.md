---
title: "restrictedAppsViolation resource type"
description: "Violation of restricted apps configuration profile per device per user"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# restrictedAppsViolation resource type


Namespace: microsoft.graph

Violation of restricted apps configuration profile per device per user


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List restrictedAppsViolations](../api/restrictedappsviolation-list.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md) collection|List properties and relationships of the [restrictedAppsViolation](../resources/restrictedappsviolation.md) objects.|
|[Get restrictedAppsViolation](../api/restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Read properties and relationships of the [restrictedAppsViolation](../resources/restrictedappsviolation.md) object.|
|[Create restrictedAppsViolation](../api/restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Create a new [restrictedAppsViolation](../resources/restrictedappsviolation.md) object.|
|[Delete restrictedAppsViolation](../api/restrictedappsviolation-delete.md)|None|Deletes a [restrictedAppsViolation](../resources/restrictedappsviolation.md).|
|[Update restrictedAppsViolation](../api/restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Update the properties of a [restrictedAppsViolation](../resources/restrictedappsviolation.md) object.|
|[List deviceConfigurationRestrictedAppsViolations](../api/intune-devices-devicemanagement-list-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md) collection|Get the restrictedAppsViolations from the deviceConfigurationRestrictedAppsViolations navigation property.|
|[Add deviceConfigurationRestrictedAppsViolations](../api/intune-devices-devicemanagement-post-deviceconfigurationrestrictedappsviolations.md)|[restrictedAppsViolation](../resources/restrictedappsviolation.md)|Add deviceConfigurationRestrictedAppsViolations by posting to the deviceConfigurationRestrictedAppsViolations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceConfigurationId|String|Device configuration profile unique identifier, must be Guid|
|deviceConfigurationName|String|Device configuration profile name|
|deviceName|String|Device name|
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceId|String|Managed device unique identifier, must be Guid|
|platformType|Enumeration|Platform type. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|restrictedApps|[managedDeviceReportedApp](../resources/manageddevicereportedapp.md) collection|List of violated restricted apps|
|restrictedAppsState|Enumeration|Restricted apps state. Possible values are: `prohibitedApps`, `notApprovedApps`.|
|userId|String|User unique identifier, must be Guid|
|userName|String|User name|

## Relationships
None

## JSON Representation
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

