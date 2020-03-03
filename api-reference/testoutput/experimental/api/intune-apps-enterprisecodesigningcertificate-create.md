---
title: "Create enterpriseCodeSigningCertificate"
description: "Create a new enterpriseCodeSigningCertificate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create enterpriseCodeSigningCertificate

Namespace: microsoft.graph

Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.

The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|Binary|The Windows Enterprise Code-Signing Certificate in the raw data format.|
|status|Enumeration|The Certificate Status Provisioned or not Provisioned. Possible values are: `notProvisioned`, `provisioned`.|
|subjectName|String|The Subject Name for the cert.|
|subject|String|The Subject Value for the cert.|
|issuerName|String|The Issuer Name for the cert.|
|issuer|String|The Issuer value for the cert.|
|expirationDateTime|DateTimeOffset|The Cert Expiration Date.|
|uploadDateTime|DateTimeOffset|The date time of CodeSigning Cert when it is uploaded.|



## Response
If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_enterprisecodesigningcertificate_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/enterpriseCodeSigningCertificates
Content-type: application/json
Content-length: 385

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "String",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
  "uploadDateTime": "2017-01-01T00:02:13.8421427+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.enterprisecodesigningcertificate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 434

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "09359bff-9bff-0935-ff9b-3509ff9b3509",
  "content": "Y29udGVudA==",
  "status": "String",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
  "uploadDateTime": "2017-01-01T00:02:13.8421427+03:00"
}
```

