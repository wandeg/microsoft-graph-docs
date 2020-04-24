---
title: "Update androidForWorkSettings"
description: "Update the properties of an androidForWorkSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update androidForWorkSettings

Namespace: microsoft.graph

Update the properties of an androidForWorkSettings object.

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
PATCH /deviceManagement/androidForWorkSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [androidForWorkSettings](../resources/androidforworksettings.md) object.

The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/androidforworksettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|bindStatus|androidForWorkBindStatus|Bind status of the tenant with the Google EMM API. Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Last completion time for app sync|
|lastAppSyncStatus|androidForWorkSyncStatus|Last application sync result. Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|Owner UPN that created the enterprise|
|ownerOrganizationName|String|Organization name used when onboarding Android for Work|
|lastModifiedDateTime|DateTimeOffset|Last modification time for Android for Work settings|
|enrollmentTarget|androidForWorkEnrollmentTarget|Indicates which users can enroll devices in Android for Work device management. Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|String collection|Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'|
|deviceOwnerManagementEnabled|Boolean|Indicates if this account is flighting for Android Device Owner Management with CloudDPC.|



## Response
If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/androidforworksettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_androidforworksettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-Type: application/json
Content-length: 446

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "String",
  "lastAppSyncDateTime": "2016-12-31T23:57:01.9362672+03:00",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "b6ff2a0a-2a0a-b6ff-0a2a-ffb60a2affb6",
  "bindStatus": "String",
  "lastAppSyncDateTime": "2016-12-31T23:57:01.9362672+03:00",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

