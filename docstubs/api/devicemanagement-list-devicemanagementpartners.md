---
title: "List deviceManagementPartners"
description: "Get the deviceManagementPartners from the deviceManagementPartners navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceManagementPartners

Namespace: microsoft.graph

Get the deviceManagementPartners from the deviceManagementPartners navigation property.

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
GET /deviceManagement/deviceManagementPartners
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/devicemanagementpartner.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementpartner"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementpartner)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1052

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "988b73c0-73c0-988b-c073-8b98c0738b98",
      "lastHeartbeatDateTime": "2017-01-01T00:00:12.4442527+03:00",
      "partnerState": "String",
      "partnerAppType": "String",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:01:40.7347161+03:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2016-12-31T23:57:41.8716965+03:00",
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:57:14.8047707+03:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2017-01-01T00:02:34.0096799+03:00",
      "groupsRequiringPartnerEnrollment": [
        {
          "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
          }
        }
      ]
    }
  ]
}
```

