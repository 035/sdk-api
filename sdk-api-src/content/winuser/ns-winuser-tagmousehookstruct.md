---
UID: NS:winuser.tagMOUSEHOOKSTRUCT
title: tagMOUSEHOOKSTRUCT
author: windows-sdk-content
description: Contains information about a mouse event passed to a WH_MOUSE hook procedure, MouseProc.
old-location: winmsg\mousehookstruct.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\hooks\hookreference\hookstructures\mousehookstruct.htm
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: "*LPMOUSEHOOKSTRUCT, *PMOUSEHOOKSTRUCT, LPMOUSEHOOKSTRUCT, LPMOUSEHOOKSTRUCT structure pointer [Windows and Messages], MOUSEHOOKSTRUCT, MOUSEHOOKSTRUCT structure [Windows and Messages], PMOUSEHOOKSTRUCT, PMOUSEHOOKSTRUCT structure pointer [Windows and Messages], _win32_MOUSEHOOKSTRUCT_str, _win32_mousehookstruct_str_cpp, tagMOUSEHOOKSTRUCT, winmsg.mousehookstruct, winui._win32_mousehookstruct_str, winuser/LPMOUSEHOOKSTRUCT, winuser/MOUSEHOOKSTRUCT, winuser/PMOUSEHOOKSTRUCT"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Winuser.h
api_name:
 - MOUSEHOOKSTRUCT
product: Windows
targetos: Windows
req.typenames: MOUSEHOOKSTRUCT, *LPMOUSEHOOKSTRUCT, *PMOUSEHOOKSTRUCT
req.redist: 
---

# tagMOUSEHOOKSTRUCT structure


## -description


Contains information about a mouse event passed to a <b>WH_MOUSE</b> hook procedure, <a href="https://msdn.microsoft.com/4fc1d81d-ee12-4ee4-b29c-2450b92b83b5">MouseProc</a>. 


## -struct-fields




### -field pt

Type: <b><a href="https://msdn.microsoft.com/ecb0f0e1-90c2-48ab-a069-552262b49c7c">POINT</a></b>

The x- and y-coordinates of the cursor, in screen coordinates. 


### -field hwnd

Type: <b>HWND</b>

A handle to the window that will receive the mouse message corresponding to the mouse event. 


### -field wHitTestCode

Type: <b>UINT</b>

The hit-test value. For a list of hit-test values, see the description of the <a href="https://msdn.microsoft.com/4c860466-a9f8-4af8-96b9-cee005481875">WM_NCHITTEST</a> message. 


### -field dwExtraInfo

Type: <b>ULONG_PTR</b>

Additional information associated with the message. 


## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/987095d7-059f-4eae-925d-6723ab6d524c">Hooks</a>



<a href="https://msdn.microsoft.com/4fc1d81d-ee12-4ee4-b29c-2450b92b83b5">MouseProc</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/66c96282-528c-4f57-acab-ae03178e4fe9">SetWindowsHookEx</a>



<a href="https://msdn.microsoft.com/4c860466-a9f8-4af8-96b9-cee005481875">WM_NCHITTEST</a>
 

 

