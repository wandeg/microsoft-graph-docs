﻿---
title: "deviceManagementExchangeAccessStateReason enum type"
description: "Device Exchange Access State Reason."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# deviceManagementExchangeAccessStateReason enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device Exchange Access State Reason.

## Members

| Member                        | Value | Description                                           |
| :---------------------------- | ----: | :---------------------------------------------------- |
| none                          | 0     | No access state reason discovered from Exchange       |
| unknown                       | 1     | Unknown access state reason                           |
| exchangeGlobalRule            | 2     | Access state determined by Exchange Global rule       |
| exchangeIndividualRule        | 3     | Access state determined by Exchange Individual rule   |
| exchangeDeviceRule            | 4     | Access state determined by Exchange Device rule       |
| exchangeUpgrade               | 5     | Access state due to Exchange upgrade                  |
| exchangeMailboxPolicy         | 6     | Access state determined by Exchange Mailbox Policy    |
| other                         | 7     | Access state determined by Exchange                   |
| compliant                     | 8     | Access state granted by compliance challenge          |
| notCompliant                  | 9     | Access state revoked by compliance challenge          |
| notEnrolled                   | 10    | Access state revoked by management challenge          |
| unknownLocation               | 12    | Access state due to unknown location                  |
| mfaRequired                   | 13    | Access state due to MFA challenge                     |
| azureADBlockDueToAccessPolicy | 14    | Access State revoked by AAD Access Policy             |
| compromisedPassword           | 15    | Access State revoked by compromised password          |
| deviceNotKnownWithManagedApp  | 16    | Access state revoked by managed application challenge |