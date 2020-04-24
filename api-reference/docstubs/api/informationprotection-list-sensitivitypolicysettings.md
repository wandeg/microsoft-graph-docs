---
title: "List sensitivityPolicySettings"
description: "Get the sensitivityPolicySettings from the sensitivityPolicySettings navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List sensitivityPolicySettings

Namespace: microsoft.graph

Get the sensitivityPolicySettings from the sensitivityPolicySettings navigation property.

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
GET /invitations/{invitationsId}/invitedUser/informationProtection/sensitivityPolicySettings
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
If successful, this method returns a `200 OK` response code and a collection of [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sensitivitypolicysettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/informationProtection/sensitivityPolicySettings
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sensitivitypolicysettings)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sensitivityPolicySettings",
      "id": "c4096ccb-6ccb-c409-cb6c-09c4cb6c09c4",
      "isMandatory": true,
      "helpWebUrl": "https://example.com/helpWebUrl/",
      "downgradeSensitivityRequiresJustification": true,
      "applicableTo": "String"
    }
  ]
}
```

