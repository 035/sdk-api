---
UID: NF:winuser.IsIconic
title: IsIconic function
author: windows-sdk-content
description: Determines whether the specified window is minimized (iconic).
old-location: winmsg\isiconic.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\windows\windowreference\windowfunctions\isiconic.htm
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: IsIconic, IsIconic function [Windows and Messages], _win32_IsIconic, _win32_isiconic_cpp, winmsg.isiconic, winui._win32_isiconic, winuser/IsIconic
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
 - Ext-MS-Win-NTUser-Window-l1-1-0.dll
 - Ext-MS-Win-NTUser-Window-l1-1-1.dll
 - Ext-MS-Win-NTUser-Window-l1-1-2.dll
 - ext-ms-win-ntuser-window-l1-1-3.dll
 - Ext-MS-Win-NTUser-Window-L1-1-4.dll
api_name:
 - IsIconic
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- IsIconic
: 
---

# IsIconic function


## -description


Determines whether the specified window is minimized (iconic).


## -parameters




### -param hWnd [in]

Type: <b>HWND</b>

A handle to the window to be tested.


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the window is iconic, the return value is nonzero.

If the window is not iconic, the return value is zero.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/7eece45d-5d18-4b1a-947e-1ed76a228bd9">IsZoomed</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/e2c778c7-7319-4bf7-a6a7-b526e4f3e98b">Windows</a>
 

 

