---
UID: NF:faxcom.IFaxStatus.get_DeviceName
title: IFaxStatus::get_DeviceName
author: windows-sdk-content
description: Retrieves the DeviceName property for the FaxStatus object of a parent FaxPort object. The DeviceName property is a null-terminated string that contains the user-friendly display name for the fax port.
old-location: fax\_mfax_ifaxstatus_mfax_ifaxstatus_get_devicename_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_67mt.htm
ms.author: windowssdkdev
ms.date: 10/26/2018
ms.keywords: DeviceName property [Fax Service], DeviceName property [Fax Service],IFaxStatus interface, IFaxStatus interface [Fax Service],DeviceName property, IFaxStatus.DeviceName, IFaxStatus.get_DeviceName, IFaxStatus::DeviceName, IFaxStatus::get_DeviceName, _mfax_ifaxstatus_get_devicename, fax._mfax_ifaxstatus_get_devicename, fax._mfax_ifaxstatus_mfax_ifaxstatus_get_devicename_cpp, faxcom/IFaxStatus::DeviceName, faxcom/IFaxStatus::get_DeviceName, get_DeviceName
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcom.h
req.include-header: 
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
req.dll: Faxcom.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Faxcom.dll
api_name:
 - IFaxStatus.DeviceName
 - IFaxStatus.get_DeviceName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxStatus::get_DeviceName


## -description


Retrieves the <b>DeviceName</b> property for the <a href="https://msdn.microsoft.com/88f02cb1-df32-4fb8-9fe7-6c3abe1948dc">FaxStatus</a> object of a parent <a href="https://msdn.microsoft.com/cc59452b-194e-4a68-955b-ac39cd5325ff">FaxPort</a> object. The <b>DeviceName</b> property is a null-terminated string that contains the user-friendly display name for the fax port.

This property is read-only.


## -parameters


## -remarks



Note that it is possible for multiple fax ports to have the same user-friendly name. You can use the <a href="https://msdn.microsoft.com/dd6c8cce-b2fd-4c77-8e74-dc1d851c0de6">DeviceId</a> property of a <a href="https://msdn.microsoft.com/88f02cb1-df32-4fb8-9fe7-6c3abe1948dc">FaxStatus</a> object to uniquely identify a fax port, and associate a FaxStatus object with a <a href="https://msdn.microsoft.com/cc59452b-194e-4a68-955b-ac39cd5325ff">FaxPort</a> object.

The <b>IFaxStatus::get_DeviceName</b> method allocates the memory required for the buffer pointed to by the <i>pVal</i> parameter. The client application must call the <a href="8f230ee3-5f6e-4cb9-a910-9c90b754dcd3">SysFreeString</a> function to deallocate the resources associated with this parameter. For more information, see <a href="https://msdn.microsoft.com/a8371d98-8a66-484a-9179-4894ae0a7dfc">Freeing Fax Resources</a>.




## -see-also




<a href="https://msdn.microsoft.com/f564dc20-7c7c-41c3-81a1-2dfc61ee09f1">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/cbc79dc5-d0ca-418d-8572-64b0a582056f">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/abdd91dd-7734-411a-9b7c-0da312269e6d">IFaxPort</a>



<a href="https://msdn.microsoft.com/e61b13b3-d86c-4f95-bf5a-6b0545a76d03">IFaxPorts</a>



<a href="https://msdn.microsoft.com/823cbedb-052a-4ac1-a73c-4bbafeac2523">IFaxStatus</a>



<a href="https://msdn.microsoft.com/dd6c8cce-b2fd-4c77-8e74-dc1d851c0de6">IFaxStatus::get_DeviceId</a>



<a href="8f230ee3-5f6e-4cb9-a910-9c90b754dcd3">SysFreeString</a>
 

 

