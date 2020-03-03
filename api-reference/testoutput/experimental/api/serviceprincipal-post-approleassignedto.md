---
title: "Add appRoleAssignedTo"
description: "Add appRoleAssignedTo by posting to the appRoleAssignedTo collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add appRoleAssignedTo

Add appRoleAssignedTo by posting to the appRoleAssignedTo collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the appRoleAssignment object.

The following table shows the properties that are required when you create the appRoleAssignment.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appRoleId|Guid||
|creationTimestamp|DateTimeOffset||
|principalDisplayName|String||
|principalId|Guid||
|principalType|String||
|resourceDisplayName|String||
|resourceId|Guid||



## Response
If successful, this method returns a `201 Created` response code and a [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_approleassignments"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
Content-type: application/json
Content-length: 451

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "d105223c-223c-d105-3c22-05d13c2205d1",
  "creationTimestamp": "2017-01-01T00:03:08.4498325+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "ad7e366f-366f-ad7e-6f36-7ead6f367ead",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "05450f46-0f46-0545-460f-4505460f4505"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 500

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "110e998a-998a-110e-8a99-0e118a990e11",
  "appRoleId": "d105223c-223c-d105-3c22-05d13c2205d1",
  "creationTimestamp": "2017-01-01T00:03:08.4498325+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "ad7e366f-366f-ad7e-6f36-7ead6f367ead",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "05450f46-0f46-0545-460f-4505460f4505"
}
```

