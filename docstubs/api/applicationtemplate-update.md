---
title: "Update applicationTemplate"
description: "Update the properties of a applicationTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update applicationTemplate

Namespace: microsoft.graph

Update the properties of a [applicationTemplate](../resources/applicationtemplate.md) object.

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
PATCH /applicationTemplates/{applicationTemplatesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [applicationTemplate](../resources/applicationtemplate.md) object.

The following table shows the properties that are required when you create the [applicationTemplate](../resources/applicationtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|homePageUrl|String||
|supportedSingleSignOnModes|String collection||
|supportedProvisioningTypes|String collection||
|logoUrl|String||
|categories|String collection||
|publisher|String||
|description|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [applicationTemplate](../resources/applicationtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_applicationtemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applicationTemplates/{applicationTemplatesId}
Content-type: application/json
Content-length: 492

{
  "@odata.type": "#microsoft.graph.applicationTemplate",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.applicationTemplate",
  "id": "8478b054-b054-8478-54b0-788454b07884",
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
```

