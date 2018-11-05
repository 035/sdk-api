---
UID: NF:faxcom.IFaxStatus.get_Send
title: IFaxStatus::get_Send
author: windows-sdk-content
description: Retrieves the Send property for the FaxStatus object of a parent FaxPort object. The Send property is a Boolean value that indicates whether a specified fax port is currently sending a fax.
old-location: fax\_mfax_ifaxstatus_mfax_ifaxstatus_get_send_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_58f8.htm
ms.author: windowssdkdev
ms.date: 10/26/2018
ms.keywords: IFaxStatus interface [Fax Service],Send property, IFaxStatus.Send, IFaxStatus.get_Send, IFaxStatus::Send, IFaxStatus::get_Send, Send property [Fax Service], Send property [Fax Service],IFaxStatus interface, _mfax_ifaxstatus_get_send, fax._mfax_ifaxstatus_get_send, fax._mfax_ifaxstatus_mfax_ifaxstatus_get_send_cpp, faxcom/IFaxStatus::Send, faxcom/IFaxStatus::get_Send, get_Send
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
 - IFaxStatus.Send
 - IFaxStatus.get_Send
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxStatus::get_Send


## -description


Retrieves the <b>Send</b> property for the <a href="https://msdn.microsoft.com/88f02cb1-df32-4fb8-9fe7-6c3abe1948dc">FaxStatus</a> object of a parent <a href="https://msdn.microsoft.com/cc59452b-194e-4a68-955b-ac39cd5325ff">FaxPort</a> object. The <b>Send</b> property is a Boolean value that indicates whether a specified fax port is currently sending a fax. 

This property is read-only.


## -parameters


## -remarks



You can call the <a href="https://msdn.microsoft.com/e7a63893-d8df-4253-80b0-3faab13934fd">IFaxStatus::get_Receive</a> method to determine if a specified port is currently receiving a fax.




## -see-also




<a href="https://msdn.microsoft.com/f564dc20-7c7c-41c3-81a1-2dfc61ee09f1">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/cbc79dc5-d0ca-418d-8572-64b0a582056f">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/abdd91dd-7734-411a-9b7c-0da312269e6d">IFaxPort</a>



<a href="https://msdn.microsoft.com/e61b13b3-d86c-4f95-bf5a-6b0545a76d03">IFaxPorts</a>



<a href="https://msdn.microsoft.com/823cbedb-052a-4ac1-a73c-4bbafeac2523">IFaxStatus</a>



<a href="https://msdn.microsoft.com/e7a63893-d8df-4253-80b0-3faab13934fd">IFaxStatus::get_Receive</a>
 

 

