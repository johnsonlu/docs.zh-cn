---
title: "ICorPublishEnum::GetCount 方法"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorPublishEnum.GetCount
api_location: mscordbi.dll
api_type: COM
f1_keywords: ICorPublishEnum::GetCount
helpviewer_keywords:
- GetCount method, ICorPublishEnum interface [.NET Framework debugging]
- ICorPublishEnum::GetCount method [.NET Framework debugging]
ms.assetid: d228f684-2be3-4029-93ae-31fe02213c1f
topic_type: apiref
caps.latest.revision: "9"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: 7b91c11482a1314bc86b464715dcba68f2a67724
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="icorpublishenumgetcount-method"></a><span data-ttu-id="bd07c-102">ICorPublishEnum::GetCount 方法</span><span class="sxs-lookup"><span data-stu-id="bd07c-102">ICorPublishEnum::GetCount Method</span></span>
<span data-ttu-id="bd07c-103">枚举中获取项的数目。</span><span class="sxs-lookup"><span data-stu-id="bd07c-103">Gets the number of items in the enumeration.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="bd07c-104">语法</span><span class="sxs-lookup"><span data-stu-id="bd07c-104">Syntax</span></span>  
  
```  
HRESULT GetCount (  
    [out] ULONG   *pcelt  
);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="bd07c-105">参数</span><span class="sxs-lookup"><span data-stu-id="bd07c-105">Parameters</span></span>  
 `pcelt`  
 <span data-ttu-id="bd07c-106">[out]一个指向枚举中的项的数目。</span><span class="sxs-lookup"><span data-stu-id="bd07c-106">[out] A pointer to the number of items in the enumeration.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="bd07c-107">要求</span><span class="sxs-lookup"><span data-stu-id="bd07c-107">Requirements</span></span>  
 <span data-ttu-id="bd07c-108">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="bd07c-108">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="bd07c-109">**标头：** CorPub.idl、 CorPub.h</span><span class="sxs-lookup"><span data-stu-id="bd07c-109">**Header:** CorPub.idl, CorPub.h</span></span>  
  
 <span data-ttu-id="bd07c-110">**库：** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="bd07c-110">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="bd07c-111">**.NET framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="bd07c-111">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="bd07c-112">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bd07c-112">See Also</span></span>  
 [<span data-ttu-id="bd07c-113">ICorPublishEnum 接口</span><span class="sxs-lookup"><span data-stu-id="bd07c-113">ICorPublishEnum Interface</span></span>](../../../../docs/framework/unmanaged-api/debugging/icorpublishenum-interface.md)