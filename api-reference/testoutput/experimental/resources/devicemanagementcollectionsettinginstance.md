---
title: "deviceManagementCollectionSettingInstance resource type"
description: "A setting instance representing a collection of values"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementCollectionSettingInstance resource type

A setting instance representing a collection of values


Inherits from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementCollectionSettingInstances](../api/devicemanagementcollectionsettinginstance-list.md)|[deviceManagementCollectionSettingInstance](../resources/deviceManagementCollectionSettingInstance.md) collection|List properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/devicemanagementcollectionsettinginstance.md) objects.|
|[Get deviceManagementCollectionSettingInstance](../api/devicemanagementcollectionsettinginstance-get.md)|[deviceManagementCollectionSettingInstance](../resources/deviceManagementCollectionSettingInstance.md)|Read properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/devicemanagementcollectionsettinginstance.md) object.|
|[Create deviceManagementCollectionSettingInstance](../api/devicemanagementcollectionsettinginstance-create.md)|[deviceManagementCollectionSettingInstance](../resources/deviceManagementCollectionSettingInstance.md)|Create a new [deviceManagementCollectionSettingInstance](../resources/devicemanagementcollectionsettinginstance.md) object.|
|[Delete deviceManagementCollectionSettingInstance](../api/devicemanagementcollectionsettinginstance-delete.md)|None|Deletes a [deviceManagementCollectionSettingInstance](../resources/devicemanagementcollectionsettinginstance.md).|
|[Update deviceManagementCollectionSettingInstance](../api/devicemanagementcollectionsettinginstance-update.md)|[deviceManagementCollectionSettingInstance](../resources/deviceManagementCollectionSettingInstance.md)|Update the properties of a [deviceManagementCollectionSettingInstance](../resources/devicemanagementcollectionsettinginstance.md) object.|
|[List value](../api/devicemanagementcollectionsettinginstance-list-value.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|Get the deviceManagementSettingInstances from the value navigation property.|
|[Create value](../api/devicemanagementcollectionsettinginstance-post-value.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|Create value by posting to the value collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definitionId|String|The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|valueJson|String|JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|value|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|The collection of values|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingInstance",
  "baseType": "microsoft.graph.deviceManagementSettingInstance",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```

