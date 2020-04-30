---
title: "homeRealmDiscoveryPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# homeRealmDiscoveryPolicy resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get homeRealmDiscoveryPolicy](../api/microsoft.directoryservices-homerealmdiscoverypolicy-get.md)|[homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md)|Read properties and relationships of a [homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md) object.|
|[Update homeRealmDiscoveryPolicy](../api/microsoft.directoryservices-homerealmdiscoverypolicy-update.md)|[homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md)|Update the properties of a [homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md) object.|
|[List appliesTo](../api/microsoft.directoryservices-homerealmdiscoverypolicy-list-appliesto.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/microsoft.directoryservices-homerealmdiscoverypolicy-post-appliesto.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add appliesTo by posting to the appliesTo collection.|
|[Remove appliesTo](../api/microsoft.directoryservices-homerealmdiscoverypolicy-delete-appliesto.md)|None|Remove an appliesTo object.|

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
  "@odata.type": "Microsoft.DirectoryServices.homeRealmDiscoveryPolicy",
  "baseType": "Microsoft.DirectoryServices.stsPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.homeRealmDiscoveryPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

