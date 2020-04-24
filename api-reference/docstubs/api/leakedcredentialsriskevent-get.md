---
title: "Get leakedCredentialsRiskEvent"
description: "Read the properties and relationships of a leakedCredentialsRiskEvent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get leakedCredentialsRiskEvent

Namespace: microsoft.graph

Read the properties and relationships of a [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object.

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
GET /leakedCredentialsRiskEvents/{leakedCredentialsRiskEventsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/leakedCredentialsRiskEvents/{leakedCredentialsRiskEventsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.leakedCredentialsRiskEvent",
    "id": "621c2d43-2d43-621c-432d-1c62432d1c62",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "riskEventDateTime": "2017-01-01T00:02:03.6171597+03:00",
    "riskEventType": "Risk Event Type value",
    "riskLevel": "String",
    "riskEventStatus": "String",
    "closedDateTime": "2016-12-31T23:58:06.1799456+03:00",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "userId": "User Id value"
  }
}
```

