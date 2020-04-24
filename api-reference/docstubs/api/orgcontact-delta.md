---
title: "orgContact: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /contacts/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [orgContact](../resources/orgcontact.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/contacts/delta
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.orgcontact)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "165a8813-8813-165a-1388-5a1613885a16",
      "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
      "addresses": [
        {
          "@odata.type": "microsoft.graph.physicalOfficeAddress"
        }
      ],
      "companyName": "Company Name value",
      "department": "Department value",
      "displayName": "Display Name value",
      "givenName": "Given Name value",
      "jobTitle": "Job Title value",
      "mail": "Mail value",
      "mailNickname": "Mail Nickname value",
      "onPremisesSyncEnabled": true,
      "onPremisesLastSyncDateTime": "2017-01-01T00:01:17.7456992+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError"
        }
      ],
      "phones": [
        {
          "@odata.type": "microsoft.graph.phone"
        }
      ],
      "proxyAddresses": [
        "Proxy Addresses value"
      ],
      "surname": "Surname value"
    }
  ]
}
```

