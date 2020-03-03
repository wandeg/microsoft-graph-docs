---
title: "iosVppAppAssignedUserLicense resource type"
description: "iOS Volume Purchase Program user license assignment. This class does not support Create, Delete, or Update."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosVppAppAssignedUserLicense resource type

iOS Volume Purchase Program user license assignment. This class does not support Create, Delete, or Update.


Inherits from [iosVppAppAssignedLicense](../resources/iosVppAppAssignedLicense.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosVppAppAssignedUserLicenses](../api/iosvppappassigneduserlicense-list.md)|[iosVppAppAssignedUserLicense](../resources/iosVppAppAssignedUserLicense.md) collection|List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) objects.|
|[Get iosVppAppAssignedUserLicense](../api/iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/iosVppAppAssignedUserLicense.md)|Read properties and relationships of the [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) object.|
|[Create iosVppAppAssignedUserLicense](../api/iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/iosVppAppAssignedUserLicense.md)|Create a new [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) object.|
|[Delete iosVppAppAssignedUserLicense](../api/iosvppappassigneduserlicense-delete.md)|None|Deletes a [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md).|
|[Update iosVppAppAssignedUserLicense](../api/iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/iosVppAppAssignedUserLicense.md)|Update the properties of a [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userEmailAddress|String|The user email address. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|
|userId|String|The user ID. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|
|userName|String|The user name. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|
|userPrincipalName|String|The user principal name. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedUserLicense",
  "baseType": "microsoft.graph.iosVppAppAssignedLicense",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```

