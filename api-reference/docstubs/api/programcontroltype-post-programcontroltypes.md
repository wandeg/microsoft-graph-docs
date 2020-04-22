---
title: "Create programControlType"
description: "Create a new programControlType object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create programControlType

Namespace: microsoft.graph

Create a new [programControlType](../resources/programcontroltype.md) object.

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
POST /programControlTypes
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [programControlType](../resources/programcontroltype.md) object.

The following table shows the properties that are required when you create the [programControlType](../resources/programcontroltype.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|controlTypeGroupId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [programControlType](../resources/programcontroltype.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_programcontroltype_from_programcontroltypes"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/programControlTypes
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
  "truncated": true,
  "@odata.type": "microsoft.graph.programcontroltype"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.programControlType",
  "id": "7089a698-a698-7089-98a6-897098a68970",
  "controlTypeGroupId": "Control Type Group Id value",
  "displayName": "Display Name value"
}
```

