---
title: "SetNoPchSettings"
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
  - "SetNoPchSettings"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "SetNoPchSettings method"
ms.assetid: 52373c98-ad5e-4e9b-9e0f-9f58ddb2a636
caps.latest.revision: 6
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
# SetNoPchSettings
Sets up a project configuration properties when no precompiled header is used.  
  
## Syntax  
  
```  
  
      function SetNoPchSettings(   
   oProj    
);  
```  
  
#### Parameters  
 `oProj`  
 The selected project.  
  
## Remarks  
 Call this function to configure the project when the project uses no precompiled header settings.  
  
## Example  
 See [SetCommonPchSettings](../ide/setcommonpchsettings.md).  
  
## See Also  
 [Customizing C++ Wizards with Common JScript Functions](../ide/customizing-c---wizards-with-common-jscript-functions.md)   
 [JScript Functions for C++ Wizards](../ide/jscript-functions-for-c---wizards.md)   
 [Creating a Custom Wizard](../ide/creating-a-custom-wizard.md)   
 [Designing a Wizard](../ide/designing-a-wizard.md)   
 [SetCommonPchSettings](../ide/setcommonpchsettings.md)   
 [AddCommonConfig](../ide/addcommonconfig.md)