---
title: "Update controls"
description: "Update the properties of a controls object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update controls

Namespace: microsoft.graph

Update the properties of a controls object.

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
PATCH /programs/{programsId}/controls
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [programControl](../resources/programcontrol.md) object.

The following table shows the properties that are required when you create the [programControl](../resources/programcontrol.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|controlId|String|**TODO: Add Description**|
|programId|String|**TODO: Add Description**|
|controlTypeId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|owner|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|resource|[programResource](../resources/programresource.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [programControl](../resources/programcontrol.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_controls"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/programs/{programsId}/controls
Content-Type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.programControl",
  "controlId": "Control Id value",
  "programId": "Program Id value",
  "controlTypeId": "Control Type Id value",
  "displayName": "Display Name value",
  "status": "Status value",
  "owner": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "resource": {
    "@odata.type": "microsoft.graph.programResource",
    "type": "Type value"
  }
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
  "@odata.type": "#microsoft.graph.programControl",
  "id": "5a1d1496-1496-5a1d-9614-1d5a96141d5a",
  "controlId": "Control Id value",
  "programId": "Program Id value",
  "controlTypeId": "Control Type Id value",
  "displayName": "Display Name value",
  "status": "Status value",
  "owner": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "resource": {
    "@odata.type": "microsoft.graph.programResource",
    "type": "Type value"
  },
  "createdDateTime": "2017-01-01T00:02:14.13292+00:00"
}
```

