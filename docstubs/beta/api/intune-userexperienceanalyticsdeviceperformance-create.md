---
title: "Create userExperienceAnalyticsDevicePerformance"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create userExperienceAnalyticsDevicePerformance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new userExperienceAnalyticsDevicePerformance object.

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

In the request body, supply JSON representation of the userExperienceAnalyticsDevicePerformance object.

The following table shows the properties that are required when you create the userExperienceAnalyticsDevicePerformance object.

| Property                | Type                           | Description                           |
| :---------------------- | :----------------------------- | :------------------------------------ |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription) |

Do not supply a request body for this method.

## Response

If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDevicePerformance](../resources/userExperienceAnalyticsDevicePerformance.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsdeviceperformance"
}
-->

```http
POST https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 516

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "bootScore": "Int32",
  "coreBootTimeInMs": "Int32",
  "coreLoginTimeInMs": "Int32",
  "deviceCount": "Int64",
  "deviceName": "String",
  "diskType": "String",
  "groupPolicyBootTimeInMs": "Int32",
  "groupPolicyLoginTimeInMs": "Int32",
  "healthStatus": "String",
  "loginScore": "Int32",
  "manufacturer": "String",
  "model": "String",
  "operatingSystemVersion": "String",
  "responsiveDesktopTimeInMs": "Int32"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsDevicePerformance"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "bootScore": "Int32",
  "coreBootTimeInMs": "Int32",
  "coreLoginTimeInMs": "Int32",
  "deviceCount": "Int64",
  "deviceName": "String",
  "diskType": "String",
  "groupPolicyBootTimeInMs": "Int32",
  "groupPolicyLoginTimeInMs": "Int32",
  "healthStatus": "String",
  "id": "String(identifier)",
  "loginScore": "Int32",
  "manufacturer": "String",
  "model": "String",
  "operatingSystemVersion": "String",
  "responsiveDesktopTimeInMs": "Int32"
}
}

```