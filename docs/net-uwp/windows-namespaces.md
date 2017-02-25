---
title: "Windows namespaces | Microsoft Docs"
ms.custom: ""
ms.date: "12/16/2016"
ms.prod: "windows-client-threshold"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - ".net-for-windows-store-apps"
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 2031b3d9-f45f-44c0-808a-645bf60dd99a
caps.latest.revision: 18
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# Windows namespaces
The `Windows` namespaces (`Windows.Foundation`, `Windows.UI`, `Windows.UI.Xaml`, `Windows.UI.Xaml.Controls.Primitives`, `Windows.UI.Xaml.Media`, `Windows.UI.Xaml.Media.Animation`, and `Windows.UI.Xaml.Media.Media3D`) contain types for managing the user interface of your application.  
  
 This topic displays the types in the `Windows` namespaces that are included in the .NET for Windows 8.x Store apps. Note that the .NET for Windows 8.x Store apps do not include all the members of each type. For information about individual types, see the linked topics. The documentation for a type indicates which members are included in the .NET for Windows 8.x Store apps.  
  
 Windows 8.x Store apps only: APIs for Windows 8.x Store apps that are expressed as HTML or XAML elements are supported only in Windows 8.x Store apps; they are not supported in desktop apps or Windows 8.x Store enabled desktop browsers.  
  
## Windows.Foundation namespace  
  
|Types supported in the .NET for Windows 8.x Store apps|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:Windows.Foundation.Point>|Represents an x- and y-coordinate pair in two-dimensional space. Can also represent a logical point for certain property usages.|  
|<xref:Windows.Foundation.Rect>|(Describes the width, height, and point origin of a rectangle.|  
|<xref:Windows.Foundation.Size>|Describes the width and height of an object.|  
  
## Windows.UI namespace  
  
|Types supported in the .NET for Windows 8.x Store apps|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:Windows.UI.Color>|Describes a color in terms of alpha, red, green, and blue channels.|  
  
## Windows.UI.Xaml namespace  
  
|Types supported in the .NET for Windows 8.x Store apps|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:Windows.UI.Xaml.CornerRadius>|Describes the characteristics of a rounded corner, such as can be applied to a Windows.UI.Xaml.Controls.Border.|  
|<xref:Windows.UI.Xaml.Duration>|Represents the duration of time that a Windows.UI.Xaml.Media.Animation.Timeline is active.|  
|<xref:Windows.UI.Xaml.DurationType>|Specifies whether a Duration has a special value of Automatic or Forever, or has valid information in its TimeSpan component.|  
|<xref:Windows.UI.Xaml.GridLength>|Represents the length of elements that explicitly support Star unit types.|  
|<xref:Windows.UI.Xaml.GridUnitType>|Describes the kind of value that a GridLength object is holding.|  
|<xref:Windows.UI.Xaml.Thickness>|Describes the thickness of a frame around a rectangle. Four Double values describe the Left, Top, Right, and Bottom sides of the rectangle, respectively.|  
  
## Windows.UI.Xaml.Controls.Primitives namespace  
  
|Types supported in the .NET for Windows 8.x Store apps|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:Windows.UI.Xaml.Controls.Primitives.GeneratorPosition>|Used to describe the position of an item that is managed by Windows.UI.Xaml.Controls.ItemContainerGenerator.|  
  
## Windows.UI.Xaml.Media namespace  
  
|Types supported in the .NET for Windows 8.x Store apps|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:Windows.UI.Xaml.Media.Matrix>|Represents a 3x3 affine transformation matrix used for transformations in two-dimensional space.|  
  
## Windows.UI.Xaml.Media.Animation namespace  
  
|Types supported in the .NET for Windows 8.x Store apps|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:Windows.UI.Xaml.Media.Animation.KeyTime>|Specifies when a particular key frame should take place during an animation.|  
|<xref:Windows.UI.Xaml.Media.Animation.RepeatBehavior>|Describes how a Windows.UI.Xaml.Media.Animation.Timeline repeats its simple duration.|  
|<xref:Windows.UI.Xaml.Media.Animation.RepeatBehaviorType>|Specifies the repeat mode that a RepeatBehavior raw value represents.|  
  
## Windows.UI.Xaml.Media.Media3D namespace  
  
|Types supported in the .NET for Windows 8.x Store apps|Description|  
|---------------------------------------------------------------------------------------------|-----------------|  
|<xref:Windows.UI.Xaml.Media.Media3D.Matrix3D>|Represents a 4 × 4 matrix that is used for transformations in a three-dimensional (3-D) space.|  
  
## See Also  
 [.NET for Windows apps](../net-uwp/dotnet-for-windows-apps.md)