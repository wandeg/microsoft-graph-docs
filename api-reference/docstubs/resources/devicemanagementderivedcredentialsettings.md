---
title: "deviceManagementDerivedCredentialSettings resource type"
description: "Entity that describes tenant level settings for derived credentials"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementDerivedCredentialSettings resource type


Namespace: microsoft.graph

Entity that describes tenant level settings for derived credentials


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Read the properties and relationships of a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|
|[Update deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-update.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The display name for the profile.|
|helpUrl|String|The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|issuer|deviceManagementDerivedCredentialIssuer|The derived credential provider to use. Possible values are: `intercede`, `entrustDatacard`, `purebred`, `xTec`.|
|notificationType|deviceManagementDerivedCredentialNotificationType|The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device. Possible values are: `none`, `companyPortal`, `email`.|

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

