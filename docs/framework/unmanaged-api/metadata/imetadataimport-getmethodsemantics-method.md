---
title: "IMetaDataImport::GetMethodSemantics 方法"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology:
- dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name:
- IMetaDataImport.GetMethodSemantics
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- IMetaDataImport::GetMethodSemantics
helpviewer_keywords:
- GetMethodSemantics method [.NET Framework metadata]
- IMetaDataImport::GetMethodSemantics method [.NET Framework metadata]
ms.assetid: 5e018eaa-d60e-4a0b-a2c5-8c36bd09d905
topic_type:
- apiref
caps.latest.revision: 
author: mairaw
ms.author: mairaw
manager: wpickett
ms.workload:
- dotnet
ms.openlocfilehash: 8f8921c4f6a676c9647d4e8907a22f0d68b0b359
ms.sourcegitcommit: 16186c34a957fdd52e5db7294f291f7530ac9d24
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2017
---
# <a name="imetadataimportgetmethodsemantics-method"></a>IMetaDataImport::GetMethodSemantics 方法
获取令牌的标志，指示由指定的 MethodDef 标记和与成对的属性引用的方法和事件由指定的 EventProp 引用之间的关系。  
  
## <a name="syntax"></a>语法  
  
```  
HRESULT GetMethodSemantics (  
   [in]  mdMethodDef   mb,  
   [in]  mdToken       tkEventProp,  
   [out] DWORD         *pdwSemanticsFlags  
);  
```  
  
#### <a name="parameters"></a>参数  
 `mb`  
 [in]表示要获取的语义角色信息的方法的 MethodDef 标记。  
  
 `tkEventProp`  
 [in]表示成对的属性和要为其获取方法的角色的事件的标记。  
  
 `pdwSemanticsFlags`  
 [out]指向关联的语义标记的指针。 此值是从一个位掩码[CorMethodSemanticsAttr](../../../../docs/framework/unmanaged-api/metadata/cormethodsemanticsattr-enumeration.md)枚举。  
  
## <a name="remarks"></a>备注  
 [Imetadataemit:: Defineproperty](../../../../docs/framework/unmanaged-api/metadata/imetadataemit-defineproperty-method.md)方法设置方法的语义标志。  
  
## <a name="requirements"></a>惠?  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** Cor.h  
  
 **库：**作为 MsCorEE.dll 中的资源  
  
 **.NET framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [IMetaDataImport 接口](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-interface.md)  
 [IMetaDataImport2 接口](../../../../docs/framework/unmanaged-api/metadata/imetadataimport2-interface.md)
