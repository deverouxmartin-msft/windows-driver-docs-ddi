---
UID: NF:dbgmodel.IDebugHostType2.GetGenericArgumentAt
title: IDebugHostType2::GetGenericArgumentAt
author: windows-driver-content
description: For the "i"-th generic argument to the generic/template, this returns a new IDebugHostSymbol  which represents that argument.
ms.assetid: 8038e101-f14b-4762-8deb-6acdc0fe28cc
ms.author: windowsdriverdev
ms.date: 09/20/2018 
ms.topic: method
ms.keywords: IDebugHostType2::GetGenericArgumentAt, GetGenericArgumentAt, IDebugHostType2.GetGenericArgumentAt, IDebugHostType2::GetGenericArgumentAt, IDebugHostType2.GetGenericArgumentAt
req.header: dbgmodel.h
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
-	COM
api_location: 
-	dbgmodel.h
api_name: 
-	IDebugHostType2.GetGenericArgumentAt
product: Windows
targetos: Windows
tech.root: debugger
---

# IDebugHostType2::GetGenericArgumentAt


## -description
For the "i"-th generic argument to the generic/template, this returns a new IDebugHostSymbol  which represents that argument.  For templates, this is most often an IDebugHostType; however --  it may be an IDebugHostConstant for non-template type arguments.  

Note that it is possible for some compiler generated generics and templates that this method  will fail.

## -parameters

### -param i
The zero based index of the generic argument to returned.

### -param argument
The i’th generic argument of the type will be returned here


## -returns
This method returns HRESULT which indicates success or failure.

## -remarks

## -see-also
[IDebugHostType2 interface](nn-dbgmodel-idebughosttype2.md)
