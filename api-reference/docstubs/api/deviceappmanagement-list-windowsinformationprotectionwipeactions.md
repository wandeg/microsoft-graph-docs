---
title: "List windowsInformationProtectionWipeActions"
description: "Get the windowsInformationProtectionWipeActions from the windowsInformationProtectionWipeActions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List windowsInformationProtectionWipeActions

Namespace: microsoft.graph

Get the windowsInformationProtectionWipeActions from the windowsInformationProtectionWipeActions navigation property.

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
GET /deviceAppManagement/windowsInformationProtectionWipeActions
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
If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_windowsinformationprotectionwipeaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsinformationprotectionwipeaction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
      "id": "826f37aa-37aa-826f-aa37-6f82aa376f82",
      "status": "String",
      "targetedUserId": "Targeted User Id value",
      "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
      "targetedDeviceName": "Targeted Device Name value",
      "targetedDeviceMacAddress": "Targeted Device Mac Address value",
      "lastCheckInDateTime": "2017-01-01T00:01:25.4137809+03:00"
    }
  ]
}
```

