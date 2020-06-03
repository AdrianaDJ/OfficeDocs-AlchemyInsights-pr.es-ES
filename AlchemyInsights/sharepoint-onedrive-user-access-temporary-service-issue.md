---
title: 'Problemas de rendimiento: SharePoint o OneDrive'
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511165"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="5a30f-102">SharePoint o OneDrive son lentos, inaccesibles o no disponibles para varios usuarios</span><span class="sxs-lookup"><span data-stu-id="5a30f-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="5a30f-103">Si un sitio de OneDrive o SharePoint no está disponible para varios usuarios que anteriormente tenían acceso, es posible que haya un problema de servicio temporal.</span><span class="sxs-lookup"><span data-stu-id="5a30f-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="5a30f-104">[Compruebe el panel de estado del servicio](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5a30f-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="5a30f-105">**Agregar y conceder una licencia al usuario**</span><span class="sxs-lookup"><span data-stu-id="5a30f-105">**Add and license the user**</span></span>

<span data-ttu-id="5a30f-106">Asegúrese de [asignar licencias a los usuarios en Microsoft 365 para empresas](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="5a30f-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="5a30f-107">**Asignar permisos**</span><span class="sxs-lookup"><span data-stu-id="5a30f-107">**Assign Permissions**</span></span>

<span data-ttu-id="5a30f-108">Si al usuario se le ha asignado una licencia de SharePoint y sigue recibiendo un mensaje de acceso denegado, asegúrese de que tiene asignado el [nivel de permisos adecuado](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="5a30f-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="5a30f-109">**Considerar el uso de la característica de solicitud de acceso**</span><span class="sxs-lookup"><span data-stu-id="5a30f-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="5a30f-110">La [característica de solicitud de acceso](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite que las personas soliciten acceso al contenido que actualmente no tiene permiso para ver.</span><span class="sxs-lookup"><span data-stu-id="5a30f-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="5a30f-111">**Permitir el script personalizado puede provocar problemas de denegación de acceso**</span><span class="sxs-lookup"><span data-stu-id="5a30f-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="5a30f-112">Hay algunos escenarios en los que la característica *permitir scripts personalizados* puede presentar un acceso denegado.</span><span class="sxs-lookup"><span data-stu-id="5a30f-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="5a30f-113">Para obtener una lista de características afectadas, consideraciones de seguridad y la posibilidad de deshabilitar la característica.</span><span class="sxs-lookup"><span data-stu-id="5a30f-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="5a30f-114">Visite [permitir o impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="5a30f-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

