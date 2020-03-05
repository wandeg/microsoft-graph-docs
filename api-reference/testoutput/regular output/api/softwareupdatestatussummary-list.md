---
title: "List softwareUpdateStatusSummaries"
description: "List properties and relationships of the softwareUpdateStatusSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List softwareUpdateStatusSummaries

Namespace: microsoft.graph

List properties and relationships of the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) objects.

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
GET ** Collection URI for microsoft.graph.softwareUpdateStatusSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_softwareupdatestatussummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.softwareUpdateStatusSummary not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.softwareupdatestatussummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
      "id": "10dc47c0-47c0-10dc-c047-dc10c047dc10",
      "displayName": "Display Name value",
      "compliantDeviceCount": 4,
      "nonCompliantDeviceCount": 7,
      "remediatedDeviceCount": 5,
      "errorDeviceCount": 0,
      "unknownDeviceCount": 2,
      "conflictDeviceCount": 3,
      "notApplicableDeviceCount": 8,
      "compliantUserCount": 2,
      "nonCompliantUserCount": 5,
      "remediatedUserCount": 3,
      "errorUserCount": 14,
      "unknownUserCount": 0,
      "conflictUserCount": 1,
      "notApplicableUserCount": 6
    }
  ]
}
```

