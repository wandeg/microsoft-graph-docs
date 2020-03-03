---
title: "Update deviceCompliancePolicyGroupAssignment"
description: "Update the properties of a deviceCompliancePolicyGroupAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceCompliancePolicyGroupAssignment

Namespace: microsoft.graph

Update the properties of a [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object.

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
PATCH ** Entity URI for microsoft.graph.deviceCompliancePolicyGroupAssignment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetGroupId|String|The Id of the AAD group we are targeting the device compliance policy to.|
|excludeGroup|Boolean|Indicates if this group is should be excluded. Defaults that the group should be included|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicecompliancepolicygroupassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.deviceCompliancePolicyGroupAssignment not found
Content-type: application/json
Content-length: 149

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
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
Content-Length: 198

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyGroupAssignment",
  "id": "081f893b-893b-081f-3b89-1f083b891f08",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

