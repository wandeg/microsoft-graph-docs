---
title: "accessPackageSubject resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageSubject resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageSubjects](../api/accesspackagesubject-list.md)|[accessPackageSubject](../resources/accesspackagesubject.md) collection|List properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) objects.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Create accessPackageSubject](../api/accesspackagesubject-create.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Create a new [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Delete accessPackageSubject](../api/accesspackagesubject-delete.md)|None|Deletes a [accessPackageSubject](../resources/accesspackagesubject.md).|
|[Update accessPackageSubject](../api/accesspackagesubject-update.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Update the properties of a [accessPackageSubject](../resources/accesspackagesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|altSecId|String||
|displayName|String||
|email|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|objectId|String||
|onPremisesSecurityIdentifier|String||
|principalName|String||
|type|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "String (identifier)",
  "objectId": "String",
  "altSecId": "String",
  "displayName": "String",
  "principalName": "String",
  "email": "String",
  "onPremisesSecurityIdentifier": "String",
  "type": "String"
}
```

