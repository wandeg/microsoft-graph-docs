---
title: "iosVppAppAssignedUserLicense resource type"
description: "iOS Volume Purchase Program user license assignment. This class does not support Create, Delete, or Update."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosVppAppAssignedUserLicense resource type


Namespace: microsoft.graph

iOS Volume Purchase Program user license assignment. This class does not support Create, Delete, or Update.


Inherits from [iosVppAppAssignedLicense](../resources/iosvppappassignedlicense.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosVppAppAssignedUserLicenses](../api/iosvppappassigneduserlicense-list.md)|[iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) collection|List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) objects.|
|[Get iosVppAppAssignedUserLicense](../api/iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md)|Read properties and relationships of the [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) object.|
|[Create iosVppAppAssignedUserLicense](../api/iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md)|Create a new [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) object.|
|[Delete iosVppAppAssignedUserLicense](../api/iosvppappassigneduserlicense-delete.md)|None|Deletes a [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md).|
|[Update iosVppAppAssignedUserLicense](../api/iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md)|Update the properties of a [iosVppAppAssignedUserLicense](../resources/iosvppappassigneduserlicense.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userEmailAddress|String|The user email address. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|The user ID. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|The user name. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|The user principal name. Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|

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

