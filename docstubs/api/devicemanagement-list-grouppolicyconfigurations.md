---
title: "List groupPolicyConfigurations"
description: "Get the groupPolicyConfigurations from the groupPolicyConfigurations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupPolicyConfigurations

Namespace: microsoft.graph

Get the groupPolicyConfigurations from the groupPolicyConfigurations navigation property.

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
GET /deviceManagement/groupPolicyConfigurations
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
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicyconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicyconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 447

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
      "id": "9908fa27-fa27-9908-27fa-089927fa0899",
      "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00"
    }
  ]
}
```

