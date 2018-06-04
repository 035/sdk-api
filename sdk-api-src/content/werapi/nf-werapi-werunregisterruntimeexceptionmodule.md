---
UID: The unique id of the API.
title: The title of the API.
author: Authoring type of the API(ie windows-driver-content)
description: Description of API
old-location: 
old-project: 
ms.assetid: The MSDN ID of the API
ms.author: The Author of the API
ms.date: The date of API publishing
ms.keywords: 
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: The topic type of the API (ie enum)
req.header: The main header of the API
req.include-header: The included headers of the API
req.target-type: 
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
---

# WerUnregisterRuntimeExceptionModule function


## -description


Removes the registration of your WER exception handler.


## -parameters




### -param pwszOutOfProcessCallbackDll [in]

The name of the exception handler DLL whose registration you want to remove.


### -param pContext [in, optional]

A pointer to arbitrary context information that was passed to the callback.


## -returns



This function returns <b>S_OK</b> on success or an error code on failure, including the following error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WER_E_INVALID_STATE</b></dt>
</dl>
</td>
<td width="60%">
The process state is not valid. For example, the process is in <a href="https://msdn.microsoft.com/9357786c-1992-4e28-ac75-c2dfda1df7f1">application recovery mode</a>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WER_E_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The list of registered runtime exception handlers does not contain the specified exception handler.

</td>
</tr>
</table>
 




## -remarks



To register your runtime exception handler, call the <a href="https://msdn.microsoft.com/b0fb2c0d-cc98-43cc-a508-e80545377b7f">WerRegisterRuntimeExceptionModule</a> function.



