---
title: "outlookUser: supportedTimeZones"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# supportedTimeZones

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /me/outlook/supportedTimeZones
GET /users/{usersId}/outlook/supportedTimeZones
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|TimeZoneStandard|timeZoneStandard|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [timeZoneInformation](../resources/timezoneinformation.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "outlookuser_supportedtimezones"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.timezoneinformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "microsoft.graph.timeZoneInformation"
    }
  ]
}
```

