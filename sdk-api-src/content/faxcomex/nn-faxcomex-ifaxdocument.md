---
UID: NN:faxcomex.IFaxDocument
title: IFaxDocument
author: windows-sdk-content
description: The IFaxDocument interface defines a messaging object used by a fax client application to compose a fax document and submit it to the fax service for processing.
old-location: fax\_mfax_faxdocument_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_3md0_cpp.htm
ms.author: windowssdkdev
ms.date: 10/26/2018
ms.keywords: IFaxDocument, IFaxDocument interface [Fax Service], IFaxDocument interface [Fax Service],described, _mfax_faxdocument_cpp, fax._mfax_faxdocument_cpp, faxcomex/IFaxDocument
ms.prod: windows
ms.technology: windows-sdk
ms.topic: interface
req.header: faxcomex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fxscomex.dll
api_name:
 - IFaxDocument
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxDocument interface


## -description


The <b>IFaxDocument</b> interface defines a messaging object used by a fax client application to compose a fax document and submit it to the fax service for processing.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IFaxDocument</b> interface inherits from the <a href="ebbff4bc-36b2-4861-9efa-ffa45e013eb5">IDispatch</a> interface. <b>IFaxDocument</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul>

## -members

The <b>IFaxDocument</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4a4d7305-fc92-45ad-a2ff-ae3a6402f76d">ConnectedSubmit</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/4a4d7305-fc92-45ad-a2ff-ae3a6402f76d">IFaxDocument::ConnectedSubmit</a> method submits a single fax document to the connected <a href="https://msdn.microsoft.com/9e8718b9-f957-43c4-92de-f320aa42a096">IFaxServer</a>. The method returns an array of fax job ID strings, one for each recipient of the fax.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/46dab8a7-157a-4869-b64e-2eebca19bdae">Submit</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/46dab8a7-157a-4869-b64e-2eebca19bdae">IFaxDocument::Submit</a> method submits a single fax document to the fax service for processing.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IFaxDocument</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="10%">Access type</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/72801d0e-49a3-4d0f-92d9-eca2a63f8a3e">AttachFaxToReceipt</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/72801d0e-49a3-4d0f-92d9-eca2a63f8a3e">IFaxDocument::get_AttachFaxToReceipt</a> property indicates whether to attach a fax to the receipt.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/02338d62-234d-4fd9-a136-24dbcab16f88">Body</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/02338d62-234d-4fd9-a136-24dbcab16f88">IFaxDocument::get_Body</a> property provides the path to the file that comprises the body of a fax. The body of a fax consists of the fax pages other than the cover page.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/27d1dd9e-6e50-4beb-96f0-b5c536f6a285">CoverPage</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/27d1dd9e-6e50-4beb-96f0-b5c536f6a285">IFaxDocument::get_CoverPage</a> property is a null-terminated string that contains the name of the cover page template file (.cov) to associate with the fax document.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/ca6b43c6-7b06-448c-b715-3c92a5c4a853">CoverPageType</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/ca6b43c6-7b06-448c-b715-3c92a5c4a853">IFaxDocument::get_CoverPageType</a> property is a value from an enumeration that indicates whether a specified cover page template file (.cov) is a server-based cover page file or a local-computer-based cover page file. You can also specify that no file is used.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/f95352b8-6f19-47b2-907a-5835568799ac">DocumentName</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/f95352b8-6f19-47b2-907a-5835568799ac">IFaxDocument::get_DocumentName</a> property is a null-terminated string that contains the user-friendly name to display for the fax document. The value is for display purposes only.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/24e949f3-d348-479f-8635-9d06514ab420">GroupBroadcastReceipts</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/24e949f3-d348-479f-8635-9d06514ab420">IFaxDocument::get_GroupBroadcastReceipts</a> property is a Boolean value that indicates whether to send an individual delivery receipt for each recipient of the broadcast, or to send a summary receipt for all the recipients.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/54d3f46c-0fb0-42d0-a3b0-a7e01feb52e1">Note</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/54d3f46c-0fb0-42d0-a3b0-a7e01feb52e1">IFaxDocument::get_Note</a> property is a null-terminated string that contains the contents of the note field on the cover page of the fax.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/4f7ebcad-ff7d-4c11-b4c4-c7325415231e">Priority</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/4f7ebcad-ff7d-4c11-b4c4-c7325415231e">IFaxDocument::get_Priority</a> property specifies the priority to use when sending the fax; for example, normal, low, or high priority.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/aa704480-0db8-4b06-9443-74b4d5981fd8">ReceiptAddress</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/aa704480-0db8-4b06-9443-74b4d5981fd8">IFaxDocument::get_ReceiptAddress</a> property is a null-terminated string that indicates the email address to which the fax service should send a delivery receipt when the fax job reaches a final state.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/ee8f9070-7f00-4bd4-8022-1d9b00f1bdaa">ReceiptType</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/ee8f9070-7f00-4bd4-8022-1d9b00f1bdaa">IFaxDocument::get_ReceiptType</a> property specifies the type of delivery receipt to deliver when the fax job reaches a final state.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/d8db3aa4-7c77-40e4-a3d3-a685097fa157">Recipients</a>


</td>
<td align="left" width="10%">
Read-only

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/d8db3aa4-7c77-40e4-a3d3-a685097fa157">IFaxDocument::get_Recipients</a> property retrieves a collection of one or more recipients for the fax document.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/1c8f5adf-9c94-4c4b-9a9a-e8377682f6f9">ScheduleTime</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/1c8f5adf-9c94-4c4b-9a9a-e8377682f6f9">IFaxDocument::get_ScheduleTime</a> property indicates the time to submit the fax for processing to the fax service.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/cbcfcdb1-de89-4e74-8f69-b25d4813f28d">ScheduleType</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/cbcfcdb1-de89-4e74-8f69-b25d4813f28d">IFaxDocument::get_ScheduleType</a> property indicates when to schedule the fax job; for example, you can specify that the fax service send the fax immediately, at a specified time, or during a predefined discount period.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/bd25ee23-284a-4d2f-83e6-1926a15dd2b5">Sender</a>


</td>
<td align="left" width="10%">
Read-only

</td>
<td align="left" width="63%">
Retrieves an object containing information about the sender of the fax document.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/6e1caac1-eead-4061-b7a0-4be92c098d4e">Subject</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/6e1caac1-eead-4061-b7a0-4be92c098d4e">IFaxDocument::get_Subject</a> property is a null-terminated string that contains the contents of the subject field on the cover page of the fax.

</td>
</tr>
</table> 


## -remarks



A default implementation of <b>IFaxDocument</b> and <a href="https://msdn.microsoft.com/20b98e3e-3126-4be1-b9af-228164d0bda6">IFaxDocument2</a> is provided as the <a href="https://msdn.microsoft.com/a87e6de7-1541-4f9e-b411-d8c6907bf93e">FaxDocument</a> object.




## -see-also




<a href="https://msdn.microsoft.com/a87e6de7-1541-4f9e-b411-d8c6907bf93e">FaxDocument</a>



<a href="ebbff4bc-36b2-4861-9efa-ffa45e013eb5">IDispatch</a>
 

 

