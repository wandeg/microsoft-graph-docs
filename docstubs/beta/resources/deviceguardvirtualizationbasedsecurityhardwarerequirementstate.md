---
title: "deviceGuardVirtualizationBasedSecurityHardwareRequirementState enum type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# deviceGuardVirtualizationBasedSecurityHardwareRequirementState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Members

| Member                       | Value | Description                                      |
| :--------------------------- | ----: | :----------------------------------------------- |
| meetHardwareRequirements     | 0     | System meets hardware configuration requirements |
| secureBootRequired           | 1     | Secure boot required                             |
| dmaProtectionRequired        | 2     | DMA protection required                          |
| hyperVNotSupportedForGuestVM | 4     | HyperV not supported for Guest VM                |
| hyperVNotAvailable           | 8     | HyperV feature is not available                  |