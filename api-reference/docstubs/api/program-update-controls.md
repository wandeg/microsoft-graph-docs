---
title: "Update controls"
description: "Update the properties of a controls object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.

The following table shows the properties that are required when you create the [programControl](../resources/programcontrol.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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
PATCH https://graph.microsoft.com/beta/programs/{programsId}/controls
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
**Note:** The response object shown here might be shortened for readability.
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
  "id": "f522c821-c821-f522-21c8-22f521c822f5",
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
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00"
}
```

