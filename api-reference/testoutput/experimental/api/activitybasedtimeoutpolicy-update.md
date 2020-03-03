---
title: "Update activityBasedTimeoutPolicy"
description: "Update the properties of a activityBasedTimeoutPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update activityBasedTimeoutPolicy

Update the properties of a [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.

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
PATCH /policies/activityBasedTimeoutPolicies/{activityBasedTimeoutPolicyId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [activityBasedTimeoutPolicy](../resources/activityBasedTimeoutPolicy.md) object.

The following table shows the properties that are required when you create the [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String| Inherited from [policyBase](../resources/policyBase.md)|
|displayName|String| Inherited from [policyBase](../resources/policyBase.md)|
|definition|String collection| Inherited from [stsPolicy](../resources/stsPolicy.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stsPolicy.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_activitybasedtimeoutpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/policies/activityBasedTimeoutPolicies/{activityBasedTimeoutPolicyId}
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.activityBasedTimeoutPolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
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
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.activityBasedTimeoutPolicy",
  "id": "86d5d598-d598-86d5-98d5-d58698d5d586",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

