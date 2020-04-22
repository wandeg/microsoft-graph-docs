---
title: "Update programControlType"
description: "Update the properties of a programControlType object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update programControlType

Namespace: microsoft.graph

Update the properties of a [programControlType](../resources/programcontroltype.md) object.

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
PATCH /programControlTypes/{programControlTypesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [programControlType](../resources/programcontroltype.md) object.

The following table shows the properties that are required when you create the [programControlType](../resources/programcontroltype.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|controlTypeGroupId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [programControlType](../resources/programcontroltype.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_programcontroltype"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/programControlTypes/{programControlTypesId}
Content-Type: application/json
Content-length: 156

{
  "@odata.type": "#microsoft.graph.programControlType",
  "controlTypeGroupId": "Control Type Group Id value",
  "displayName": "Display Name value"
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
  "@odata.type": "#microsoft.graph.programControlType",
  "id": "ec1d2b57-2b57-ec1d-572b-1dec572b1dec",
  "controlTypeGroupId": "Control Type Group Id value",
  "displayName": "Display Name value"
}
```

