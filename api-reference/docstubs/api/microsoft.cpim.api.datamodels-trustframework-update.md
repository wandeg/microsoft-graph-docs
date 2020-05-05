---
title: "Update trustFramework"
description: "Update the properties of a trustFramework object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update trustFramework

Namespace: microsoft.cpim.api.dataModels

Update the properties of a [trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md) object.

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
PATCH /trustFramework
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md) object.

The following table shows the properties that are required when you create the [trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_trustframework"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/trustFramework
Content-Type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.cpim.api.dataModels.trustFramework"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.trustFramework",
  "id": "1579292e-292e-1579-2e29-79152e297915"
}
```

