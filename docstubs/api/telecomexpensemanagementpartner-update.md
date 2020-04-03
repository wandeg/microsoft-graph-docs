---
title: "Update telecomExpenseManagementPartner"
description: "Update the properties of a telecomExpenseManagementPartner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update telecomExpenseManagementPartner

Namespace: microsoft.graph

Update the properties of a [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.

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
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.

The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|url|String||
|appAuthorized|Boolean||
|enabled|Boolean||
|lastConnectionDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_telecomexpensemanagementpartner"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2017-01-01T00:01:57.2663846+00:00"
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
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "25d0638c-638c-25d0-8c63-d0258c63d025",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2017-01-01T00:01:57.2663846+00:00"
}
```

