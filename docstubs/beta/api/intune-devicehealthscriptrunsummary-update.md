---
title: "Update deviceHealthScriptRunSummary"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update deviceHealthScriptRunSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a deviceHealthScriptRunSummary object.

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

In the request body, supply JSON representation of the deviceHealthScriptRunSummary object.

The following table shows the properties that are required when you create the deviceHealthScriptRunSummary object.

| Property                | Type                           | Description                           |
| :---------------------- | :----------------------------- | :------------------------------------ |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription) |

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [deviceHealthScriptRunSummary](../resources/deviceHealthScriptRunSummary.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_devicehealthscriptrunsummary"
}
-->

```http
PATCH https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 524

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "detectionScriptErrorDeviceCount": "Int32",
  "detectionScriptPendingDeviceCount": "Int32",
  "issueDetectedDeviceCount": "Int32",
  "issueRemediatedCumulativeDeviceCount": "Int32",
  "issueRemediatedDeviceCount": "Int32",
  "issueReoccurredDeviceCount": "Int32",
  "lastScriptRunDateTime": "DateTimeOffset",
  "noIssueDetectedDeviceCount": "Int32",
  "remediationScriptErrorDeviceCount": "Int32",
  "remediationSkippedDeviceCount": "Int32"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.deviceHealthScriptRunSummary"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "detectionScriptErrorDeviceCount": "Int32",
  "detectionScriptPendingDeviceCount": "Int32",
  "id": "String(identifier)",
  "issueDetectedDeviceCount": "Int32",
  "issueRemediatedCumulativeDeviceCount": "Int32",
  "issueRemediatedDeviceCount": "Int32",
  "issueReoccurredDeviceCount": "Int32",
  "lastScriptRunDateTime": "DateTimeOffset",
  "noIssueDetectedDeviceCount": "Int32",
  "remediationScriptErrorDeviceCount": "Int32",
  "remediationSkippedDeviceCount": "Int32"
}
}

```