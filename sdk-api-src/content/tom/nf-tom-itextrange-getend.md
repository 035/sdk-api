---
UID: NF:tom.ITextRange.GetEnd
title: ITextRange::GetEnd
author: windows-sdk-content
description: Gets the end character position of the range.
old-location: controls\ITextRange_GetEnd.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\getend.htm
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: GetEnd, GetEnd method [Windows Controls], GetEnd method [Windows Controls],ITextRange interface, ITextRange interface [Windows Controls],GetEnd method, ITextRange.GetEnd, ITextRange::GetEnd, _win32_ITextRange_GetEnd, _win32_ITextRange_GetEnd_cpp, controls.ITextRange_GetEnd, controls._win32_ITextRange_GetEnd, tom/ITextRange::GetEnd
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - ITextRange.GetEnd
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- COM
: 
- tom.h
: 
- ITextRange.GetEnd
: 
---

# ITextRange::GetEnd


## -description


Gets the end character position of the range.


## -parameters




### -param pcpLim

Type: <b>long*</b>

The end character position. 


## -returns



Type: <b>HRESULT</b>

The method returns an <b>HRESULT</b> value. If the method succeeds, it returns <b>S_OK</b>. If <i>pcpLim</i> is null, the method fails and it returns E_INVALIDARG.




## -remarks



Although a pointer to a range remains valid when the text is edited, this is not the case for the 
				character position. A 
				character position is volatile; that is, it becomes invalid as soon as text is inserted or deleted before the 
				character position. Be careful about using methods that return 
				character position values, especially if the values are to be stored for any duration. 

This method is similar to the <a href="https://msdn.microsoft.com/55c6785f-1e56-4e9d-86bb-d6f963c693b5">ITextRange::GetStart</a> method which gets the start character position of the range.
			




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/55c6785f-1e56-4e9d-86bb-d6f963c693b5">GetStart</a>



<a href="https://msdn.microsoft.com/e19678cb-f951-458c-bf96-de4b123fd63a">ITextRange</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/d84f9fd8-ac3c-4b26-a745-7528c7ba0bb3">SetEnd</a>



<a href="https://msdn.microsoft.com/a15f0334-1a31-4bc3-bc1e-e5cf53112007">Text Object Model</a>
 

 

