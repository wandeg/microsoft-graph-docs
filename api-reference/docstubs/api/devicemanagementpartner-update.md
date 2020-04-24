---
title: "Update deviceManagementPartner"
description: "Update the properties of a deviceManagementPartner object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceManagementPartner

Namespace: microsoft.graph

Update the properties of a [deviceManagementPartner](../resources/devicemanagementpartner.md) object.

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
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementPartner](../resources/devicemanagementpartner.md) object.

The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/devicemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastHeartbeatDateTime|DateTimeOffset|Timestamp of last heartbeat after admin enabled option Connect to Device management Partner|
|partnerState|deviceManagementPartnerTenantState|Partner state of this tenant. Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|deviceManagementPartnerAppType|Partner App type. Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|String|Partner Single tenant App id|
|displayName|String|Partner display name|
|isConfigured|Boolean|Whether device management partner is configured or not|
|whenPartnerDevicesWillBeRemoved|DateTimeOffset|DateTime in UTC when PartnerDevices will be removed. This will become obselete soon.|
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset|DateTime in UTC when PartnerDevices will be marked as NonCompliant. This will become obselete soon.|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|DateTime in UTC when PartnerDevices will be removed|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|DateTime in UTC when PartnerDevices will be marked as NonCompliant|
|groupsRequiringPartnerEnrollment|[deviceManagementPartnerAssignment](../resources/devicemanagementpartnerassignment.md) collection|User groups that specifies whether enrollment is through partner.|



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
Content-Type: application/json
Content-length: 890

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2017-01-01T00:02:45.9937149+03:00",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:02:45.3822258+03:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2016-12-31T23:58:36.3953817+03:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2017-01-01T00:00:12.4112773+03:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2017-01-01T00:00:05.4461028+03:00",
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
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "59385f60-5f60-5938-605f-3859605f3859",
  "lastHeartbeatDateTime": "2017-01-01T00:02:45.9937149+03:00",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:02:45.3822258+03:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2016-12-31T23:58:36.3953817+03:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2017-01-01T00:00:12.4112773+03:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2017-01-01T00:00:05.4461028+03:00",
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

