---
title: "getActivitiesByInterval"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getActivitiesByInterval

Namespace: microsoft.graph



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
GET /shares/{sharesId}/listItem/getActivitiesByInterval
GET /workbooks/{workbooksId}/listItem/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/list/items/{listItemId}/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/listItem/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/listItem/getActivitiesByInterval
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|startDateTime|String||
|endDateTime|String||
|interval|String||



## Response
If successful, this function returns a `200 OK` response code and a [itemActivityStat](../resources/itemactivitystat.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "listitem_getactivitiesbyinterval"
}
-->
``` http
GET https://graph.microsoft.com/beta/shares/{sharesId}/listItem/getActivitiesByInterval(startDateTime='parameterValue',endDateTime='parameterValue',interval='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemactivitystat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 815

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.itemActivityStat",
      "id": "b3bdfd6c-fd6c-b3bd-6cfd-bdb36cfdbdb3",
      "startDateTime": "2016-12-31T23:59:00.3105042+00:00",
      "endDateTime": "2016-12-31T23:57:26.2105705+00:00",
      "access": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "create": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "delete": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "edit": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "move": {
        "@odata.type": "microsoft.graph.itemActionStat"
      },
      "isTrending": true,
      "incompleteData": {
        "@odata.type": "microsoft.graph.incompleteData"
      }
    }
  ]
}
```

