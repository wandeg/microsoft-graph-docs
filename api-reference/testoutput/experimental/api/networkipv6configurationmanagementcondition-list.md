---
title: "List networkIPv6ConfigurationManagementConditions"
description: "List properties and relationships of the networkIPv6ConfigurationManagementCondition objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List networkIPv6ConfigurationManagementConditions

Namespace: microsoft.graph

List properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) objects.

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
GET ** Collection URI for microsoft.graph.networkIPv6ConfigurationManagementCondition not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_networkipv6configurationmanagementcondition"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.networkIPv6ConfigurationManagementCondition not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.networkipv6configurationmanagementcondition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 751

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
      "id": "904a3b62-3b62-904a-623b-4a90623b4a90",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "String"
      ],
      "ipV6Prefix": "Ip V6Prefix value",
      "ipV6Gateway": "Ip V6Gateway value",
      "ipV6DNSServerList": [
        "Ip V6DNSServer List value"
      ],
      "dnsSuffixList": [
        "Dns Suffix List value"
      ]
    }
  ]
}
```

