---
title: "List defaultDeviceCompliancePolicies"
description: "List properties and relationships of the defaultDeviceCompliancePolicy objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List defaultDeviceCompliancePolicies

Namespace: microsoft.graph

List properties and relationships of the [defaultDeviceCompliancePolicy](../resources/defaultdevicecompliancepolicy.md) objects.

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
GET ** Collection URI for microsoft.graph.defaultDeviceCompliancePolicy not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [defaultDeviceCompliancePolicy](../resources/defaultdevicecompliancepolicy.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_defaultdevicecompliancepolicy"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.defaultDeviceCompliancePolicy not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.defaultdevicecompliancepolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
      "id": "88b6f316-f316-88b6-16f3-b68816f3b688",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "description": "Description value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```

