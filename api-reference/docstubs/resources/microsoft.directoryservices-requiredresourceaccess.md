---
title: "requiredResourceAccess resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# requiredResourceAccess resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|resourceAccess|[resourceAccess](../resources/microsoft.directoryservices-resourceaccess.md) collection|**TODO: Add Description**|
|resourceAppId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.requiredResourceAccess"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.requiredResourceAccess",
  "resourceAppId": "String",
  "resourceAccess": [
    {
      "@odata.type": "Microsoft.DirectoryServices.resourceAccess",
      "id": "Guid",
      "type": "String"
    }
  ]
}
```

