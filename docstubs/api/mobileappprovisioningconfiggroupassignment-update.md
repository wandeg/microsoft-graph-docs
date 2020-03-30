---
title: "Update mobileAppProvisioningConfigGroupAssignment"
description: "Update the properties of a mobileAppProvisioningConfigGroupAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mobileAppProvisioningConfigGroupAssignment

Namespace: microsoft.graph

Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) object.

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
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) object.

The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetGroupId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mobileappprovisioningconfiggroupassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
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
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "id": "c6bcbf59-bf59-c6bc-59bf-bcc659bfbcc6",
  "targetGroupId": "Target Group Id value"
}
```

