---
UID: NC:d3dkmthk.PFND3DKMT_DESTROYALLOCATION
title: PFND3DKMT_DESTROYALLOCATION
author: windows-driver-content
description: The PFND3DKMT_DESTROYALLOCATION callback function releases allocations.
ms.assetid: cad9c963-924a-427a-886c-62e0541c0caa
ms.author: windowsdriverdev
ms.date: 
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: d3dkmthk.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.irql: 
req.ddi-compliance:
req.unicode-ansi:
req.idl:
req.max-support:
req.namespace:
req.assembly:
req.type-library: 
topic_type: 
-	apiref
api_type: 
-	UserDefined
api_location: 
-	d3dkmthk.h
api_name: 
-	PFND3DKMT_DESTROYALLOCATION
product:
-	Windows
targetos: Windows
---

# PFND3DKMT_DESTROYALLOCATION callback function

## -description

The PFND3DKMT_DESTROYALLOCATION callback function releases allocations.

## -prototype

```
//Declaration

PFND3DKMT_DESTROYALLOCATION Pfnd3dkmtDestroyallocation; 

// Definition

NTSTATUS Pfnd3dkmtDestroyallocation 
(
	const D3DKMT_DESTROYALLOCATION *
)
{...}

```

## -parameters

### -param *

Pointer to a [D3DKMT_DESTROYALLOCATION](ns-d3dkmthk-_d3dkmt_destroyallocation.md) structure.

## -returns

Returns NTSTATUS.