---
UID: NF:winfax.FaxGetDeviceStatusW
title: FaxGetDeviceStatusW function
author: windows-sdk-content
description: The FaxGetDeviceStatus function returns to a fax client application current status information for the fax device of interest.
old-location: fax\_mfax_faxgetdevicestatus.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_1u0j.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FaxGetDeviceStatus, FaxGetDeviceStatus function [Fax Service], FaxGetDeviceStatusA, FaxGetDeviceStatusW, _mfax_faxgetdevicestatus, fax._mfax_faxgetdevicestatus, winfax/FaxGetDeviceStatus, winfax/FaxGetDeviceStatusA, winfax/FaxGetDeviceStatusW
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winfax.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: FaxGetDeviceStatusW (Unicode) and FaxGetDeviceStatusA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WinFax.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - WinFax.lib
 - WinFax.dll
api_name:
 - FaxGetDeviceStatus
 - FaxGetDeviceStatusA
 - FaxGetDeviceStatusW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# FaxGetDeviceStatusW function


## -description


The <b>FaxGetDeviceStatus</b> function returns to a fax client application current status information for the fax device of interest. The returned data includes, among other items, device and station identifiers, sender and recipient names, and routing information.


## -parameters




### -param FaxPortHandle [in]

Type: <b>HANDLE</b>

Specifies a fax port handle returned by a call to the <a href="https://msdn.microsoft.com/9010d651-3259-40b2-91bf-de0a841207c1">FaxOpenPort</a> function.


### -param DeviceStatus [out]

Type: <b>PFAX_DEVICE_STATUS*</b>

Pointer to the address of a buffer to receive a <a href="https://msdn.microsoft.com/34031249-6111-4d5f-bd1c-f4932188ecdb">FAX_DEVICE_STATUS</a> structure. The structure describes the status of one fax device. For information about memory allocation, see the following Remarks section


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. GetLastError can return one of the following errors.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
One or both of the <i>DeviceStatus</i> or <i>FaxPortHandle</i> parameters are <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
Access is denied. <a href="https://msdn.microsoft.com/7d6ff208-33e4-42b2-ae21-76ec8ff58809">FAX_PORT_QUERY</a> access is required.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
An error occurred during memory allocation.

</td>
</tr>
</table>
 




## -remarks



A fax administration application typically calls the <b>FaxGetDeviceStatus</b> function to display the status of a fax device associated with a fax server. The <b>FaxGetDeviceStatus</b> function allocates the memory required for the <a href="https://msdn.microsoft.com/34031249-6111-4d5f-bd1c-f4932188ecdb">FAX_DEVICE_STATUS</a> buffer pointed to by the <i>DeviceStatus</i> parameter. An application must call the <a href="https://msdn.microsoft.com/9a7eedc8-e00f-40e8-a9f4-8e919012ed47">FaxFreeBuffer</a> function to deallocate the resources associated with this parameter.

For more information, see <a href="https://msdn.microsoft.com/784fdc0e-c664-4ea9-8a4f-0a0cd89c0d81">Fax Device Management</a> and <a href="https://msdn.microsoft.com/a8371d98-8a66-484a-9179-4894ae0a7dfc">Freeing Fax Resources</a>.




## -see-also




<a href="https://msdn.microsoft.com/34031249-6111-4d5f-bd1c-f4932188ecdb">FAX_DEVICE_STATUS</a>



<a href="https://msdn.microsoft.com/b076b5ba-09af-4312-90c1-27abd0b859df">Fax Service Client API Functions</a>



<a href="https://msdn.microsoft.com/cbc79dc5-d0ca-418d-8572-64b0a582056f">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/9a7eedc8-e00f-40e8-a9f4-8e919012ed47">FaxFreeBuffer</a>



<a href="https://msdn.microsoft.com/9010d651-3259-40b2-91bf-de0a841207c1">FaxOpenPort</a>
 

 

