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
GET /drives/{drivesId}/root/getActivitiesByInterval
GET /shares/{sharesId}/root/getActivitiesByInterval
GET /workbooks/{workbooksId}/getActivitiesByInterval
GET /shares/{sharesId}/driveItem/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/root/getActivitiesByInterval
GET /drives/{drivesId}/items/{driveItemId}/getActivitiesByInterval
GET /shares/{sharesId}/items/{driveItemId}/getActivitiesByInterval
GET /drives/{drivesId}/bundles/{driveItemId}/getActivitiesByInterval
GET /drives/{drivesId}/special/{driveItemId}/getActivitiesByInterval
GET /drives/{drivesId}/following/{driveItemId}/getActivitiesByInterval
GET /workbooks/{workbooksId}/children/{driveItemId}/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/items/{driveItemId}/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/special/{driveItemId}/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/following/{driveItemId}/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/getActivitiesByInterval
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/getActivitiesByInterval
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
  "name": "driveitem_getactivitiesbyinterval"
}
-->
``` http
GET https://graph.microsoft.com/beta/drives/{drivesId}/root/getActivitiesByInterval(startDateTime='parameterValue',endDateTime='parameterValue',interval='parameterValue')
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
      "id": "d164322e-322e-d164-2e32-64d12e3264d1",
      "startDateTime": "2016-12-31T23:57:02.6825424+00:00",
      "endDateTime": "2016-12-31T23:59:12.2321935+00:00",
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

