---
title: Restringir el acceso a SharePoint o OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720699"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="87f79-102">Restringir el acceso a SharePoint o OneDrive</span><span class="sxs-lookup"><span data-stu-id="87f79-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="87f79-103">En SharePoint y OneDrive, se restringe el acceso a elementos como archivos, carpetas y listas al conceder acceso solo a los grupos o usuarios a los que desea tener acceso.</span><span class="sxs-lookup"><span data-stu-id="87f79-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="87f79-104">De forma predeterminada, los permisos de SharePoint se heredan de un nivel superior en la jerarquía.</span><span class="sxs-lookup"><span data-stu-id="87f79-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="87f79-105">Por lo tanto, un archivo hereda sus permisos de la carpeta, que hereda sus permisos de la biblioteca, que hereda sus permisos del sitio.</span><span class="sxs-lookup"><span data-stu-id="87f79-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="87f79-106">Puede compartir a un nivel superior (por ejemplo, compartiendo un sitio completo) y, a continuación, interrumpir la herencia si no desea compartir todos los elementos del sitio.</span><span class="sxs-lookup"><span data-stu-id="87f79-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="87f79-107">Sin embargo, no lo recomendamos porque hace que el mantenimiento de los permisos sea más complejo y confuso en el futuro.</span><span class="sxs-lookup"><span data-stu-id="87f79-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="87f79-108">Esto es lo que puede hacer en su lugar:</span><span class="sxs-lookup"><span data-stu-id="87f79-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="87f79-109">Si, por ejemplo, desea compartir todo el contenido de una carpeta excepto un archivo de la misma, mueva ese archivo a una nueva ubicación que no esté compartida.</span><span class="sxs-lookup"><span data-stu-id="87f79-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="87f79-110">Si tiene dos subcarpetas en una carpeta y desea compartir una subcarpeta con los grupos A y B y permitir que sólo el grupo tenga acceso a la segunda subcarpeta, comparta la carpeta principal con el grupo A y agregue el grupo B a la primera subcarpeta.</span><span class="sxs-lookup"><span data-stu-id="87f79-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="87f79-111">Dejar de compartir un archivo o una carpeta </span><span class="sxs-lookup"><span data-stu-id="87f79-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

