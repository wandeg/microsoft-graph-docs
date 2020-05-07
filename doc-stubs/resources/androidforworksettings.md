---
title: "androidForWorkSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidForWorkSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[requestSignupUrl](../api/androidforworksettings-requestsignupurl.md)|String|**TODO: Add Description**|
|[completeSignup](../api/androidforworksettings-completesignup.md)|None|**TODO: Add Description**|
|[syncApps](../api/androidforworksettings-syncapps.md)|None|**TODO: Add Description**|
|[unbind](../api/androidforworksettings-unbind.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bindStatus|androidForWorkBindStatus|**TODO: Add Description**. Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|deviceOwnerManagementEnabled|Boolean|**TODO: Add Description**|
|enrollmentTarget|androidForWorkEnrollmentTarget|**TODO: Add Description**. Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastAppSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|lastAppSyncStatus|androidForWorkSyncStatus|**TODO: Add Description**. Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|ownerOrganizationName|String|**TODO: Add Description**|
|ownerUserPrincipalName|String|**TODO: Add Description**|
|targetGroupIds|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "deviceOwnerManagementEnabled": "Boolean"
}
```

