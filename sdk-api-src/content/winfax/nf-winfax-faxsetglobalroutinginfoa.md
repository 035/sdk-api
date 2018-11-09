---
UID: NF:winfax.FaxSetGlobalRoutingInfoA
title: FaxSetGlobalRoutingInfoA function
author: windows-sdk-content
description: A fax management application calls the FaxSetGlobalRoutingInfo function to modify fax routing method data, such as routing priority, that applies globally to the fax server.
old-location: fax\_mfax_faxsetglobalroutinginfo.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_3jlb.htm
ms.author: windowssdkdev
ms.date: 11/05/2018
ms.keywords: FaxSetGlobalRoutingInfo, FaxSetGlobalRoutingInfo function [Fax Service], FaxSetGlobalRoutingInfoA, FaxSetGlobalRoutingInfoW, _mfax_faxsetglobalroutinginfo, fax._mfax_faxsetglobalroutinginfo, winfax/FaxSetGlobalRoutingInfo, winfax/FaxSetGlobalRoutingInfoA, winfax/FaxSetGlobalRoutingInfoW
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
req.unicode-ansi: FaxSetGlobalRoutingInfoW (Unicode) and FaxSetGlobalRoutingInfoA (ANSI)
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
 - FaxSetGlobalRoutingInfo
 - FaxSetGlobalRoutingInfoA
 - FaxSetGlobalRoutingInfoW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# FaxSetGlobalRoutingInfoA function


## -description


A fax management application calls the <b>FaxSetGlobalRoutingInfo</b> function to modify fax routing method data, such as routing priority, that applies globally to the fax server.


## -parameters




### -param FaxHandle [in]

Type: <b>HANDLE</b>

Specifies a fax server handle returned by a call to the <a href="https://msdn.microsoft.com/8705fb04-1047-4f83-ada9-898024ce719c">FaxConnectFaxServer</a> function.


### -param RoutingInfo [in]

Type: <b>const <a href="https://msdn.microsoft.com/df832bcb-d07f-454b-b571-43854706a6c1">FAX_GLOBAL_ROUTING_INFO</a>*</b>

Pointer to a buffer that contains a <a href="https://msdn.microsoft.com/df832bcb-d07f-454b-b571-43854706a6c1">FAX_GLOBAL_ROUTING_INFO</a> structure.


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
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
Access is denied. <a href="https://msdn.microsoft.com/7d6ff208-33e4-42b2-ae21-76ec8ff58809">FAX_CONFIG_SET</a> access is required.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_DATA</b></dt>
</dl>
</td>
<td width="60%">
The <b>Guid</b> member of the specified <a href="https://msdn.microsoft.com/df832bcb-d07f-454b-b571-43854706a6c1">FAX_GLOBAL_ROUTING_INFO</a> structure does not correspond to an installed fax routing method.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
One or both of the <i>FaxHandle</i> or <i>RoutingInfo</i> parameters are invalid.

</td>
</tr>
</table>
 




## -remarks



An application such as the fax service administration application, a Microsoft Management Console (MMC) snap-in component that manages the specified fax routing method, typically calls the <b>FaxSetGlobalRoutingInfo</b> function.

To retrieve the current global configuration, call the <a href="https://msdn.microsoft.com/776b1a16-9a5f-458b-96ee-b2f41568b7e5">FaxEnumGlobalRoutingInfo</a> function. Call the <a href="https://msdn.microsoft.com/1f78fed5-6b49-4946-8607-f1d7f9052aaa">FaxEnumRoutingMethods</a> function to enumerate the fax routing methods associated with a particular device. For more information, see <a href="https://msdn.microsoft.com/356dda5c-852e-46b7-8fa4-f3a0c62d65cb">Managing Fax Routing Data</a>.




## -see-also




<a href="https://msdn.microsoft.com/df832bcb-d07f-454b-b571-43854706a6c1">FAX_GLOBAL_ROUTING_INFO</a>



<a href="https://msdn.microsoft.com/b076b5ba-09af-4312-90c1-27abd0b859df">Fax Service Client API Functions</a>



<a href="https://msdn.microsoft.com/cbc79dc5-d0ca-418d-8572-64b0a582056f">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/776b1a16-9a5f-458b-96ee-b2f41568b7e5">FaxEnumGlobalRoutingInfo</a>



<a href="https://msdn.microsoft.com/1f78fed5-6b49-4946-8607-f1d7f9052aaa">FaxEnumRoutingMethods</a>
 

 

