---
title: "androidForWorkSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidForWorkSettings resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidForWorkSettings](../api/androidforworksettings-get.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Read properties and relationships of the [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[Update androidForWorkSettings](../api/androidforworksettings-update.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Update the properties of a [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[requestSignupUrl](../api/androidforworksettings-requestsignupurl.md)|String||
|[completeSignup](../api/androidforworksettings-completesignup.md)|None||
|[syncApps](../api/androidforworksettings-syncapps.md)|None||
|[unbind](../api/androidforworksettings-unbind.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bindStatus|Enumeration| Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|deviceOwnerManagementEnabled|Boolean||
|enrollmentTarget|Enumeration| Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastAppSyncDateTime|DateTimeOffset||
|lastAppSyncStatus|Enumeration| Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|lastModifiedDateTime|DateTimeOffset||
|ownerOrganizationName|String||
|ownerUserPrincipalName|String||
|targetGroupIds|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true
}
```

