---
title: "List installedApps"
description: "Get the teamsAppInstallations from the installedApps navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List installedApps

Namespace: microsoft.graph

Get the teamsAppInstallations from the installedApps navigation property.

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
GET /teams/{teamsId}/installedApps
GET /me/joinedGroups/{groupId}/team/installedApps
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamsappinstallation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/teams/{teamsId}/installedApps
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsappinstallation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 152

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsAppInstallation",
      "id": "c98be40a-e40a-c98b-0ae4-8bc90ae48bc9"
    }
  ]
}
```

