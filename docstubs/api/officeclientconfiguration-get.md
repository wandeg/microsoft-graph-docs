---
title: "Get officeClientConfiguration"
description: "Read properties and relationships of the officeClientConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get officeClientConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [officeClientConfiguration](../resources/officeclientconfiguration.md) object.

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
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
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
If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/officeclientconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_officeclientconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1078

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfiguration",
    "id": "945263d4-63d4-9452-d463-5294d4635294",
    "userPreferencePayload": "Stream",
    "policyPayload": "Stream",
    "description": "Description value",
    "displayName": "Display Name value",
    "priority": 8,
    "userCheckinSummary": {
      "@odata.type": "microsoft.graph.officeUserCheckinSummary",
      "succeededUserCount": 2,
      "failedUserCount": 15
    },
    "checkinStatuses": [
      {
        "@odata.type": "microsoft.graph.officeClientCheckinStatus",
        "userPrincipalName": "User Principal Name value",
        "deviceName": "Device Name value",
        "devicePlatform": "Device Platform value",
        "devicePlatformVersion": "Device Platform Version value",
        "wasSuccessful": true,
        "userId": "User Id value",
        "checkinDateTime": "2016-12-31T23:59:00.425875+03:00",
        "errorMessage": "Error Message value",
        "appliedPolicies": [
          "Applied Policies value"
        ]
      }
    ]
  }
}
```

