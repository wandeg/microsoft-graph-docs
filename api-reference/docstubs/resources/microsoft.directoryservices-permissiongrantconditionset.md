---
title: "permissionGrantConditionSet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# permissionGrantConditionSet resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|permissionClassification|String|**TODO: Add Description**|
|permissions|[permissionConditionSet](../resources/microsoft.directoryservices-permissionconditionset.md)|**TODO: Add Description**|
|permissionType|permissionType|**TODO: Add Description**. Possible values are: `application`, `delegated`, `delegatedUserConsentable`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.permissionGrantConditionSet"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.permissionGrantConditionSet",
  "permissionClassification": "String",
  "permissionType": "String",
  "permissions": {
    "@odata.type": "Microsoft.DirectoryServices.permissionConditionSet",
    "resourceApplication": "String",
    "includeAllPermissions": true,
    "includeSpecificPermissions": [
      "String"
    ]
  }
}
```

