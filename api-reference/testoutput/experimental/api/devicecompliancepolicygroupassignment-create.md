---
title: "Create deviceCompliancePolicyGroupAssignment"
description: "Create a new deviceCompliancePolicyGroupAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create deviceCompliancePolicyGroupAssignment

Namespace: microsoft.graph

Create a new [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object.

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
POST ** Collection URI for microsoft.graph.deviceCompliancePolicyGroupAssignment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetGroupId|String|The Id of the AAD group we are targeting the device compliance policy to.|
|excludeGroup|Boolean|Indicates if this group is should be excluded. Defaults that the group should be included|



## Response
If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyGroupAssignment](../resources/devicecompliancepolicygroupassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicecompliancepolicygroupassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceCompliancePolicyGroupAssignment not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.devicecompliancepolicygroupassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 198

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyGroupAssignment",
  "id": "081f893b-893b-081f-3b89-1f083b891f08",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

