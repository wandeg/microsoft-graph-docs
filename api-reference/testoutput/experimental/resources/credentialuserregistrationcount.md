---
title: "credentialUserRegistrationCount resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# credentialUserRegistrationCount resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List credentialUserRegistrationCounts](../api/credentialuserregistrationcount-list.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection|List properties and relationships of the [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) objects.|
|[Get credentialUserRegistrationCount](../api/credentialuserregistrationcount-get.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md)|Read properties and relationships of the [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) object.|
|[Create credentialUserRegistrationCount](../api/credentialuserregistrationcount-create.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md)|Create a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) object.|
|[Delete credentialUserRegistrationCount](../api/credentialuserregistrationcount-delete.md)|None|Deletes a [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md).|
|[Update credentialUserRegistrationCount](../api/credentialuserregistrationcount-update.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md)|Update the properties of a [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|totalUserCount|Int64||
|userRegistrationCounts|[userRegistrationCount](../resources/userregistrationcount.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationCount",
  "id": "String (identifier)",
  "totalUserCount": 1024,
  "userRegistrationCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationCount"
    }
  ]
}
```

