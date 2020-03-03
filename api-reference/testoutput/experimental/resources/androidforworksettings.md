---
title: "androidForWorkSettings resource type"
description: "Settings for Android For Work."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidForWorkSettings resource type


Namespace: microsoft.graph

Settings for Android For Work.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidForWorkSettingses](../api/androidforworksettings-list.md)|[androidForWorkSettings](../resources/androidforworksettings.md) collection|List properties and relationships of the [androidForWorkSettings](../resources/androidforworksettings.md) objects.|
|[Get androidForWorkSettings](../api/androidforworksettings-get.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Read properties and relationships of the [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[Create androidForWorkSettings](../api/androidforworksettings-create.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Create a new [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[Delete androidForWorkSettings](../api/androidforworksettings-delete.md)|None|Deletes a [androidForWorkSettings](../resources/androidforworksettings.md).|
|[Update androidForWorkSettings](../api/androidforworksettings-update.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Update the properties of a [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[requestSignupUrl](../api/androidforworksettings-requestsignupurl.md)|String||
|[completeSignup](../api/androidforworksettings-completesignup.md)|None||
|[syncApps](../api/androidforworksettings-syncapps.md)|None||
|[unbind](../api/androidforworksettings-unbind.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bindStatus|Enumeration|Bind status of the tenant with the Google EMM API. Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|deviceOwnerManagementEnabled|Boolean|Indicates if this account is flighting for Android Device Owner Management with CloudDPC.|
|enrollmentTarget|Enumeration|Indicates which users can enroll devices in Android for Work device management. Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastAppSyncDateTime|DateTimeOffset|Last completion time for app sync|
|lastAppSyncStatus|Enumeration|Last application sync result. Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|lastModifiedDateTime|DateTimeOffset|Last modification time for Android for Work settings|
|ownerOrganizationName|String|Organization name used when onboarding Android for Work|
|ownerUserPrincipalName|String|Owner UPN that created the enterprise|
|targetGroupIds|String collection|Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'|

## Relationships
None

## JSON Representation
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

