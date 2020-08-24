---
title: "Update dataSharingConsent"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update dataSharingConsent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a dataSharingConsent object.

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

In the request body, supply JSON representation of the dataSharingConsent object.

The following table shows the properties that are required when you create the dataSharingConsent object.

| Property                | Type                           | Description                                                  |
| :---------------------- | :----------------------------- | :----------------------------------------------------------- |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription)                        |
| grantDateTime           | DateTimeOffset                 | The time consent was granted for this account                |
| granted                 | Boolean                        | The granted state for the data sharing consent               |
| grantedByUpn            | String                         | The Upn of the user that granted consent for this account    |
| grantedByUserId         | String                         | The UserId of the user that granted consent for this account |
| id                      | String                         | The data sharing consent Id Read-only.                       |
| serviceDisplayName      | String                         | The display name of the service work flow                    |
| termsUrl                | String                         | The TermsUrl for the data sharing consent                    |

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [dataSharingConsent](../resources/dataSharingConsent.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_datasharingconsent"
}
-->

```http
PATCH https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 244

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "grantDateTime": "DateTimeOffset",
  "granted": "Boolean",
  "grantedByUpn": "String",
  "grantedByUserId": "String",
  "serviceDisplayName": "String",
  "termsUrl": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.dataSharingConsent"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "grantDateTime": "DateTimeOffset",
  "granted": "Boolean",
  "grantedByUpn": "String",
  "grantedByUserId": "String",
  "id": "String(identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String"
}
}

```