---
title: "Create networkIPv6ConfigurationManagementCondition"
description: "Create a new networkIPv6ConfigurationManagementCondition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create networkIPv6ConfigurationManagementCondition

Namespace: microsoft.graph

Create a new [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) object.

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
POST ** Collection URI for microsoft.graph.networkIPv6ConfigurationManagementCondition not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) object.

The following table shows the properties that are required when you create the [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|uniqueName|String|Unique name for the management condition. Used in management condition expressions. Inherited from [managementCondition](../resources/managementcondition.md)|
|displayName|String|The admin defined name of the management condition. Inherited from [managementCondition](../resources/managementcondition.md)|
|description|String|The admin defined description of the management condition. Inherited from [managementCondition](../resources/managementcondition.md)|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side. Inherited from [managementCondition](../resources/managementcondition.md)|
|modifiedDateTime|DateTimeOffset|The time the management condition was last modified. Updated service side. Inherited from [managementCondition](../resources/managementcondition.md)|
|eTag|String|ETag of the management condition. Updated service side. Inherited from [managementCondition](../resources/managementcondition.md)|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition. Inherited from [managementCondition](../resources/managementcondition.md). Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ipV6Prefix|String|The IPv6 subnet to be connected to. e.g. 2001:db8::/32|
|ipV6Gateway|String|The IPv6 gateway address to. e.g 2001:db8::1|
|ipV6DNSServerList|String collection|An IPv6 DNS servers configured for the adapter.|
|dnsSuffixList|String collection|Valid DNS suffixes for the current network. e.g. seattle.contoso.com|



## Response
If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_networkipv6configurationmanagementcondition_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.networkIPv6ConfigurationManagementCondition not found
Content-type: application/json
Content-length: 475

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.networkipv6configurationmanagementcondition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 642

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
```

