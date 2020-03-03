---
title: "List windowsInformationProtectionNetworkLearningSummaries"
description: "List properties and relationships of the windowsInformationProtectionNetworkLearningSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windowsInformationProtectionNetworkLearningSummaries

Namespace: microsoft.graph

List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) objects.

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
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsinformationprotectionnetworklearningsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsinformationprotectionnetworklearningsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
      "id": "4e7d5a7e-5a7e-4e7d-7e5a-7d4e7e5a7d4e",
      "url": "Url value",
      "deviceCount": 11
    }
  ]
}
```

