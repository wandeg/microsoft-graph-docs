---
title: "deviceManagementDerivedCredentialSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementDerivedCredentialSettings resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|
|[Update deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-update.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|helpUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|issuer|Enumeration| Possible values are: `intercede`, `entrustDatacard`, `purebred`, `xTec`.|
|notificationType|Enumeration| Possible values are: `none`, `companyPortal`, `email`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```

