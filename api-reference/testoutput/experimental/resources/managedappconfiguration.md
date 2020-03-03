---
title: "managedAppConfiguration resource type"
description: "Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppConfiguration resource type


Namespace: microsoft.graph

Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped


Inherits from [managedAppPolicy](../resources/managedapppolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAppConfigurations](../api/managedappconfiguration-list.md)|[managedAppConfiguration](../resources/managedappconfiguration.md) collection|List properties and relationships of the [managedAppConfiguration](../resources/managedappconfiguration.md) objects.|
|[Get managedAppConfiguration](../api/managedappconfiguration-get.md)|[managedAppConfiguration](../resources/managedappconfiguration.md)|Read properties and relationships of the [managedAppConfiguration](../resources/managedappconfiguration.md) object.|
|[targetApps](../api/managedappconfiguration-targetapps.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the policy was created. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service|
|description|String|The policy's description. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|displayName|String|Policy display name. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String|Version of the entity. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration",
  "baseType": "microsoft.graph.managedAppPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```

