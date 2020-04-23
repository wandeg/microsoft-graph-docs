---
title: "Create userStatusOverview"
description: "Create a new userStatusOverview object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userStatusOverview

Namespace: microsoft.graph

Create a new userStatusOverview object.

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
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.

The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|pendingCount|Int32|Number of pending Users|
|notApplicableCount|Int32|Number of not applicable users|
|successCount|Int32|Number of succeeded Users|
|errorCount|Int32|Number of error Users|
|failedCount|Int32|Number of failed Users|
|lastUpdateDateTime|DateTimeOffset|Last update time|
|configurationVersion|Int32|Version of the policy for that overview|



## Response
If successful, this method returns a `201 Created` response code and a [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicecomplianceuseroverview_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-Type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2017-01-01T00:01:10.8938585+03:00",
  "configurationVersion": 4
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicecomplianceuseroverview"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "70c5e981-e981-70c5-81e9-c57081e9c570",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2017-01-01T00:01:10.8938585+03:00",
  "configurationVersion": 4
}
```

