---
title: "&lt;qualifyAssembly&gt;元素"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: article
f1_keywords:
- http://schemas.microsoft.com/.NetConfiguration/v2.0#qualifyAssembly
- http://schemas.microsoft.com/.NetConfiguration/v2.0#configuration/runtime/assemblyBinding/qualifyAssembly
helpviewer_keywords:
- container tags, <qualifyAssembly> element
- <qualifyAssembly> element
- qualifyAssembly element
ms.assetid: ad6442f6-1a9d-43b6-b733-04ac1b7f9b82
caps.latest.revision: "13"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.workload: dotnet
ms.openlocfilehash: 7dd24ae9e5659deff7ddbe4183c70d5b442542cd
ms.sourcegitcommit: c0dd436f6f8f44dc80dc43b07f6841a00b74b23f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2018
---
# <a name="ltqualifyassemblygt-element"></a>&lt;qualifyAssembly&gt;元素
指定使用部分名称时应动态加载的程序集全名。  
  
 \<configuration>  
\<runtime>  
\<assemblyBinding>  
\<qualifyAssembly>  
  
## <a name="syntax"></a>语法  
  
```xml  
      <qualifyAssembly partialName=  
      "PartialAssemblyName"  
                 fullName="FullAssemblyName"/>  
```  
  
## <a name="attributes-and-elements"></a>特性和元素  
 下列各节描述了特性、子元素和父元素。  
  
### <a name="attributes"></a>特性  
  
|特性|描述|  
|---------------|-----------------|  
|`partialName`|必需的特性。<br /><br /> 指定程序集的部分名称，在代码中所示。|  
|`fullName`|必需的特性。<br /><br /> 指定的程序集的完整名称，在全局程序集缓存中所示。|  
  
### <a name="child-elements"></a>子元素  
 无。  
  
### <a name="parent-elements"></a>父元素  
  
|元素|描述|  
|-------------|-----------------|  
|`assemblyBinding`|包含有关程序集版本重定向和程序集位置的信息。|  
|`configuration`|公共语言运行时和 .NET Framework 应用程序所使用的每个配置文件中的根元素。|  
|`runtime`|包含有关程序集绑定和垃圾回收的信息。|  
  
## <a name="remarks"></a>备注  
 调用<xref:System.Reflection.Assembly.Load%2A?displayProperty=nameWithType>使用部分程序集名称的方法使公共语言运行时查找仅在应用程序基目录中的程序集。 使用 **\<qualifyAssembly >**中应用程序配置文件可提供完整的程序集信息 （名称、 版本、 公钥标记和区域性） 并且使公共语言运行时，要搜索的元素全局程序集缓存中程序集。  
  
 **FullName**属性必须包含程序集标识的四个字段： 名称、 版本、 公钥标记和区域性。 **PartialName**属性部分必须引用的程序集。 你必须至少指定程序集的文本名称 （最常见的情况），但你也可以包括版本、 公钥标记或区域性 （或四个，但并非所有四个的任意组合）。 **PartialName**必须匹配你调用中指定的名称。 例如，不能指定`"math"`作为**partialName**中你的配置文件和调用属性`Assembly.Load("math, Version=3.3.3.3")`在代码中。  
  
## <a name="example"></a>示例  
 下面的示例以逻辑方式调用变成`Assembly.Load("math")`到`Assembly.Load("math,version=1.0.0.0,publicKeyToken=a1690a5ea44bab32,culture=neutral")`。  
  
```xml  
<configuration>  
   <runtime>  
      <assemblyBinding xmlns="urn:schemas-microsoft-com:asm.v1">  
         <qualifyAssembly partialName="math"   
                         fullName=  
"math,version=1.0.0.0,publicKeyToken=a1690a5ea44bab32,culture=neutral"/>  
      </assemblyBinding>  
   </runtime>  
</configuration>  
```  
  
## <a name="see-also"></a>请参阅  
 [运行时设置架构](../../../../../docs/framework/configure-apps/file-schema/runtime/index.md)  
 [运行时如何定位程序集](../../../../../docs/framework/deployment/how-the-runtime-locates-assemblies.md)  
 [NIB： 部分程序集引用](http://msdn.microsoft.com/library/ec90f07a-398c-4306-9401-0fc5ff9cb59f)
