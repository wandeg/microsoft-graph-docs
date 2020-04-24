---
title: "Create symantecCodeSigningCertificate"
description: "Create a new symantecCodeSigningCertificate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create symantecCodeSigningCertificate

Namespace: microsoft.graph

Create a new symantecCodeSigningCertificate object.

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
POST /deviceAppManagement/symantecCodeSigningCertificate
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.

The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|content|Binary|The Windows Symantec Code-Signing Certificate in the raw data format.|
|status|certificateStatus|The Cert Status Provisioned or not Provisioned. Possible values are: `notProvisioned`, `provisioned`.|
|password|String|The Password required for .pfx file.|
|subjectName|String|The Subject Name for the cert.|
|subject|String|The Subject value for the cert.|
|issuerName|String|The Issuer Name for the cert.|
|issuer|String|The Issuer value for the cert.|
|expirationDateTime|DateTimeOffset|The Cert Expiration Date.|
|uploadDateTime|DateTimeOffset|The Type of the CodeSigning Cert as Symantec Cert.|



## Response
If successful, this method returns a `201 Created` response code and a [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_symanteccodesigningcertificate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-Type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "String",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "uploadDateTime": "2017-01-01T00:01:55.145768+03:00"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.symanteccodesigningcertificate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "7c79f2e8-f2e8-7c79-e8f2-797ce8f2797c",
  "content": "Y29udGVudA==",
  "status": "String",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "uploadDateTime": "2017-01-01T00:01:55.145768+03:00"
}
```

