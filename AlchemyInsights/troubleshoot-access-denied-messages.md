---
title: Solucionar problemas de mensajes de acceso denegado
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690800"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="32fb4-102">Solucionar problemas de mensajes de acceso denegado</span><span class="sxs-lookup"><span data-stu-id="32fb4-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="32fb4-103">Si alguien recibe un mensaje "acceso denegado" a una carpeta compartida de SharePoint, es posible que el administrador de la colección de sitios haya habilitado el modo de bloqueo de permisos de usuario de acceso limitado.</span><span class="sxs-lookup"><span data-stu-id="32fb4-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="32fb4-104">Para desactivarlo:</span><span class="sxs-lookup"><span data-stu-id="32fb4-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="32fb4-105">Vaya al sitio, haga clic en el icono configuración y, a continuación, haga clic en **configuración del sitio**.</span><span class="sxs-lookup"><span data-stu-id="32fb4-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="32fb4-106">En **Administración de la colección de sitios**, haga clic en **Características de la colección de sitios**.</span><span class="sxs-lookup"><span data-stu-id="32fb4-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="32fb4-107">Junto a **modo de bloqueo de permisos de usuario de acceso limitado**, haga clic en **desactivar**.</span><span class="sxs-lookup"><span data-stu-id="32fb4-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="32fb4-108">Un mensaje de acceso denegado también puede producirse para carpetas compartidas si el sitio es un sitio de publicación.</span><span class="sxs-lookup"><span data-stu-id="32fb4-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="32fb4-109">Para obtener información, vea [acceso denegado cuando se tiene acceso a una carpeta compartida](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="32fb4-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="32fb4-110">Si un usuario obtuvo un mensaje de "acceso denegado" al intentar ver las solicitudes de acceso, el usuario debe agregarse como administrador de la colección de sitios o como miembro del grupo de propietarios del sitio.</span><span class="sxs-lookup"><span data-stu-id="32fb4-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="32fb4-111">Para obtener más información, consulte [acceso denegado a solicitudes de acceso a la lista de solicitudes](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="32fb4-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="32fb4-112">Si un usuario obtuvo un mensaje de "acceso denegado" después de que se quitó de Active Directory local y después se volvió a agregar, vea [acceso denegado cuando una cuenta de usuario se sincroniza con Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="32fb4-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

