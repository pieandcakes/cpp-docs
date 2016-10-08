---
title: "-Oy (Frame-Pointer Omission)"
ms.custom: na
ms.date: 10/03/2016
ms.devlang: 
  - C++
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-cpp
ms.tgt_pltfrm: na
ms.topic: article
H1: /Oy (Frame-Pointer Omission)
ms.assetid: c451da86-5297-4c5a-92bc-561d41379853
caps.latest.revision: 17
manager: ghogen
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# -Oy (Frame-Pointer Omission)
Suppresses creation of frame pointers on the call stack.  
  
## Syntax  
  
```  
/Oy[-]  
```  
  
## Remarks  
 This option speeds function calls, because no frame pointers need to be set up and removed. It also frees one more register, (EBP on the Intel 386 or later) for storing frequently used variables and sub-expressions.  
  
 **/Oy** enables frame-pointer omission and **/Oy-** disables omission. **/Oy** is available only in x86 compilers.  
  
 If your code requires EBP-based addressing, you can specify the **/Oy–** option after the **/Ox** option or use [optimize](../VS_visualcpp/optimize.md) with the "**y**" and **off** arguments to gain maximum optimization with EBP-based addressing. The compiler detects most situations where EBP-based addressing is required (for instance, with the `_alloca` and `setjmp` functions and with structured exception handling).  
  
 The [/Ox (Full Optimization)](../VS_visualcpp/-Ox--Full-Optimization-.md) and [/O1, /O2 (Minimize Size, Maximize Speed)](../VS_visualcpp/-O1---O2--Minimize-Size--Maximize-Speed-.md) options imply **/Oy**. Specifying **/Oy–** after the **/Ox**, **/O1**, or **/O2** option disables **/Oy**, whether it is explicit or implied.  
  
 The **/Oy** compiler option makes using the debugger more difficult because the compiler suppresses frame pointer information. If you specify a debug compiler option ([/Z7, /Zi, /ZI](../VS_visualcpp/-Z7---Zi---ZI--Debug-Information-Format-.md)), we recommend that you specify the **/Oy-** option after any other optimization compiler options.  
  
### To set this compiler option in the Visual Studio development environment  
  
1.  Open the project's **Property Pages** dialog box. For details, see [How to: Open Project Property Pages](../Topic/How%20to:%20Open%20Project%20Property%20Pages.md).  
  
2.  Click the **C/C++** folder.  
  
3.  Click the **Optimization** property page.  
  
4.  Modify the **Omit Frame Pointers** property. This property adds or removes only the **/Oy** option. If you want to add the **/Oy-** option, click **Command Line** and modify **Additional options**.  
  
### To set this compiler option programmatically  
  
-   See <xref:Microsoft.VisualStudio.VCProjectEngine.VCCLCompilerTool.OmitFramePointers?qualifyHint=False>.  
  
## See Also  
 [/O Options (Optimize Code)](../VS_visualcpp/-O-Options--Optimize-Code-.md)   
 [Compiler Options](../VS_visualcpp/Compiler-Options.md)   
 [Setting Compiler Options](../VS_visualcpp/Setting-Compiler-Options.md)