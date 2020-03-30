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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_androidforworksettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "String",
  "lastAppSyncDateTime": "2016-12-31T23:58:53.908903+00:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "dc99cf40-cf40-dc99-40cf-99dc40cf99dc",
  "bindStatus": "String",
  "lastAppSyncDateTime": "2016-12-31T23:58:53.908903+00:00",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

