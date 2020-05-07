---
title: "Get deviceManagementPartner"
description: "Read the properties and relationships of a deviceManagementPartner object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get deviceManagementPartner

Namespace: microsoft.graph

Read the properties and relationships of a [deviceManagementPartner](../resources/devicemanagementpartner.md) object.

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
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [deviceManagementPartner](../resources/devicemanagementpartner.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementpartner"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementPartner",
    "id": "73431e3c-1e3c-7343-3c1e-43733c1e4373",
    "lastHeartbeatDateTime": "String (timestamp)",
    "partnerState": "String",
    "partnerAppType": "String",
    "singleTenantAppId": "String",
    "displayName": "String",
    "isConfigured": "Boolean",
    "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
    "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
    "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)",
    "groupsRequiringPartnerEnrollment": [
      {
        "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
      }
    ]
  }
}
```

