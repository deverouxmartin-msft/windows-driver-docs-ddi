---
UID: NS:d3dumddi.D3DDDICB_OFFERALLOCATIONS2
title: D3DDDICB_OFFERALLOCATIONS2
author: windows-driver-content
description: Used to offer allocations.
ms.assetid: 96f8b4fd-05e2-4250-8492-f861793d0b12
ms.author: windowsdriverdev
ms.date: 
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: D3DDDICB_OFFERALLOCATIONS2, D3DDDICB_OFFERALLOCATIONS2, 
req.header: d3dumddi.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.ddi-compliance:
req.unicode-ansi:
req.max-support:
req.typenames: D3DDDICB_OFFERALLOCATIONS2
topic_type: 
-	apiref
api_type: 
-	HeaderDef
api_location: 
-	d3dumddi.h
api_name: 
-	D3DDDICB_OFFERALLOCATIONS2
product:
-	Windows
targetos: Windows
---

# D3DDDICB_OFFERALLOCATIONS2 structure

## -description

Used to offer allocations.

## -struct-fields

### -field pResources

An array of Direct3D runtime resource handles.

### -field HandleList

[in] An array of D3DKMT_HANDLE data types that represent kernel-mode handles to the allocations.

### -field NumAllocations

[in] The number of elements in the allocation list.

### -field Priority

The priority of the allocations.

### -field Flags
 
Flags used to offer allocations.

## -remarks

## -see-also