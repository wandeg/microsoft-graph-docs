---
title: "accessPackageResourceRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageResourceRequest resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) collection|List properties and relationships of the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.|
|[Get accessPackageResourceRequest](../api/accesspackageresourcerequest-get.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Read properties and relationships of the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.|
|[Create accessPackageResourceRequest](../api/accesspackageresourcerequest-post-accesspackageresourcerequests.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.|
|[Delete accessPackageResourceRequest](../api/accesspackageresourcerequest-delete.md)|None|Deletes a [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md).|
|[Update accessPackageResourceRequest](../api/accesspackageresourcerequest-update.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Update the properties of a [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accesspackageresource.md)|Read properties and relationships of the [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|catalogId|String||
|executeImmediately|Boolean||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|isValidationOnly|Boolean||
|justification|String||
|requestState|String||
|requestStatus|String||
|requestType|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResource|[accessPackageResource](../resources/accesspackageresource.md)||
|requestor|[accessPackageSubject](../resources/accesspackagesubject.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
  "id": "String (identifier)",
  "catalogId": "String",
  "executeImmediately": true,
  "isValidationOnly": true,
  "requestType": "String",
  "requestState": "String",
  "requestStatus": "String",
  "justification": "String",
  "expirationDateTime": "String (timestamp)"
}
```

