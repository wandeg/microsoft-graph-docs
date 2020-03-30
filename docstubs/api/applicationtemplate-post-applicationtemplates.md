---
title: "Create applicationTemplate"
description: "Create a new applicationTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create applicationTemplate

Namespace: microsoft.graph

Create a new [applicationTemplate](../resources/applicationtemplate.md) object.

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
POST /applicationTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [applicationTemplate](../resources/applicationtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_applicationtemplate_from_applicationtemplates"
}
-->
``` http
POST https://graph.microsoft.com/beta/applicationTemplates
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
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationtemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.applicationTemplate",
  "id": "04e16492-6492-04e1-9264-e1049264e104",
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

