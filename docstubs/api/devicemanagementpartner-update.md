---
title: "Update deviceManagementPartner"
description: "Update the properties of a deviceManagementPartner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementPartner

Namespace: microsoft.graph

Update the properties of a [deviceManagementPartner](../resources/devicemanagementpartner.md) object.

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
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/devicemanagementpartner.md) object.

The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/devicemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastHeartbeatDateTime|DateTimeOffset||
|partnerState|Enumeration| Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|Enumeration| Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|String||
|displayName|String||
|isConfigured|Boolean||
|whenPartnerDevicesWillBeRemoved|DateTimeOffset||
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset||
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset||
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset||
|groupsRequiringPartnerEnrollment|[deviceManagementPartnerAssignment](../resources/devicemanagementpartnerassignment.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/devicemanagementpartner.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementpartner"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 890

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:57:13.0947485+00:00",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2016-12-31T23:59:57.9616608+00:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2016-12-31T23:56:28.7845609+00:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:57:07.2946764+00:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2017-01-01T00:02:15.1018941+00:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      }
    }
  ]
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
Content-Length: 939

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "c71cc27a-c27a-c71c-7ac2-1cc77ac21cc7",
  "lastHeartbeatDateTime": "2016-12-31T23:57:13.0947485+00:00",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2016-12-31T23:59:57.9616608+00:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2016-12-31T23:56:28.7845609+00:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:57:07.2946764+00:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2017-01-01T00:02:15.1018941+00:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      }
    }
  ]
}
```

