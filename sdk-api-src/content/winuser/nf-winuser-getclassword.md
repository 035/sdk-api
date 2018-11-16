---
UID: NF:winuser.GetClassWord
title: GetClassWord function
author: windows-sdk-content
description: Retrieves the 16-bit (WORD) value at the specified offset into the extra class memory for the window class to which the specified window belongs.
old-location: winmsg\getclassword.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\windowclasses\windowclassreference\windowclassfunctions\getclassword.htm
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: GCW_ATOM, GetClassWord, GetClassWord function [Windows and Messages], _win32_GetClassWord, _win32_getclassword_cpp, winmsg.getclassword, winui._win32_getclassword, winuser/GetClassWord
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winuser.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - User32.dll
 - ext-ms-win-ntuser-windowclass-l1-1-2.dll
api_name:
 - GetClassWord
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- GetClassWord
: 
---

# GetClassWord function


## -description


Retrieves the 16-bit (<b>WORD</b>) value at the specified offset into the extra class memory for the window class to which the specified window belongs. 
		
<div class="alert"><b>Note</b>  This function is deprecated for any use other than <i>nIndex</i> set to <b>GCW_ATOM</b>. The function is provided only for compatibility with 16-bit versions of Windows. Applications should use the <a href="https://msdn.microsoft.com/8d8e0b2e-635f-4612-8279-a07679c9a144">GetClassLongPtr</a> or <a href="https://msdn.microsoft.com/73805362-fd27-458c-ac8f-8ea0cab5f311">GetClassLongPtr</a> function.</div><div> </div>

## -parameters




### -param hWnd [in]

Type: <b>HWND</b>

A handle to the window and, indirectly, the class to which the window belongs. 


### -param nIndex [in]

Type: <b>int</b>

The zero-based byte offset of the value to be retrieved. Valid values are in the range zero through the number of bytes of class memory, minus two; for example, if you specified 10 or more bytes of extra class memory, a value of eight would be an index to the fifth 16-bit integer. There is an additional valid value as shown in the following table. 

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="GCW_ATOM"></a><a id="gcw_atom"></a><dl>
<dt><b>GCW_ATOM</b></dt>
<dt>-32</dt>
</dl>
</td>
<td width="60%">
Retrieves an <b>ATOM</b> value that uniquely identifies the window class. This is the same atom that the <a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a> or <a href="https://msdn.microsoft.com/f48ba5a5-08c7-4d16-bc25-e028ea9a73f4">RegisterClassEx</a> function returns.

</td>
</tr>
</table>
 


## -returns



Type: <strong>Type: <b>WORD</b>
</strong>

If the function succeeds, the return value is the requested 16-bit value.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. 




## -remarks



Reserve extra class memory by specifying a nonzero value in the 
				<b>cbClsExtra</b> member of the <a href="https://msdn.microsoft.com/7e2a4e89-19b6-4ef7-81dd-f44a3874e546">WNDCLASS</a> structure used with the <a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a> function. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/8d8e0b2e-635f-4612-8279-a07679c9a144">GetClassLong</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a>



<a href="https://msdn.microsoft.com/f48ba5a5-08c7-4d16-bc25-e028ea9a73f4">RegisterClassEx</a>



<a href="https://msdn.microsoft.com/7d7fb3ac-702f-4fef-b94e-5b38537b98b5">SetClassWord</a>



<a href="https://msdn.microsoft.com/7e2a4e89-19b6-4ef7-81dd-f44a3874e546">WNDCLASS</a>



<a href="https://msdn.microsoft.com/6ef633db-af76-42d6-b211-96846578eaac">Window Classes</a>
 

 

