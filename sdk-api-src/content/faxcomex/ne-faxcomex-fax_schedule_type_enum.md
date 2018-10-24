---
UID: NE:faxcomex.FAX_SCHEDULE_TYPE_ENUM
title: FAX_SCHEDULE_TYPE_ENUM
author: windows-sdk-content
description: The FAX_SCHEDULE_TYPE_ENUM enumeration defines the types of scheduling for outbound faxes.
old-location: fax\_mfax_fax_schedule_type_enum.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_5ust.htm
ms.author: windowssdkdev
ms.date: 10/09/2018
ms.keywords: FAX_SCHEDULE_TYPE_ENUM, FAX_SCHEDULE_TYPE_ENUM enumeration [Fax Service], _mfax_fax_schedule_type_enum, fax._mfax_fax_schedule_type_enum, faxcomex/FAX_SCHEDULE_TYPE_ENUM, faxcomex/fstDISCOUNT_PERIOD, faxcomex/fstNOW, faxcomex/fstSPECIFIC_TIME, fstDISCOUNT_PERIOD, fstNOW, fstSPECIFIC_TIME
ms.prod: windows
ms.technology: windows-sdk
ms.topic: enum
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - FaxComex.h
api_name:
 - FAX_SCHEDULE_TYPE_ENUM
product: Windows
targetos: Windows
req.typenames: FAX_SCHEDULE_TYPE_ENUM
req.redist: 
---

# FAX_SCHEDULE_TYPE_ENUM enumeration


## -description


The <b>FAX_SCHEDULE_TYPE_ENUM</b> enumeration defines the types of scheduling for outbound faxes.


## -enum-fields




### -field fstNOW

Send the fax as soon as a device is available.


### -field fstSPECIFIC_TIME

Send the fax no sooner than the specified time. The actual time that the fax will be sent depends on device availability and fax priority.


### -field fstDISCOUNT_PERIOD

Send the fax during the discount rate period.


## -see-also




<a href="https://msdn.microsoft.com/1c8f5adf-9c94-4c4b-9a9a-e8377682f6f9">IFaxDocument::get_ScheduleTime</a>



<a href="https://msdn.microsoft.com/cbcfcdb1-de89-4e74-8f69-b25d4813f28d">IFaxDocument::get_ScheduleType</a>



<a href="https://msdn.microsoft.com/5bb282da-3226-4c9d-ab75-82a587b0a56f">IFaxOutgoingQueue::get_DiscountRateEnd</a>



<a href="https://msdn.microsoft.com/8df89f09-8fba-4bad-a516-82ab471d189e">IFaxOutgoingQueue::get_DiscountRateStart</a>
 

 

