---
title: "Update appLogCollectionRequest"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update appLogCollectionRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an appLogCollectionRequest object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request body

In the request body, supply JSON representation of the appLogCollectionRequest object.

The following table shows the properties that are required when you create the appLogCollectionRequest object.

| Property                | Type                           | Description                                                         |
| :---------------------- | :----------------------------- | :------------------------------------------------------------------ |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription)                               |
| completedDateTime       | DateTimeOffset                 | Time at which the upload log request reached a terminal state       |
| customLogFolders        | String collection              | List of log folders.                                                |
| errorMessage            | String                         | Error message if any during the upload process                      |
| id                      | String                         | The unique Identifier. This is userId_DeviceId_AppId id. Read-only. |
| status                  | String                         | Log upload status                                                   |

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [appLogCollectionRequest](../resources/appLogCollectionRequest.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_applogcollectionrequest"
}
-->

```http
PATCH https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "completedDateTime": "DateTimeOffset",
  "customLogFolders": [
    "String"
  ],
  "errorMessage": "String",
  "status": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.appLogCollectionRequest"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "completedDateTime": "DateTimeOffset",
  "customLogFolders": [
    "String"
  ],
  "errorMessage": "String",
  "id": "String(identifier)",
  "status": "String"
}
}

```