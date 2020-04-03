---
title: "Add deviceManagementPartners"
description: "Add deviceManagementPartners by posting to the deviceManagementPartners collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceManagementPartners

Namespace: microsoft.graph

Add deviceManagementPartners by posting to the deviceManagementPartners collection.

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
POST /deviceManagement/deviceManagementPartners/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/devicemanagementpartner.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementpartner_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 889

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:00.975564+00:00",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2016-12-31T23:56:25.9411206+00:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2016-12-31T23:59:04.2027222+00:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:27.0396085+00:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:11.6794127+00:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementpartner"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 938

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "68650f79-0f79-6865-790f-6568790f6568",
  "lastHeartbeatDateTime": "2016-12-31T23:59:00.975564+00:00",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2016-12-31T23:56:25.9411206+00:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2016-12-31T23:59:04.2027222+00:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:27.0396085+00:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:11.6794127+00:00",
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

