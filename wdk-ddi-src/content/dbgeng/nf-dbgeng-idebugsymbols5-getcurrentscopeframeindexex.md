---
UID: NF:dbgeng.IDebugSymbols5.GetCurrentScopeFrameIndexEx
title: IDebugSymbols5::GetCurrentScopeFrameIndexEx
author: windows-driver-content
description: Gets the index of the current frame.
old-location: debugger\idebugsymbols5_getcurrentscopeframeindexex.htm
tech.root: debugger
ms.assetid: 0D8198BB-583F-4828-8131-61EB17621F32
ms.author: windowsdriverdev
ms.date: 5/3/2018
ms.keywords: GetCurrentScopeFrameIndexEx, GetCurrentScopeFrameIndexEx method [Windows Debugging], GetCurrentScopeFrameIndexEx method [Windows Debugging],IDebugSymbols5 interface, IDebugSymbols5 interface [Windows Debugging],GetCurrentScopeFrameIndexEx method, IDebugSymbols5.GetCurrentScopeFrameIndexEx, IDebugSymbols5::GetCurrentScopeFrameIndexEx, dbgeng/IDebugSymbols5::GetCurrentScopeFrameIndexEx, debugger.idebugsymbols5_getcurrentscopeframeindexex
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dbgeng.h
req.include-header: Dbgeng.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Dbgeng.h
api_name:
-	IDebugSymbols5.GetCurrentScopeFrameIndexEx
product:
- Windows
targetos: Windows
req.typenames: 
---

# IDebugSymbols5::GetCurrentScopeFrameIndexEx


## -description


Gets the index of the current frame.


## -parameters




### -param Flags [in]

A bit-set that contains options that affect the behavior of this method. 


### -param Index [out]

A pointer to an index that this function gets.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/0D239C0E-96C8-49F9-BDFD-182F3F7C3976">IDebugSymbols5</a>
 

 

