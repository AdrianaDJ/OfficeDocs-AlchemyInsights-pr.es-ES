---
title: Crear un sitio en SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732258"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="ad398-102">Crear sitios de SharePoint con plantillas</span><span class="sxs-lookup"><span data-stu-id="ad398-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="ad398-103">La capacidad de guardar un sitio como plantilla no es compatible con la comunicación o los sitios de grupo modernos.</span><span class="sxs-lookup"><span data-stu-id="ad398-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="ad398-104">Para obtener más información sobre el uso de plantillas [, vea guardar, descargar y cargar un sitio de SharePoint como plantilla](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="ad398-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="ad398-105">Estos son algunos problemas o soluciones comunes en relación con guardar un sitio o una lista como una plantilla en SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ad398-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="ad398-106">**El botón Guardar plantilla de sitio o lista no está disponible o no se encuentra**</span><span class="sxs-lookup"><span data-stu-id="ad398-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="ad398-107">Los administradores tendrán que permitir el script personalizado para habilitar las características de plantilla.</span><span class="sxs-lookup"><span data-stu-id="ad398-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="ad398-108">Para obtener instrucciones detalladas, vea ejemplos y consideraciones.</span><span class="sxs-lookup"><span data-stu-id="ad398-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="ad398-109">Permitir o impedir scripts personalizados</span><span class="sxs-lookup"><span data-stu-id="ad398-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="ad398-110">El comando Guardar sitio como plantilla no es compatible y puede causar problemas en sitios que usan la infraestructura de publicación de SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="ad398-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="ad398-111">**La plantilla de sitio no se puede crear o no funciona correctamente**</span><span class="sxs-lookup"><span data-stu-id="ad398-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="ad398-112">Puede que la plantilla falte una [característica](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) y no se activará.</span><span class="sxs-lookup"><span data-stu-id="ad398-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="ad398-113">Si la característica no está disponible para activarse en la colección de sitios actual, no se puede usar la plantilla de sitio para crear un sitio.</span><span class="sxs-lookup"><span data-stu-id="ad398-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="ad398-114">Compruebe si hay listas o bibliotecas que superen el [umbral límite](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de la vista de lista de 5000 elementos, ya que esto puede bloquear la creación de una plantilla de sitio.</span><span class="sxs-lookup"><span data-stu-id="ad398-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="ad398-115">Es posible que el sitio esté usando demasiados recursos y, por lo tanto, la plantilla de sitio supera el límite de 50 MB.</span><span class="sxs-lookup"><span data-stu-id="ad398-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="ad398-116">Hay problemas para mostrar los datos de una lista que usa una columna de búsqueda.</span><span class="sxs-lookup"><span data-stu-id="ad398-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="ad398-117">Para obtener más información, vea [la lista generada por plantillas no muestra los datos de la lista de búsqueda correcta en SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="ad398-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="ad398-118">Para obtener información más detallada sobre los problemas comunes y las soluciones, consulte [crear y usar plantillas de sitio](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="ad398-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



