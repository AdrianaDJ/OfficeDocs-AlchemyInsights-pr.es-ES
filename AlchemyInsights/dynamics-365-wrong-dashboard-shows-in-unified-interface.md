---
title: Dynamics 365-se muestra un panel incorrecto en la interfaz unificada Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711292"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="c43f6-102">Se muestra un panel equivocado en la interfaz unificada Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c43f6-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="c43f6-103">Hay varios motivos por los que puede ver un panel diferente del que esperaba:</span><span class="sxs-lookup"><span data-stu-id="c43f6-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="c43f6-104">El usuario ha establecido un panel predeterminado del usuario</span><span class="sxs-lookup"><span data-stu-id="c43f6-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="c43f6-105">Normalmente, puede identificar un panel predeterminado del usuario si el botón **establecer como predeterminado** no se muestra en la barra de comandos del panel.</span><span class="sxs-lookup"><span data-stu-id="c43f6-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="c43f6-106">El panel predeterminado del usuario sobrescribirá el resto de los paneles predeterminados, incluso si el panel predeterminado del usuario no está en la aplicación actual.</span><span class="sxs-lookup"><span data-stu-id="c43f6-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="c43f6-107">Use la siguiente solución alternativa para no desactivar el panel predeterminado.</span><span class="sxs-lookup"><span data-stu-id="c43f6-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="c43f6-108">Cree un nuevo panel personal.</span><span class="sxs-lookup"><span data-stu-id="c43f6-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="c43f6-109">Establecer ese nuevo panel como usuario predeterminado.</span><span class="sxs-lookup"><span data-stu-id="c43f6-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="c43f6-110">Eliminar ese panel.</span><span class="sxs-lookup"><span data-stu-id="c43f6-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="c43f6-111">El panel se establece en el mapa del sitio</span><span class="sxs-lookup"><span data-stu-id="c43f6-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="c43f6-112">Puede que haya establecido un panel predeterminado de la organización seleccionando un panel y eligiendo "establecer como predeterminado" en "personalizar el sistema".</span><span class="sxs-lookup"><span data-stu-id="c43f6-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="c43f6-113">Pero el panel definido en el diseñador de Sitemap tendrá prioridad sobre este panel, si el usuario tiene acceso a él.</span><span class="sxs-lookup"><span data-stu-id="c43f6-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="c43f6-114">Para que los usuarios vean el panel que ha establecido como predeterminado de la organización, puede:</span><span class="sxs-lookup"><span data-stu-id="c43f6-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="c43f6-115">Establecer ese panel en el mapa del sitio</span><span class="sxs-lookup"><span data-stu-id="c43f6-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="c43f6-116">Quitar el acceso al panel definido del mapa del sitio para esos usuarios</span><span class="sxs-lookup"><span data-stu-id="c43f6-116">Remove access to the sitemap defined dashboard for those users</span></span>
