---
title: Solución de problemas al usar abrir con el explorador
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659075"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="186d9-102">Solucionar problemas con abrir con el explorador</span><span class="sxs-lookup"><span data-stu-id="186d9-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="186d9-103">Solucionar problemas comunes de la apertura de una biblioteca de documentos en SharePoint o OneDrive con el comando **abrir con el explorador** :</span><span class="sxs-lookup"><span data-stu-id="186d9-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="186d9-104">Usar Internet Explorer 10 o Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="186d9-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="186d9-105">**Abrir con el explorador** no es compatible con Microsoft Edge, Google Chrome, Firefox y otros.</span><span class="sxs-lookup"><span data-stu-id="186d9-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="186d9-106">**Abrir con el explorador** está deshabilitado en todos los exploradores excepto en Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="186d9-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="186d9-107">**Abrir con el explorador** no está disponible en la experiencia moderna de las bibliotecas de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="186d9-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="186d9-108">En su lugar, use **ver en el explorador de archivos** .</span><span class="sxs-lookup"><span data-stu-id="186d9-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="186d9-109">Seleccione Ver **Opciones** \> **de vista en el explorador de archivos**.</span><span class="sxs-lookup"><span data-stu-id="186d9-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="186d9-110">Ver en el explorador de archivos no es compatible con Microsoft Edge, Google Chrome, Firefox y otros.</span><span class="sxs-lookup"><span data-stu-id="186d9-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="186d9-111">**Ver en el explorador de archivos** solo está disponible en Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="186d9-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="186d9-112">Asegúrese de que el servicio WebClient se está ejecutando.</span><span class="sxs-lookup"><span data-stu-id="186d9-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="186d9-113">En el cuadro de búsqueda de Windows, escriba ejecutar, seleccione la aplicación de escritorio ejecutar, escriba Services. msc y, a continuación, presione Entrar.</span><span class="sxs-lookup"><span data-stu-id="186d9-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="186d9-114">Desplácese hacia abajo hasta el servicio WebClient y asegúrese de que la columna **Estado** muestra "en ejecución".</span><span class="sxs-lookup"><span data-stu-id="186d9-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="186d9-115">Si no es así, haga doble clic en el servicio, haga clic en **Inicio**y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="186d9-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="186d9-116">(Es posible que tenga que habilitar primero el servicio seleccionando **manual** o **automático** en el cuadro **tipo de inicio** ).</span><span class="sxs-lookup"><span data-stu-id="186d9-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="186d9-117">Abrir una biblioteca en el explorador de archivos es útil si necesita copiar o mover varios archivos y carpetas una vez, pero si desea trabajar con regularidad en la biblioteca, le recomendamos que lo sincronice.</span><span class="sxs-lookup"><span data-stu-id="186d9-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="186d9-118">Para solucionar problemas de apertura en el explorador de archivos, consulte [abrir en el explorador](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="186d9-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="186d9-119">Para obtener información sobre cómo configurar la sincronización, vea [sincronizar archivos de SharePoint con el nuevo cliente de sincronización de OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="186d9-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="186d9-120">Consulte el artículo [Cómo usar el comando "abrir con el explorador" para solucionar problemas en SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="186d9-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

