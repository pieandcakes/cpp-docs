---
title: "SetErrorInfo"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "SetErrorInfo"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "SetErrorInfo method"
ms.assetid: 78bca763-3f90-4e04-b566-b4b7fe2431b1
caps.latest.revision: 7
ms.author: "mblome"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# SetErrorInfo
Called by [OnWizFinish](../ide/onwizfinish.md) and [CanUseFileName](../ide/canusefilename.md) to provide current error information.  
  
## Syntax  
  
```  
  
      function SetErrorInfo(   
   oErrorObj   
);  
```  
  
#### Parameters  
 *oErrorObj*  
 The error object.  
  
## Remarks  
 Called by [OnWizFinish](../ide/onwizfinish.md) and [CanUseFileName](../ide/canusefilename.md) to provide current error information. See \<xref:Microsoft.VisualStudio.VsWizard.VCWizCtlClass.SetErrorInfo*> in the Visual C++ Wizard Model documentation for more information.  
  
## See Also  
 [Customizing C++ Wizards with Common JScript Functions](../ide/customizing-c---wizards-with-common-jscript-functions.md)   
 [JScript Functions for C++ Wizards](../ide/jscript-functions-for-c---wizards.md)   
 [Creating a Custom Wizard](../ide/creating-a-custom-wizard.md)   
 [Designing a Wizard](../ide/designing-a-wizard.md)