---
title: "Get anonymousIpRiskEvent"
description: "Read the properties and relationships of an anonymousIpRiskEvent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get anonymousIpRiskEvent

Namespace: microsoft.graph

Read the properties and relationships of an [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object.

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
GET /anonymousIpRiskEvents/{anonymousIpRiskEventsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/anonymousIpRiskEvents/{anonymousIpRiskEventsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.anonymousIpRiskEvent",
    "id": "740f2544-2544-740f-4425-0f7444250f74",
    "userDisplayName": "String",
    "userPrincipalName": "String",
    "riskEventDateTime": "String (timestamp)",
    "riskEventType": "String",
    "riskLevel": "String",
    "riskEventStatus": "String",
    "closedDateTime": "String (timestamp)",
    "createdDateTime": "String (timestamp)",
    "userId": "String",
    "location": {
      "@odata.type": "microsoft.graph.signInLocation"
    },
    "ipAddress": "String"
  }
}
```

