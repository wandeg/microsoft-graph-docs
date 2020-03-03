---
title: "List networkIPv4ConfigurationManagementConditions"
description: "List properties and relationships of the networkIPv4ConfigurationManagementCondition objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List networkIPv4ConfigurationManagementConditions

List properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) objects.

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
GET ** Collection URI for microsoft.graph.networkIPv4ConfigurationManagementCondition not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_networkipv4configurationmanagementcondition"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.networkIPv4ConfigurationManagementCondition not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.networkipv4configurationmanagementcondition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 802

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
      "id": "be6ebca1-bca1-be6e-a1bc-6ebea1bc6ebe",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
      "modifiedDateTime": "2017-01-01T00:03:12.7204145+03:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "String"
      ],
      "ipV4Prefix": "Ip V4Prefix value",
      "ipV4Gateway": "Ip V4Gateway value",
      "ipV4DHCPServer": "Ip V4DHCPServer value",
      "ipV4DNSServerList": [
        "Ip V4DNSServer List value"
      ],
      "dnsSuffixList": [
        "Dns Suffix List value"
      ]
    }
  ]
}
```

