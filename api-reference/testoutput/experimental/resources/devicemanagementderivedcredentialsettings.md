---
title: "deviceManagementDerivedCredentialSettings resource type"
description: "Entity that describes tenant level settings for derived credentials"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementDerivedCredentialSettings resource type


Namespace: microsoft.graph

Entity that describes tenant level settings for derived credentials


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementDerivedCredentialSettingses](../api/devicemanagementderivedcredentialsettings-list.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) collection|List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) objects.|
|[Get deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|
|[Create deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-create.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Create a new [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|
|[Delete deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-delete.md)|None|Deletes a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md).|
|[Update deviceManagementDerivedCredentialSettings](../api/devicemanagementderivedcredentialsettings-update.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.|
|[List derivedCredentials](../api/intune-devices-devicemanagement-list-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) collection|Get the deviceManagementDerivedCredentialSettingses from the derivedCredentials navigation property.|
|[Add derivedCredentials](../api/intune-devices-devicemanagement-post-derivedcredentials.md)|[deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md)|Add derivedCredentials by posting to the derivedCredentials collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The display name for the profile.|
|helpUrl|String|The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.|
|id|String| Inherited from [entity](../resources/entity.md)|
|issuer|Enumeration|The derived credential provider to use. Possible values are: `intercede`, `entrustDatacard`, `purebred`.|
|notificationType|Enumeration|The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device. Possible values are: `none`, `companyPortal`, `email`.|

## Relationships
None

## JSON Representation
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

