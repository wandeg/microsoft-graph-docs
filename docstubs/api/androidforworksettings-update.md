---
title: "Update androidForWorkSettings"
description: "Update the properties of a androidForWorkSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update androidForWorkSettings

Namespace: microsoft.graph

Update the properties of a [androidForWorkSettings](../resources/androidforworksettings.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/androidforworksettings.md) object.

The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/androidforworksettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|bindStatus|Enumeration| Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset||
|lastAppSyncStatus|Enumeration| Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String||
|ownerOrganizationName|String||
|lastModifiedDateTime|DateTimeOffset||
|enrollmentTarget|Enumeration| Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|String collection||
|deviceOwnerManagementEnabled|Boolean||



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
Content-type: application/json
Content-length: 446

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "String",
  "lastAppSyncDateTime": "2016-12-31T23:58:25.8481316+00:00",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "d46a3086-3086-d46a-8630-6ad486306ad4",
  "bindStatus": "String",
  "lastAppSyncDateTime": "2016-12-31T23:58:25.8481316+00:00",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

