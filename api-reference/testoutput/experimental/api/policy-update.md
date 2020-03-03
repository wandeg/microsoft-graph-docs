---
title: "Update policy"
description: "Update the properties of a policy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update policy

Update the properties of a [policy](../resources/policy.md) object.

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
PATCH /policies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [policy](../resources/policy.md) object.

The following table shows the properties that are required when you create the [policy](../resources/policy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [policy](../resources/policy.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_policy"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/policies
Content-type: application/json
Content-length: 48

{
  "@odata.type": "#microsoft.graph.policy"
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
Content-Length: 97

{
  "@odata.type": "#microsoft.graph.policy",
  "id": "88e8f630-f630-88e8-30f6-e88830f6e888"
}
```

