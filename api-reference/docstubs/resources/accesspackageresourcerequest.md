---
title: "accessPackageResourceRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageResourceRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) collection|Get a list of the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects and their properties.|
|[Get accessPackageResourceRequest](../api/accesspackageresourcerequest-get.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Read the properties and relationships of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.|
|[Create accessPackageResourceRequest](../api/accesspackageresourcerequest-post-accesspackageresourcerequests.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.|
|[Delete accessPackageResourceRequest](../api/accesspackageresourcerequest-delete.md)|None|Deletes an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.|
|[Update accessPackageResourceRequest](../api/accesspackageresourcerequest-update.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Update the properties of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.|
|[List accessPackageResource](../api/accesspackageresourcerequest-list-accesspackageresource.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|Get the accessPackageResources from the accessPackageResource navigation property.|
|[Add accessPackageResource](../api/accesspackageresourcerequest-post-accesspackageresource.md)|[accessPackageResource](../resources/accesspackageresource.md)|Add accessPackageResource by posting to the accessPackageResource collection.|
|[Remove accessPackageResource](../api/accesspackageresourcerequest-delete-accesspackageresource.md)|None|Remove an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[List requestor](../api/accesspackageresourcerequest-list-requestor.md)|[accessPackageSubject](../resources/accesspackagesubject.md) collection|Get the accessPackageSubjects from the requestor navigation property.|
|[Create requestor](../api/accesspackageresourcerequest-post-requestor.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Create a new requestor object.|
|[Delete requestor](../api/accesspackageresourcerequest-delete-requestor.md)|None|Delete a [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Update requestor](../api/accesspackageresourcerequest-update-requestor.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Update the properties of a requestor object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read the properties and relationships of an [accessPackageSubject](../resources/accesspackagesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|catalogId|String|**TODO: Add Description**|
|executeImmediately|Boolean|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isValidationOnly|Boolean|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|
|requestState|String|**TODO: Add Description**|
|requestStatus|String|**TODO: Add Description**|
|requestType|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResource|[accessPackageResource](../resources/accesspackageresource.md)|**TODO: Add Description**|
|requestor|[accessPackageSubject](../resources/accesspackagesubject.md)|**TODO: Add Description**|

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
  "expirationDateTime": "String (timestamp)",
  "justification": "String"
}
```

