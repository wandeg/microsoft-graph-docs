---
title: "claimsMappingPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# claimsMappingPolicy resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get claimsMappingPolicy](../api/microsoft.directoryservices-claimsmappingpolicy-get.md)|[claimsMappingPolicy](../resources/microsoft.directoryservices-claimsmappingpolicy.md)|Read properties and relationships of a [claimsMappingPolicy](../resources/microsoft.directoryservices-claimsmappingpolicy.md) object.|
|[Update claimsMappingPolicy](../api/microsoft.directoryservices-claimsmappingpolicy-update.md)|[claimsMappingPolicy](../resources/microsoft.directoryservices-claimsmappingpolicy.md)|Update the properties of a [claimsMappingPolicy](../resources/microsoft.directoryservices-claimsmappingpolicy.md) object.|
|[List appliesTo](../api/microsoft.directoryservices-claimsmappingpolicy-list-appliesto.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/microsoft.directoryservices-claimsmappingpolicy-post-appliesto.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add appliesTo by posting to the appliesTo collection.|
|[Remove appliesTo](../api/microsoft.directoryservices-claimsmappingpolicy-delete-appliesto.md)|None|Remove an appliesTo object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/microsoft.directoryservices-stspolicy.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|id|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/microsoft.directoryservices-stspolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.claimsMappingPolicy",
  "baseType": "Microsoft.DirectoryServices.stsPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.claimsMappingPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

