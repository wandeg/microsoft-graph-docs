---
title: "List deviceEnrollmentConfigurations"
description: "Get the deviceEnrollmentConfigurations from the deviceEnrollmentConfigurations navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceEnrollmentConfigurations

Namespace: microsoft.graph

Get the deviceEnrollmentConfigurations from the deviceEnrollmentConfigurations navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/deviceEnrollmentConfigurations
GET /users/{usersId}/deviceEnrollmentConfigurations
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_deviceenrollmentconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/deviceEnrollmentConfigurations
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceenrollmentconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "323fdf55-df55-323f-55df-3f3255df3f32",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:00:27.4994223+03:00",
      "lastModifiedDateTime": "2016-12-31T23:57:51.1888653+03:00",
      "version": 7
    }
  ]
}
```

