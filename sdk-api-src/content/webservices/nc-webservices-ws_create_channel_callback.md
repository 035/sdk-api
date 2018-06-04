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

# WS_CREATE_CHANNEL_CALLBACK callback function


## -description


Handles the <a href="https://msdn.microsoft.com/4bef6f97-06f1-442a-8b84-869776f0541d">WsCreateChannel</a> call
                for a <a href="https://msdn.microsoft.com/554cc239-feab-4262-9821-6478a3d93ffc">WS_CUSTOM_CHANNEL_BINDING</a>.
            


## -parameters




### -param channelType [in]


                    The message exchange pattern of the channel.
                


                    If the type of channel is not supported by the custom
                    channel implementation,  <b>E_INVALIDARG</b> should be returned.
                


### -param *channelParameters


                    The pointer to the value that was specified by the
                    <a href="https://msdn.microsoft.com/3207c7f0-7f12-4f6b-8ddd-bac9c06ccfbf">WS_CHANNEL_PROPERTY_CUSTOM_CHANNEL_PARAMETERS</a>
                    property when the custom channel is created using <a href="https://msdn.microsoft.com/4bef6f97-06f1-442a-8b84-869776f0541d">WsCreateChannel</a>.
                


                    If the <a href="https://msdn.microsoft.com/3207c7f0-7f12-4f6b-8ddd-bac9c06ccfbf">WS_CHANNEL_PROPERTY_CUSTOM_CHANNEL_PARAMETERS</a>
                    property was not specified, the value will be <b>NULL</b>.
                


### -param channelParametersSize [in]


                    The size in bytes of the value pointed to by channelParameters.
                


                    If the <a href="https://msdn.microsoft.com/3207c7f0-7f12-4f6b-8ddd-bac9c06ccfbf">WS_CHANNEL_PROPERTY_CUSTOM_CHANNEL_PARAMETERS</a>
                    property was not specified, the size will be 0.
                


#### - **channelInstance


                    A pointer to an structure allocated by the callback 
                    that contains the data specific to this channel instance.  This pointer
                    will be passed to all the other channel callbacks
                    for this particular channel instance.
                


                    If this callback is successful, then the <a href="https://msdn.microsoft.com/f1781c50-824e-4b79-91b6-97e31581617a">WS_FREE_CHANNEL_CALLBACK</a>
                    will be used to free the channel instance returned
                    in this parameter.
                


### -param *error [in, optional]


                    Specifies where additional error information should be stored if the function fails.
                


#### - channelInstance


                    A pointer to an structure allocated by the callback 
                    that contains the data specific to this channel instance.  This pointer
                    will be passed to all the other channel callbacks
                    for this particular channel instance.
                


                    If this callback is successful, then the <a href="https://msdn.microsoft.com/f1781c50-824e-4b79-91b6-97e31581617a">WS_FREE_CHANNEL_CALLBACK</a>
                    will be used to free the channel instance returned
                    in this parameter.
                


## -returns



<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">

One or more arguments are invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">

Ran out of memory.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b> Other Errors </b></dt>
</dl>
</td>
<td width="60%">
This function may return other errors not listed above.

</td>
</tr>
</table>
 



