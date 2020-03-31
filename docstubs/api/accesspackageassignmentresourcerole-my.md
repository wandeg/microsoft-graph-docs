---
title: "My"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# My

Namespace: microsoft.graph



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
GET /accessPackageAssignmentResourceRoles/My
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/My
GET /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentResourceRoles/My
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/My
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentresourcerole_my"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignmentResourceRoles/My
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignmentresourcerole)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
      "id": "6907cb03-cb03-6907-03cb-076903cb0769",
      "originId": "Origin Id value",
      "originSystem": "Origin System value",
      "status": "Status value"
    }
  ]
}
```

