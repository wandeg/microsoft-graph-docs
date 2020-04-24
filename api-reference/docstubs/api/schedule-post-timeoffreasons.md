---
title: "Create timeOffReasons"
description: "Create a new timeOffReasons object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create timeOffReasons

Namespace: microsoft.graph

Create a new timeOffReasons object.

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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/timeOffReasons
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [timeOffReason](../resources/timeoffreason.md) object.

The following table shows the properties that are required when you create the [timeOffReason](../resources/timeoffreason.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|displayName|String|**TODO: Add Description**|
|iconType|timeOffReasonIconType|**TODO: Add Description**. Possible values are: `none`, `car`, `calendar`, `running`, `plane`, `firstAid`, `doctor`, `notWorking`, `clock`, `juryDuty`, `globe`, `cup`, `phone`, `weather`, `umbrella`, `piggyBank`, `dog`, `cake`, `trafficCone`, `pin`, `sunny`, `unknownFutureValue`.|
|isActive|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_timeoffreason_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/timeOffReasons
Content-Type: application/json
Content-length: 141

{
  "@odata.type": "#microsoft.graph.timeOffReason",
  "displayName": "Display Name value",
  "iconType": "String",
  "isActive": true
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeoffreason"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.timeOffReason",
  "id": "e4a9f7ad-f7ad-e4a9-adf7-a9e4adf7a9e4",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "displayName": "Display Name value",
  "iconType": "String",
  "isActive": true
}
```

