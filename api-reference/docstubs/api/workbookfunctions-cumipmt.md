---
title: "workbookFunctions: cumIPmt"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# cumIPmt

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/functions/cumIPmt
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|rate|[Json](../resources/json.md)|**TODO: Add Description**|
|nper|[Json](../resources/json.md)|**TODO: Add Description**|
|pv|[Json](../resources/json.md)|**TODO: Add Description**|
|startPeriod|[Json](../resources/json.md)|**TODO: Add Description**|
|endPeriod|[Json](../resources/json.md)|**TODO: Add Description**|
|type|[Json](../resources/json.md)|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [workbookFunctionResult](../resources/workbookfunctionresult.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "workbookfunctions_cumipmt"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/functions/cumIPmt

Content-Type: application/json
Content-length: 385

{
  "rate": {
    "@odata.type": "microsoft.graph.Json"
  },
  "nper": {
    "@odata.type": "microsoft.graph.Json"
  },
  "pv": {
    "@odata.type": "microsoft.graph.Json"
  },
  "startPeriod": {
    "@odata.type": "microsoft.graph.Json"
  },
  "endPeriod": {
    "@odata.type": "microsoft.graph.Json"
  },
  "type": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookfunctionresult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "id": "935dd6e3-d6e3-935d-e3d6-5d93e3d65d93",
    "error": "Error value",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

