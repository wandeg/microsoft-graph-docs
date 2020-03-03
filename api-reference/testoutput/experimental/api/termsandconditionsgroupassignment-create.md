---
title: "Create termsAndConditionsGroupAssignment"
description: "Create a new termsAndConditionsGroupAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create termsAndConditionsGroupAssignment

Namespace: microsoft.graph

Create a new [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.

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
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.

The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetGroupId|String|Unique identifier of a group that the T&C policy is assigned to.|



## Response
If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_termsandconditionsgroupassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termsandconditionsgroupassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "51085c9a-5c9a-5108-9a5c-08519a5c0851",
  "targetGroupId": "Target Group Id value"
}
```

