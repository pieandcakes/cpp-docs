---
title: "-MANIFEST (Create Side-by-Side Assembly Manifest)"
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
H1: /MANIFEST (Create Side-by-Side Assembly Manifest)
ms.assetid: 98c52e1e-712c-4f49-b149-4d0a3501b600
caps.latest.revision: 20
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
# -MANIFEST (Create Side-by-Side Assembly Manifest)
```  
/MANIFEST[:{EMBED[,ID=#]|NO}]  
```  
  
## Remarks  
 /MANIFEST specifies that the linker should create a side-by-side manifest file. For more information about manifest files, see [Manifest Files Reference](http://msdn.microsoft.com/library/aa375632).  
  
 The default is /MANIFEST.  
  
 The /MANIFEST:EMBED option specifies that the linker should embed the manifest file in the image as a resource of type RT_MANIFEST. The optional `ID` parameter is the resource ID to use for the manifest. Use a value of 1 for an executable file. Use a value of 2 for a DLL to enable it to specify private dependencies. If the `ID` parameter is not specified, the default value is 2 if the /DLL option is set; otherwise, the default value is 1.  
  
 Beginning with Visual Studio 2008, manifest files for executables contain a section that specifies User Account Control (UAC) information. If you specify /MANIFEST but specify neither [/MANIFESTUAC](../VS_visualcpp/-MANIFESTUAC--Embeds-UAC-information-in-manifest-.md) nor [/DLL](../VS_visualcpp/-DLL--Build-a-DLL-.md), a default UAC fragment that has the UAC level set to *asInvoker* is inserted into the manifest. For more information about UAC levels, see [/MANIFESTUAC (Embeds UAC information in manifest)](../VS_visualcpp/-MANIFESTUAC--Embeds-UAC-information-in-manifest-.md).  
  
 To change the default behavior for UAC, do one of these:  
  
-   Specify the /MANIFESTUAC option and set the UAC level to the desired value.  
  
-   Or specify the /MANIFESTUAC:NO option if you do not want to generate a UAC fragment in the manifest.  
  
 If you do not specify /MANIFEST but do specify [/MANIFESTDEPENDENCY](../VS_visualcpp/-MANIFESTDEPENDENCY--Specify-Manifest-Dependencies-.md) comments, a manifest file is created. A manifest file is not created if you specify /MANIFEST:NO.  
  
 If you specify /MANIFEST, the name of the manifest file is the same as the name of your output file, but with .manifest appended to the file name. For example, if your output file name is MyFile.exe, the manifest file name is MyFile.exe.manifest.  If you specify /MANIFESTFILE:*name*, the name of the manifest is what you specify in *name*.  
  
### To set this linker option in the Visual Studio development environment  
  
1.  Open the project's **Property Pages** dialog box. For details, see [How to: Open Project Property Pages](../Topic/How%20to:%20Open%20Project%20Property%20Pages.md).  
  
2.  Expand the **Configuration Properties** node.  
  
3.  Expand the **Linker** node.  
  
4.  Select the **Manifest File** property page.  
  
5.  Modify the **Generate Manifest** property.  
  
### To set this linker option programmatically  
  
1.  See <xref:Microsoft.VisualStudio.VCProjectEngine.VCLinkerTool.GenerateManifest?qualifyHint=False>.  
  
## See Also  
 [Setting Linker Options](../VS_visualcpp/Setting-Linker-Options.md)   
 [Linker Options](../VS_visualcpp/Linker-Options.md)