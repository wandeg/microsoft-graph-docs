---
title: "Create deviceManagementPartners"
description: "Create a new deviceManagementPartners object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceManagementPartners

Namespace: microsoft.graph

Create a new deviceManagementPartners object.

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
POST /deviceManagement/deviceManagementPartners
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementPartner](../resources/devicemanagementpartner.md) object.

The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/devicemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastHeartbeatDateTime|DateTimeOffset|**TODO: Add Description**|
|partnerState|deviceManagementPartnerTenantState|**TODO: Add Description**. Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|deviceManagementPartnerAppType|**TODO: Add Description**. Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isConfigured|Boolean|**TODO: Add Description**|
|whenPartnerDevicesWillBeRemoved|DateTimeOffset|**TODO: Add Description**|
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset|**TODO: Add Description**|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|**TODO: Add Description**|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|**TODO: Add Description**|
|groupsRequiringPartnerEnrollment|[deviceManagementPartnerAssignment](../resources/devicemanagementpartnerassignment.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/devicemanagementpartner.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementpartner_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
Content-Type: application/json
Content-length: 684

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementpartner"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

