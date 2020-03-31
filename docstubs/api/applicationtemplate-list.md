---
title: "List applicationTemplates"
description: "List properties and relationships of the applicationTemplate objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List applicationTemplates

Namespace: microsoft.graph

List properties and relationships of the [applicationTemplate](../resources/applicationtemplate.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /applicationTemplates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/applicationTemplates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.applicationtemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 638

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.applicationTemplate",
      "id": "47293385-3385-4729-8533-294785332947",
      "displayName": "Display Name value",
      "homePageUrl": "https://example.com/homePageUrl/",
      "supportedSingleSignOnModes": [
        "Supported Single Sign On Modes value"
      ],
      "supportedProvisioningTypes": [
        "Supported Provisioning Types value"
      ],
      "logoUrl": "https://example.com/logoUrl/",
      "categories": [
        "Categories value"
      ],
      "publisher": "Publisher value",
      "description": "Description value"
    }
  ]
}
```

