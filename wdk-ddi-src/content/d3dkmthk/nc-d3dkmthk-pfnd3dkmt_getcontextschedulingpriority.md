---
UID: NC:d3dkmthk.PFND3DKMT_GETCONTEXTSCHEDULINGPRIORITY
title: PFND3DKMT_GETCONTEXTSCHEDULINGPRIORITY
author: windows-driver-content
description: The Pfnd3dkmtGetcontextschedulingpriority retrieves the scheduling priority for a device context.
ms.assetid: 37420543-d819-4fa9-b73e-3787db47dce9
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
-	PFND3DKMT_GETCONTEXTSCHEDULINGPRIORITY
product:
-	Windows
targetos: Windows
---

# PFND3DKMT_GETCONTEXTSCHEDULINGPRIORITY callback function

## -description

The Pfnd3dkmtGetcontextschedulingpriority retrieves the scheduling priority for a device context.

## -prototype

```
//Declaration

PFND3DKMT_GETCONTEXTSCHEDULINGPRIORITY Pfnd3dkmtGetcontextschedulingpriority; 

// Definition

NTSTATUS Pfnd3dkmtGetcontextschedulingpriority 
(
	D3DKMT_GETCONTEXTSCHEDULINGPRIORITY *
)
{...}

```

## -parameters

### -param * 

Pointer to a [D3DKMT_GETCONTEXTSCHEDULINGPRIORITY](ns-d3dkmthk-_d3dkmt_getcontextschedulingpriority.md) structure.

## -returns

Returns NTSTATUS.


## -remarks




## -see-also