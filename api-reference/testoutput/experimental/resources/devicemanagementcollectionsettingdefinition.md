---
title: "deviceManagementCollectionSettingDefinition resource type"
description: "Entity representing the defintion for a collection setting"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementCollectionSettingDefinition resource type


Namespace: microsoft.graph

Entity representing the defintion for a collection setting


Inherits from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementCollectionSettingDefinitions](../api/devicemanagementcollectionsettingdefinition-list.md)|[deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md) collection|List properties and relationships of the [deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md) objects.|
|[Get deviceManagementCollectionSettingDefinition](../api/devicemanagementcollectionsettingdefinition-get.md)|[deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md)|Read properties and relationships of the [deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md) object.|
|[Create deviceManagementCollectionSettingDefinition](../api/devicemanagementcollectionsettingdefinition-create.md)|[deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md)|Create a new [deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md) object.|
|[Delete deviceManagementCollectionSettingDefinition](../api/devicemanagementcollectionsettingdefinition-delete.md)|None|Deletes a [deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md).|
|[Update deviceManagementCollectionSettingDefinition](../api/devicemanagementcollectionsettingdefinition-update.md)|[deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md)|Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/devicemanagementcollectionsettingdefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|constraints|[deviceManagementConstraint](../resources/devicemanagementconstraint.md) collection|Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|dependencies|[deviceManagementSettingDependency](../resources/devicemanagementsettingdependency.md) collection|Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|description|String|The setting's description Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|displayName|String|The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|documentationUrl|String|Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|elementDefinitionId|String|The Setting Definition ID that describes what each element of the collection looks like|
|id|String| Inherited from [entity](../resources/entity.md)|
|isTopLevel|Boolean|If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|keywords|String collection|Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|valueType|Enumeration|The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md). Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingDefinition",
  "baseType": "microsoft.graph.deviceManagementSettingDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
    }
  ],
  "elementDefinitionId": "String"
}
```

