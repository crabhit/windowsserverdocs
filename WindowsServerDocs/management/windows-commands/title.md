---
title: title
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: c0bbe8bd-201a-4b6c-b617-5d9809881dc8
author: jaimeo
---
# title
creates a title for the Command prompt window.  
  
for examples of how to use this command, see [Examples](#BKMK_examples).  
  
## Syntax  
  
```  
title [<String>]  
```  
  
## Parameters  
  
|Parameter|Description|  
|-------------|---------------|  
|<String>|Specifies the title of the Command prompt window.|  
|\/?|Displays help at the command prompt.|  
  
## remarks  
  
-   To create window title for batch programs, include the **title** command at the beginning of a batch program.  
  
-   After a window title is set, you can reset it only by using the **title** command.  
  
## <a name="BKMK_examples"></a>Examples  
In the following sample script, the title of the Command prompt window is changed to "Updating Files" while the batch file executes the **copy** command. After the command is executed, the text `Files Updated` is displayed, and the title of the Command prompt window is changed back to "Command prompt."  
  
```  
@echo off  
title Updating Files  
copy \\server\share\*.xls c:\users\common\*.xls  
echo Files Updated.  
title Command prompt  
```  
  
#### additional references  
[Command-Line Syntax Key](commandline-syntax-key.md)  
  
