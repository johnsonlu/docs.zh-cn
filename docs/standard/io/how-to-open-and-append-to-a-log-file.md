---
title: "如何：打开并追加到日志文件"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-standard
ms.tgt_pltfrm: 
ms.topic: article
dev_langs:
- csharp
- vb
helpviewer_keywords:
- log files, opening
- streams, opening and appending to log file
- log files, appending to
- I/O [.NET Framework], log files
ms.assetid: 74423362-1721-49cb-aa0a-e04005f72a06
caps.latest.revision: 
author: mairaw
ms.author: mairaw
manager: wpickett
ms.workload:
- dotnet
- dotnetcore
ms.openlocfilehash: 333b20adee4ea2826a1fc6795a39490dca1af843
ms.sourcegitcommit: e7f04439d78909229506b56935a1105a4149ff3d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/23/2017
---
# <a name="how-to-open-and-append-to-a-log-file"></a>如何：打开并追加到日志文件
<xref:System.IO.StreamWriter> 和 <xref:System.IO.StreamReader> 对流执行字符写入和读取操作。 下面的代码示例打开 `log.txt` 文件以供输入，或创建文件（如果尚无文件的话），并将信息追加到文件末尾。 然后，将文件内容写入标准输出以供显示。 作为此示例的替换方法，可以将信息存储为一个字符串或字符串数组，并能使用 <xref:System.IO.File.WriteAllText%2A> 或 <xref:System.IO.File.WriteAllLines%2A> 方法实现相同的功能。  
  
> [!NOTE]
>  Visual Basic 用户可以选择使用 <xref:Microsoft.VisualBasic.Logging.Log> 类或 <xref:Microsoft.VisualBasic.FileIO.FileSystem> 类提供的方法和属性，以创建或写入日志文件。  
  
## <a name="example"></a>示例  
 [!code-csharp[Conceptual.BasicIO.TextFiles#2](../../../samples/snippets/csharp/VS_Snippets_CLR/conceptual.basicio.textfiles/cs/source2.cs#2)]
 [!code-vb[Conceptual.BasicIO.TextFiles#2](../../../samples/snippets/visualbasic/VS_Snippets_CLR/conceptual.basicio.textfiles/vb/source2.vb#2)]  
  
## <a name="see-also"></a>请参阅  
 <xref:System.IO.StreamWriter>  
 <xref:System.IO.StreamReader>  
 <xref:System.IO.File.AppendText%2A?displayProperty=nameWithType>  
 <xref:System.IO.File.OpenText%2A?displayProperty=nameWithType>  
 <xref:System.IO.StreamReader.ReadLine%2A?displayProperty=nameWithType>  
 [如何：枚举目录和文件](../../../docs/standard/io/how-to-enumerate-directories-and-files.md)  
 [如何：对新建的数据文件进行读取和写入](../../../docs/standard/io/how-to-read-and-write-to-a-newly-created-data-file.md)  
 [如何：从文件读取文本](../../../docs/standard/io/how-to-read-text-from-a-file.md)  
 [如何：向文件写入文本](../../../docs/standard/io/how-to-write-text-to-a-file.md)  
 [如何：从字符串中读取字符](../../../docs/standard/io/how-to-read-characters-from-a-string.md)  
 [如何：向字符串写入字符](../../../docs/standard/io/how-to-write-characters-to-a-string.md)  
 [文件和流 I-O](../../../docs/standard/io/index.md)
