---
UID: NC:d3dkmthk.PFND3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY
title: PFND3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY
author: windows-driver-content
description: The PFND3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY callback function sets the scheduling priority for a device context that is in the same process as other device contexts.
ms.assetid: f449b34a-48be-498b-856b-fd9f2f48008f
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
-	PFND3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY
product:
-	Windows
targetos: Windows
---

# PFND3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY callback function

## -description

The PFND3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY callback function sets the scheduling priority for a device context that is in the same process as other device contexts.

## -prototype

```
//Declaration

PFND3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY Pfnd3dkmtSetcontextinprocessschedulingpriority; 

// Definition

NTSTATUS Pfnd3dkmtSetcontextinprocessschedulingpriority 
(
	const D3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY *
)
{...}

```

## -parameters

### -param * 

Pointer to a [D3DKMT_SETCONTEXTINPROCESSSCHEDULINGPRIORITY](ns-d3dkmthk-_d3dkmt_setcontextinprocessschedulingpriority.md) structure.

## -returns

Returns NTSTATUS.


## -remarks




## -see-also