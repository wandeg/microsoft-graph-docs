---
title: "Create androidForWorkSettings"
description: "Create a new androidForWorkSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create androidForWorkSettings

Namespace: microsoft.graph

Create a new androidForWorkSettings object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [androidForWorkSettings](../resources/androidforworksettings.md) object.

The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/androidforworksettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|bindStatus|androidForWorkBindStatus|**TODO: Add Description**. Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|lastAppSyncStatus|androidForWorkSyncStatus|**TODO: Add Description**. Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|**TODO: Add Description**|
|ownerOrganizationName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|enrollmentTarget|androidForWorkEnrollmentTarget|**TODO: Add Description**. Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|String collection|**TODO: Add Description**|
|deviceOwnerManagementEnabled|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [androidForWorkSettings](../resources/androidforworksettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_androidforworksettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-Type: application/json
Content-length: 372

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidforworksettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "40145a05-5a05-4014-055a-1440055a1440",
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

