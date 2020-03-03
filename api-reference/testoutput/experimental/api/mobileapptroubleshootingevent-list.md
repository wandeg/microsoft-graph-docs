---
title: "List mobileAppTroubleshootingEvents"
description: "List properties and relationships of the mobileAppTroubleshootingEvent objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mobileAppTroubleshootingEvents

Namespace: microsoft.graph

List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) objects.

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
GET /deviceManagement/mobileAppTroubleshootingEvents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mobileapptroubleshootingevent"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/mobileAppTroubleshootingEvents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mobileapptroubleshootingevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1384

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "4b1b7b68-7b68-4b1b-687b-1b4b687b1b4b",
      "eventDateTime": "2017-01-01T00:01:42.7768776+03:00",
      "correlationId": "Correlation Id value",
      "troubleshootingErrorDetails": {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
        "context": "Context value",
        "failure": "Failure value",
        "failureDetails": "Failure Details value",
        "remediation": "Remediation value",
        "resources": [
          {
            "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
            "text": "Text value",
            "link": "Link value"
          }
        ]
      },
      "eventName": "Event Name value",
      "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "applicationId": "Application Id value",
      "history": [
        {
          "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
          "occurrenceDateTime": "2017-01-01T00:00:25.0683756+03:00"
        }
      ]
    }
  ]
}
```

