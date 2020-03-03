---
title: "deviceManagementUserRightsSetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementUserRightsSetting resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|localUsersOrGroups|[deviceManagementUserRightsLocalUserOrGroup](../resources/deviceManagementUserRightsLocalUserOrGroup.md) collection|Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed. This collection can contain a maximum of 500 elements.|
|state|Enumeration|Representing the current state of this user rights setting. Possible values are: `notConfigured`, `blocked`, `allowed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```

