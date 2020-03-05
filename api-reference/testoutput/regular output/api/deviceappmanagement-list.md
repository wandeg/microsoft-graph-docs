---
title: "List deviceAppManagements"
description: "List properties and relationships of the deviceAppManagement objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceAppManagements

Namespace: microsoft.graph

List properties and relationships of the [deviceAppManagement](../resources/deviceappmanagement.md) objects.

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
GET ** Collection URI for microsoft.graph.deviceAppManagement not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceAppManagement](../resources/deviceappmanagement.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceappmanagement"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceAppManagement not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceappmanagement)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAppManagement",
      "id": "5b1223ef-23ef-5b12-ef23-125bef23125b",
      "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:58:55.447624+03:00",
      "isEnabledForMicrosoftStoreForBusiness": true,
      "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
      "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2016-12-31T23:58:17.743368+03:00"
    }
  ]
}
```

