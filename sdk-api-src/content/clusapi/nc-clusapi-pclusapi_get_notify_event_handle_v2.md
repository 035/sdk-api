---
UID: NC:clusapi.PCLUSAPI_GET_NOTIFY_EVENT_HANDLE_V2
title: PCLUSAPI_GET_NOTIFY_EVENT_HANDLE_V2
author: windows-sdk-content
description: Retrieves a handle to a notification event.
old-location: mscs\getnotifyeventhandle.htm
tech.root: MsCS
ms.assetid: DCA68080-B405-47E9-BC35-613EA56D1E59
ms.author: windowssdkdev
ms.date: 09/26/2018
ms.keywords: PCLUSAPI_GET_NOTIFY_EVENT_HANDLE_V2, PCLUSAPI_GET_NOTIFY_EVENT_HANDLE_V2 callback, PCLUSAPI_GET_NOTIFY_EVENT_HANDLE_V2 callback function [Failover Cluster], clusapi/PCLUSAPI_GET_NOTIFY_EVENT_HANDLE_V2, mscs.getnotifyeventhandle
ms.prod: windows
ms.technology: windows-sdk
ms.topic: callback
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012
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
 - UserDefined
api_location:
 - ClusAPI.h
api_name:
 - PCLUSAPI_GET_NOTIFY_EVENT_HANDLE_V2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PCLUSAPI_GET_NOTIFY_EVENT_HANDLE_V2 callback function


## -description


Retrieves a handle to a notification event.


## -parameters




### -param hChange [in]

A handle to the notification port that received the notification event.


### -param lphTargetEvent [out]

The handle to the notification event.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>. 

If the operation fails, the function returns a system error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa369107(v=VS.85).aspx">Failover Cluster Management Function</a>
 

 

