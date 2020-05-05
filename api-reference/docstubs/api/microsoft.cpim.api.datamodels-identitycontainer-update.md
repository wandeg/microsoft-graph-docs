---
title: "Update identityContainer"
description: "Update the properties of a identityContainer object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update identityContainer

Namespace: microsoft.cpim.api.dataModels

Update the properties of a [identityContainer](../resources/microsoft.cpim.api.datamodels-identitycontainer.md) object.

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
PATCH /identity
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [identityContainer](../resources/microsoft.cpim.api.datamodels-identitycontainer.md) object.

The following table shows the properties that are required when you create the [identityContainer](../resources/microsoft.cpim.api.datamodels-identitycontainer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [identityContainer](../resources/microsoft.cpim.api.datamodels-identitycontainer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_identitycontainer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity
Content-Type: application/json
Content-length: 73

{
  "@odata.type": "#microsoft.cpim.api.dataModels.identityContainer"
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
  "@odata.type": "#microsoft.cpim.api.dataModels.identityContainer",
  "id": "7bd92cac-2cac-7bd9-ac2c-d97bac2cd97b"
}
```

