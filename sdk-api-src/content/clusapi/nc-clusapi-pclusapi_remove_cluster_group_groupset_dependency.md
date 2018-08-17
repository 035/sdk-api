---
UID: NC:clusapi.PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY
title: PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY
author: windows-sdk-content
description: Removes a groupset from a groupset's dependency expression.
old-location: mscs\removeclustergroupcollectiondependency.htm
old-project: mscs
ms.assetid: 1a9dcc3f-e73a-4f14-a418-b1c62a0c98c2
ms.author: windowssdkdev
ms.date: 06/08/2018
ms.keywords: PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY, PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY callback, PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY callback function [Failover Cluster], clusapi/PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY, mscs.removeclustergroupcollectiondependency
ms.prod: windows
ms.technology: windows-sdk
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
tech.root: 
req.typenames: Sources
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - ClusAPI.h
api_name:
 - PCLUSAPI_REMOVE_CLUSTER_GROUP_GROUPSET_DEPENDENCY
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
the function returns a <a href="https://msdn.microsoft.com/en-us/library/ms681381(v=VS.85).aspx">system error code</a>.



