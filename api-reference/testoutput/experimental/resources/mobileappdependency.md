---
title: "mobileAppDependency resource type"
description: "Describes a dependency type between two mobile apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppDependency resource type


Namespace: microsoft.graph

Describes a dependency type between two mobile apps.


Inherits from [mobileAppRelationship](../resources/mobileapprelationship.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileAppDependencies](../api/mobileappdependency-list.md)|[mobileAppDependency](../resources/mobileappdependency.md) collection|List properties and relationships of the [mobileAppDependency](../resources/mobileappdependency.md) objects.|
|[Get mobileAppDependency](../api/mobileappdependency-get.md)|[mobileAppDependency](../resources/mobileappdependency.md)|Read properties and relationships of the [mobileAppDependency](../resources/mobileappdependency.md) object.|
|[Create mobileAppDependency](../api/mobileappdependency-create.md)|[mobileAppDependency](../resources/mobileappdependency.md)|Create a new [mobileAppDependency](../resources/mobileappdependency.md) object.|
|[Delete mobileAppDependency](../api/mobileappdependency-delete.md)|None|Deletes a [mobileAppDependency](../resources/mobileappdependency.md).|
|[Update mobileAppDependency](../api/mobileappdependency-update.md)|[mobileAppDependency](../resources/mobileappdependency.md)|Update the properties of a [mobileAppDependency](../resources/mobileappdependency.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dependencyType|Enumeration|The type of dependency relationship between the parent and child apps. Possible values are: `detect`, `autoInstall`.|
|dependentAppCount|Int32|The total number of dependencies the child app has.|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetDisplayName|String|The target child mobile app's display name. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency",
  "baseType": "microsoft.graph.mobileAppRelationship",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```

