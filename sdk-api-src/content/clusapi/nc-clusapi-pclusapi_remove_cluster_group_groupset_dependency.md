---
UID: NC:clusapi.PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY
title: PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY
author: windows-driver-content
description: Removes a groupset from a groupset's dependency expression.
old-location: mscs\removeclustergroupcollectiondependency.htm
old-project: MsCS
ms.assetid: 1a9dcc3f-e73a-4f14-a418-b1c62a0c98c2
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY, PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY callback, PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY callback function [Failover Cluster], clusapi/PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY, mscs.removeclustergroupcollectiondependency
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2016
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: Sources
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	UserDefined
api_location:
-	ClusAPI.h
api_name:
-	PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
---

# PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY callback function


## -description


Removes a groupset from a groupset's dependency expression.


## -parameters




### -param hGroupSet [in]

The groupset from which to remove the dependency.


### -param hDependsOn [in]

The collection to remove


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, 
the function returns a <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>.



