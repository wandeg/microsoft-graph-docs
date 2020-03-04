---
title: "List deviceManagements"
description: "List properties and relationships of the deviceManagement objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceManagements

Namespace: microsoft.graph

List properties and relationships of the [deviceManagement](../resources/devicemanagement.md) objects.

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
GET ** Collection URI for microsoft.graph.deviceManagement not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagement](../resources/devicemanagement.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagement"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceManagement not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagement)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagement",
      "id": "4a85ccea-ccea-4a85-eacc-854aeacc854a",
      "settings": {
        "@odata.type": "microsoft.graph.deviceManagementSettings",
        "deviceComplianceCheckinThresholdDays": 4,
        "isScheduledActionEnabled": true,
        "secureByDefault": true
      },
      "intuneBrand": {
        "@odata.type": "microsoft.graph.intuneBrand",
        "displayName": "Display Name value",
        "contactITName": "Contact ITName value",
        "contactITPhoneNumber": "Contact ITPhone Number value",
        "contactITEmailAddress": "Contact ITEmail Address value",
        "contactITNotes": "Contact ITNotes value",
        "privacyUrl": "https://example.com/privacyUrl/",
        "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
        "onlineSupportSiteName": "Online Support Site Name value",
        "themeColor": {
          "@odata.type": "microsoft.graph.rgbColor",
          "r": 1,
          "g": 1,
          "b": 1
        },
        "showLogo": true,
        "lightBackgroundLogo": {
          "@odata.type": "microsoft.graph.mimeContent",
          "type": "Type value",
          "value": "dmFsdWU="
        },
        "darkBackgroundLogo": {
          "@odata.type": "microsoft.graph.mimeContent"
        },
        "showNameNextToLogo": true,
        "showDisplayNameNextToLogo": true
      },
      "subscriptionState": "String"
    }
  ]
}
```

