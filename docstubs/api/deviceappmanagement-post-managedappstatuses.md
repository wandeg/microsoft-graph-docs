---
title: "Add managedAppStatuses"
description: "Add managedAppStatuses by posting to the managedAppStatuses collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add managedAppStatuses

Namespace: microsoft.graph

Add managedAppStatuses by posting to the managedAppStatuses collection.

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
POST /deviceAppManagement/managedAppStatuses/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedAppStatus](../resources/managedappstatus.md) object.

The following table shows the properties that are required when you create the [managedAppStatus](../resources/managedappstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|version|String||



## Response
If successful, this method returns a `201 Created` response code and a [managedAppStatus](../resources/managedappstatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedappstatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedappstatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "id": "2145b56d-b56d-2145-6db5-45216db54521",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

