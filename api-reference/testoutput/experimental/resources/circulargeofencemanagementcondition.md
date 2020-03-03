---
title: "circularGeofenceManagementCondition resource type"
description: "Contains the information to define a circular geo-fence management condition, an area of interest, to monitor."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# circularGeofenceManagementCondition resource type

Contains the information to define a circular geo-fence management condition, an area of interest, to monitor.


Inherits from [locationManagementCondition](../resources/locationManagementCondition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List circularGeofenceManagementConditions](../api/circulargeofencemanagementcondition-list.md)|[circularGeofenceManagementCondition](../resources/circularGeofenceManagementCondition.md) collection|List properties and relationships of the [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md) objects.|
|[Get circularGeofenceManagementCondition](../api/circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/circularGeofenceManagementCondition.md)|Read properties and relationships of the [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md) object.|
|[Create circularGeofenceManagementCondition](../api/circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/circularGeofenceManagementCondition.md)|Create a new [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md) object.|
|[Delete circularGeofenceManagementCondition](../api/circulargeofencemanagementcondition-delete.md)|None|Deletes a [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md).|
|[Update circularGeofenceManagementCondition](../api/circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/circularGeofenceManagementCondition.md)|Update the properties of a [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md) object.|
|[List managementConditionStatements](../api/circulargeofencemanagementcondition-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementConditionStatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Create managementConditionStatements](../api/circulargeofencemanagementcondition-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementConditionStatement.md)|Create managementConditionStatements by posting to the managementConditionStatements collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|description|String|The admin defined description of the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|displayName|String|The admin defined name of the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|eTag|String|ETag of the management condition. Updated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|latitude|Double|Latitude in degrees, between -90 and +90 inclusive.|
|longitude|Double|Longitude in degrees, between -180 and +180 inclusive.|
|modifiedDateTime|DateTimeOffset|The time the management condition was last modified. Updated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|radiusInMeters|Single|Radius in meters.|
|uniqueName|String|Unique name for the management condition. Used in management condition expressions. Inherited from [managementCondition](../resources/managementCondition.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/managementConditionStatement.md) collection|The management condition statements associated to the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.circularGeofenceManagementCondition",
  "baseType": "microsoft.graph.locationManagementCondition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "latitude": "Double",
  "longitude": "Double",
  "radiusInMeters": "Single"
}
```

