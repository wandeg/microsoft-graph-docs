---
title: "List targetedManagedAppConfigurations"
description: "Get the targetedManagedAppConfigurations from the targetedManagedAppConfigurations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List targetedManagedAppConfigurations

Namespace: microsoft.graph

Get the targetedManagedAppConfigurations from the targetedManagedAppConfigurations navigation property.

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
GET /deviceAppManagement/targetedManagedAppConfigurations
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
If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_targetedmanagedappconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.targetedmanagedappconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 731

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "id": "38c87962-7962-38c8-6279-c8386279c838",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```

