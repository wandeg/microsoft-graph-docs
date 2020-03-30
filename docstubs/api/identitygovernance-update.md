---
title: "Update identityGovernance"
description: "Update the properties of a identityGovernance object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update identityGovernance

Namespace: microsoft.graph

Update the properties of a [identityGovernance](../resources/identitygovernance.md) object.

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
PATCH /identityGovernance
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [identityGovernance](../resources/identitygovernance.md) object.

The following table shows the properties that are required when you create the [identityGovernance](../resources/identitygovernance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [identityGovernance](../resources/identitygovernance.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_identitygovernance"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance
Content-type: application/json
Content-length: 60

{
  "@odata.type": "#microsoft.graph.identityGovernance"
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
Content-Length: 109

{
  "@odata.type": "#microsoft.graph.identityGovernance",
  "id": "f2b85f95-5f95-f2b8-955f-b8f2955fb8f2"
}
```

