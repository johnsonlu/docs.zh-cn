---
title: "如何：指定专用存储字段"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-ado
ms.tgt_pltfrm: 
ms.topic: article
ms.assetid: 5a40e816-cc6e-43a0-b32a-9caaa0ab6912
caps.latest.revision: "2"
author: douglaslMS
ms.author: douglasl
manager: craigg
ms.workload: dotnet
ms.openlocfilehash: bdb25f21a94ac6eb521e08688e33903e8891caf4
ms.sourcegitcommit: ed26cfef4e18f6d93ab822d8c29f902cff3519d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2018
---
# <a name="how-to-specify-private-storage-fields"></a>如何：指定专用存储字段
使用[!INCLUDE[vbtecdlinq](../../../../../../includes/vbtecdlinq-md.md)]<xref:System.Data.Linq.Mapping.DataAttribute.Storage%2A>属性<xref:System.Data.Linq.Mapping.DataAttribute>特性来指定基础存储字段的名称。  
  
 有关代码示例，请参见<xref:System.Data.Linq.Mapping.DataAttribute.Storage%2A>。  
  
### <a name="to-specify-the-name-of-an-underlying-storage-field"></a>指定基础存储字段的名称  
  
1.  将 <xref:System.Data.Linq.Mapping.DataAttribute.Storage%2A> 属性 (Property) 添加到 <xref:System.Data.Linq.Mapping.ColumnAttribute> 属性 (Attribute)。  
  
2.  指定字段的名称作为 <xref:System.Data.Linq.Mapping.DataAttribute.Storage%2A> 属性的值。  
  
## <a name="see-also"></a>请参阅  
 [LINQ to SQL 对象模型](../../../../../../docs/framework/data/adonet/sql/linq/the-linq-to-sql-object-model.md)  
 [如何：通过使用代码编辑器自定义实体类](../../../../../../docs/framework/data/adonet/sql/linq/how-to-customize-entity-classes-by-using-the-code-editor.md)
