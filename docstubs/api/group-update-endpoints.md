---
title: "Update endpoints"
description: "Update the properties of an endpoints object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update endpoints

Namespace: microsoft.graph

Update the properties of an endpoints object.

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
PATCH /groups/{groupsId}/endpoints
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/endpoints
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [endpoint](../resources/endpoint.md) object.

The following table shows the properties that are required when you create the [endpoint](../resources/endpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|capability|String|**TODO: Add Description**|
|providerId|String|**TODO: Add Description**|
|providerName|String|**TODO: Add Description**|
|uri|String|**TODO: Add Description**|
|providerResourceId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [endpoint](../resources/endpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_endpoints"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/endpoints
Content-Type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.endpoint",
  "deletedDateTime": "2016-12-31T23:56:33.098707+03:00",
  "capability": "Capability value",
  "providerId": "Provider Id value",
  "providerName": "Provider Name value",
  "uri": "Uri value",
  "providerResourceId": "Provider Resource Id value"
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
  "@odata.type": "#microsoft.graph.endpoint",
  "id": "1e2072d4-72d4-1e20-d472-201ed472201e",
  "deletedDateTime": "2016-12-31T23:56:33.098707+03:00",
  "capability": "Capability value",
  "providerId": "Provider Id value",
  "providerName": "Provider Name value",
  "uri": "Uri value",
  "providerResourceId": "Provider Resource Id value"
}
```

