---
title: "Create deviceManagementPartner"
description: "Create a new deviceManagementPartner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create deviceManagementPartner

Namespace: microsoft.graph

Create a new [deviceManagementPartner](../resources/devicemanagementpartner.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/devicemanagementpartner.md) object.

The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/devicemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastHeartbeatDateTime|DateTimeOffset|Timestamp of last heartbeat after admin enabled option Connect to Device management Partner|
|partnerState|Enumeration|Partner state of this tenant. Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|Enumeration|Partner App type. Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|String|Partner Single tenant App id|
|displayName|String|Partner display name|
|isConfigured|Boolean|Whether device management partner is configured or not|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|DateTime in UTC when PartnerDevices will be removed|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|DateTime in UTC when PartnerDevices will be marked as NonCompliant|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/devicemanagementpartner.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementpartner_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 488

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2017-01-01T00:03:33.2924976+03:00",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2017-01-01T00:03:09.2463513+03:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:57.0898884+03:00"
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
Content-Length: 537

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "da463021-3021-da46-2130-46da213046da",
  "lastHeartbeatDateTime": "2017-01-01T00:03:33.2924976+03:00",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2017-01-01T00:03:09.2463513+03:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:57.0898884+03:00"
}
```

