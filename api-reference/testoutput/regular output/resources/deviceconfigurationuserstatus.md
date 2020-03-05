---
title: "deviceConfigurationUserStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationUserStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceConfigurationUserStatuses](../api/deviceconfigurationuserstatus-list.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|List properties and relationships of the [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) objects.|
|[Get deviceConfigurationUserStatus](../api/deviceconfigurationuserstatus-get.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Read properties and relationships of the [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) object.|
|[Create deviceConfigurationUserStatus](../api/deviceconfigurationuserstatus-create.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Create a new [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) object.|
|[Delete deviceConfigurationUserStatus](../api/deviceconfigurationuserstatus-delete.md)|None|Deletes a [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md).|
|[Update deviceConfigurationUserStatus](../api/deviceconfigurationuserstatus-update.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Update the properties of a [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|devicesCount|Int32|Devices count for that user.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userDisplayName|String|User name of the DevicePolicyStatus.|
|userPrincipalName|String|UserPrincipalName.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```

