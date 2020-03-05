---
title: "Get windowsUpdateForBusinessConfiguration"
description: "Read properties and relationships of the windowsUpdateForBusinessConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsUpdateForBusinessConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.windowsUpdateForBusinessConfiguration not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsupdateforbusinessconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.windowsUpdateForBusinessConfiguration not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdateForBusinessConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1045

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "436380b0-80b0-4363-b080-6343b0806343",
    "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
    "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "deliveryOptimizationMode": "String",
    "prereleaseFeatures": "String",
    "automaticUpdateMode": "String",
    "microsoftUpdateServiceAllowed": true,
    "driversExcluded": true,
    "installationSchedule": {
      "@odata.type": "microsoft.graph.windowsUpdateInstallScheduleType"
    },
    "qualityUpdatesDeferralPeriodInDays": 2,
    "featureUpdatesDeferralPeriodInDays": 2,
    "qualityUpdatesPaused": true,
    "featureUpdatesPaused": true,
    "qualityUpdatesPauseExpiryDateTime": "2016-12-31T23:58:55.8726181+03:00",
    "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:59:52.8851894+03:00",
    "businessReadyUpdatesOnly": "String"
  }
}
```

