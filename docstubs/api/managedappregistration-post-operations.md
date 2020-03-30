---
title: "Add operations"
description: "Add operations by posting to the operations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add operations

Namespace: microsoft.graph

Add operations by posting to the operations collection.

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
POST /me/managedAppRegistrations/{managedAppRegistrationId}/operations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedAppOperation](../resources/managedappoperation.md) object.

The following table shows the properties that are required when you create the [managedAppOperation](../resources/managedappoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||
|state|String||
|version|String||



## Response
If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/managedappoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedappoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedappoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "id": "c3f35979-5979-c3f3-7959-f3c37959f3c3",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "state": "State value",
  "version": "Version value"
}
```

