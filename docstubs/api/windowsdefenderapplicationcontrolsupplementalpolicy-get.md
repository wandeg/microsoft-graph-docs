---
title: "Get windowsDefenderApplicationControlSupplementalPolicy"
description: "Read properties and relationships of the windowsDefenderApplicationControlSupplementalPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsDefenderApplicationControlSupplementalPolicy

Namespace: microsoft.graph

Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.

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
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsdefenderapplicationcontrolsupplementalpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
    "id": "fbc55652-5652-fbc5-5256-c5fb5256c5fb",
    "displayName": "Display Name value",
    "description": "Description value",
    "content": "Y29udGVudA==",
    "contentFileName": "Content File Name value",
    "version": "Version value",
    "creationDateTime": "2017-01-01T00:02:18.736171+00:00",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```

