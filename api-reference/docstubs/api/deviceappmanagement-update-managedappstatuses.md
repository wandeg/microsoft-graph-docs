---
title: "Update managedAppStatuses"
description: "Update the properties of a managedAppStatuses object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update managedAppStatuses

Namespace: microsoft.graph

Update the properties of a managedAppStatuses object.

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
PATCH /deviceAppManagement/managedAppStatuses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [managedAppStatus](../resources/managedappstatus.md) object.

The following table shows the properties that are required when you create the [managedAppStatus](../resources/managedappstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|Friendly name of the status report.|
|version|String|Version of the entity.|



## Response
If successful, this method returns a `200 OK` response code and an updated [managedAppStatus](../resources/managedappstatus.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_managedappstatuses"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
Content-Type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "Display Name value",
  "version": "Version value"
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
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "id": "81189725-9725-8118-2597-188125971881",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

