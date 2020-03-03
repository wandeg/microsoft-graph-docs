---
title: "Create activityBasedTimeoutPolicy"
description: "Create a new activityBasedTimeoutPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create activityBasedTimeoutPolicy

Namespace: microsoft.graph

Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.

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
POST /policies/activityBasedTimeoutPolicies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.

The following table shows the properties that are required when you create the [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String| Inherited from [policyBase](../resources/policybase.md)|
|displayName|String| Inherited from [policyBase](../resources/policybase.md)|
|definition|String collection| Inherited from [stsPolicy](../resources/stspolicy.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stspolicy.md)|



## Response
If successful, this method returns a `201 Created` response code and a [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/policies/activityBasedTimeoutPolicies
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
  "truncated": true,
  "@odata.type": "microsoft.graph.activitybasedtimeoutpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.activityBasedTimeoutPolicy",
  "id": "e1930949-0949-e193-4909-93e1490993e1",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

