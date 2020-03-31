---
title: "Update dataLossPreventionPolicy"
description: "Update the properties of a dataLossPreventionPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update dataLossPreventionPolicy

Namespace: microsoft.graph

Update the properties of a [dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) object.

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
PATCH /informationProtection/dataLossPreventionPolicies/{dataLossPreventionPolicyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) object.

The following table shows the properties that are required when you create the [dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_datalosspreventionpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/informationProtection/dataLossPreventionPolicies/{dataLossPreventionPolicyId}
Content-type: application/json
Content-length: 91

{
  "@odata.type": "#microsoft.graph.dataLossPreventionPolicy",
  "name": "Name value"
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
Content-Length: 140

{
  "@odata.type": "#microsoft.graph.dataLossPreventionPolicy",
  "id": "6812d73e-d73e-6812-3ed7-12683ed71268",
  "name": "Name value"
}
```

