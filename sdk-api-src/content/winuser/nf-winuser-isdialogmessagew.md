---
UID: NF:winuser.IsDialogMessageW
title: IsDialogMessageW function
author: windows-sdk-content
description: Determines whether a message is intended for the specified dialog box and, if it is, processes the message.
old-location: dlgbox\isdialogmessage.htm
tech.root: dlgbox
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\dialogboxes\dialogboxreference\dialogboxfunctions\isdialogmessage.htm
ms.author: windowssdkdev
ms.date: 10/30/2018
ms.keywords: IsDialogMessage, IsDialogMessage function [Dialog Boxes], IsDialogMessageA, IsDialogMessageW, _win32_IsDialogMessage, _win32_isdialogmessage_cpp, dlgbox.isdialogmessage, winui._win32_isdialogmessage, winuser/IsDialogMessage, winuser/IsDialogMessageA, winuser/IsDialogMessageW
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
req.unicode-ansi: IsDialogMessageW (Unicode) and IsDialogMessageA (ANSI)
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
 - ext-ms-win-ntuser-dialogbox-l1-1-2.dll
api_name:
 - IsDialogMessage
 - IsDialogMessageA
 - IsDialogMessageW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- IsDialogMessageW
: 
---

# IsDialogMessageW function


## -description


Determines whether a message is intended for the specified dialog box and, if it is, processes the message. 


## -parameters




### -param hDlg [in]

Type: <b>HWND</b>

A handle to the dialog box. 


### -param lpMsg [in]

Type: <b>LPMSG</b>

A pointer to an <a href="https://msdn.microsoft.com/fee176ba-ad07-4145-ab4d-1b8c335fd100">MSG</a> structure that contains the message to be checked. 


## -returns



Type: <b>BOOL</b>

If the message has been processed, the return value is nonzero.

If the message has not been processed, the return value is zero. 




## -remarks



Although the <b>IsDialogMessage</b> function is intended for modeless dialog boxes, you can use it with any window that contains controls, enabling the windows to provide the same keyboard selection as is used in a dialog box. 

When <b>IsDialogMessage</b> processes a message, it checks for keyboard messages and converts them into selections for the corresponding dialog box. For example, the TAB key, when pressed, selects the next control or group of controls, and the DOWN ARROW key, when pressed, selects the next control in a group. 

Because the <b>IsDialogMessage</b> function performs all necessary translating and dispatching of messages, a message processed by <b>IsDialogMessage</b> must not be passed to the <a href="https://msdn.microsoft.com/41c2baf4-6426-4789-919c-ab8ff9be8679">TranslateMessage</a> or <a href="https://msdn.microsoft.com/6d5e2d1d-dcd2-48ce-a8ba-99bd5dbdfb21">DispatchMessage</a> function. 

<b>IsDialogMessage</b> sends <a href="https://msdn.microsoft.com/96d2caee-be6e-46e9-98b3-bffc3af1c003">WM_GETDLGCODE</a> messages to the dialog box procedure to determine which keys should be processed. 

<b>IsDialogMessage</b> can send <a href="https://msdn.microsoft.com/9f00a494-f5a2-4c4e-a9fc-2220d9326eb9">DM_GETDEFID</a> and <a href="https://msdn.microsoft.com/30720fa1-48cb-42d4-8370-87bdbaa34600">DM_SETDEFID</a> messages to the window. These messages are defined in the Winuser.h header file as <a href="https://msdn.microsoft.com/4115c587-fcb4-4170-9948-fe33bcb8742a">WM_USER</a> and <b>WM_USER</b> + 1, so conflicts are possible with application-defined messages having the same values. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/9f00a494-f5a2-4c4e-a9fc-2220d9326eb9">DM_GETDEFID</a>



<a href="https://msdn.microsoft.com/30720fa1-48cb-42d4-8370-87bdbaa34600">DM_SETDEFID</a>



<a href="https://msdn.microsoft.com/07ebee3c-5aa7-4b0d-b6cb-e642e01e1a88">Dialog Boxes</a>



<a href="https://msdn.microsoft.com/6d5e2d1d-dcd2-48ce-a8ba-99bd5dbdfb21">DispatchMessage</a>



<a href="https://msdn.microsoft.com/fee176ba-ad07-4145-ab4d-1b8c335fd100">MSG</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/41c2baf4-6426-4789-919c-ab8ff9be8679">TranslateMessage</a>



<a href="https://msdn.microsoft.com/96d2caee-be6e-46e9-98b3-bffc3af1c003">WM_GETDLGCODE</a>



<a href="https://msdn.microsoft.com/4115c587-fcb4-4170-9948-fe33bcb8742a">WM_USER</a>
 

 

