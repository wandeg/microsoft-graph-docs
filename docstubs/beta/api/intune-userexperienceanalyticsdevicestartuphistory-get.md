---
title: "Get userExperienceAnalyticsDeviceStartupHistory"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get userExperienceAnalyticsDeviceStartupHistory

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships a userExperienceAnalyticsDeviceStartupHistory object.

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

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/userExperienceAnalyticsDeviceStartupHistory.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsdevicestartuphistory"
}
-->

```http
GET https://graph.microsoft.com/beta/

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsDeviceStartupHistory"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "coreBootTimeInMs": "Int32",
  "coreLoginTimeInMs": "Int32",
  "deviceId": "String",
  "featureUpdateBootTimeInMs": "Int32",
  "groupPolicyBootTimeInMs": "Int32",
  "groupPolicyLoginTimeInMs": "Int32",
  "id": "String(identifier)",
  "isFeatureUpdate": "Boolean",
  "isFirstLogin": "Boolean",
  "operatingSystemVersion": "String",
  "responsiveDesktopTimeInMs": "Int32",
  "startTime": "DateTimeOffset",
  "totalBootTimeInMs": "Int32",
  "totalLoginTimeInMs": "Int32"
}
}

```