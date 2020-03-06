---
title: "deviceManagementIntentUserState resource type"
description: "Entity that represents user state for an intent"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementIntentUserState resource type


Namespace: microsoft.graph

Entity that represents user state for an intent


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentUserState](../api/devicemanagementintentuserstate-get.md)|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md)|Read properties and relationships of the [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object.|
|[Update deviceManagementIntentUserState](../api/devicemanagementintentuserstate-update.md)|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md)|Update the properties of a [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object.|
|[List userStates](../api/devicemanagementintent-list-userstates.md)|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) collection|Get the deviceManagementIntentUserStates from the userStates navigation property.|
|[Add userStates](../api/devicemanagementintent-post-userstates.md)|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md)|Add userStates by posting to the userStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceCount|Int32|Count of Devices that belongs to a user for an intent|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset|Last modified date time of an intent report|
|state|Enumeration|User state for an intent. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userName|String|The user name that is being reported on a device|
|userPrincipalName|String|The user principal name that is being reported on a device|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": 1024,
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```

