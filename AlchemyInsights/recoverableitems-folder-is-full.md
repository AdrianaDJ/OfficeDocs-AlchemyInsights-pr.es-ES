---
title: 1336 la carpeta RecoverableItems está llena
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741284"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="1ba4f-102">La carpeta elementos recuperables está llena</span><span class="sxs-lookup"><span data-stu-id="1ba4f-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="1ba4f-103">Para los buzones de correo de Exchange Online, el límite de almacenamiento predeterminado para la carpeta elementos recuperables es de 30 GB.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="1ba4f-104">El límite de almacenamiento de la carpeta elementos recuperables aumenta automáticamente a 100 GB si el buzón se coloca en retención por juicio, suspensión de eDiscovery o se asigna a una directiva de retención.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="1ba4f-105">Cuando la carpeta elementos recuperables alcanza el límite de almacenamiento, la funcionalidad de buzón de correo se ve afectada de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="1ba4f-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="1ba4f-106">El usuario no puede eliminar elementos del buzón.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="1ba4f-107">El asistente para carpetas administradas no puede eliminar elementos basados en la etiqueta de retención o en la configuración de carpetas administradas.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="1ba4f-108">Para los buzones que tienen habilitada la recuperación de un único elemento o que están en espera, el proceso de protección de página de copia en escritura no puede mantener versiones de los elementos editados por el usuario.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="1ba4f-109">Para los buzones que tienen habilitado el registro de auditoría de buzones de correo, las entradas del registro de auditoría de buzones no se pueden guardar en la subcarpeta auditorías de la carpeta elementos recuperables.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="1ba4f-110">Para los buzones que no están en suspensión, los administradores pueden usar el `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comando en Exchange Online PowerShell para eliminar elementos de la carpeta elementos recuperables.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="1ba4f-111">Para obtener más información, consulte los siguientes temas:</span><span class="sxs-lookup"><span data-stu-id="1ba4f-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="1ba4f-112">Búsqueda y eliminación de mensajes</span><span class="sxs-lookup"><span data-stu-id="1ba4f-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="1ba4f-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="1ba4f-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="1ba4f-114">Para los buzones que están en retención, los administradores deben quitar la retención antes de que puedan eliminar elementos de la carpeta elementos recuperables.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="1ba4f-115">Para obtener más información, vea [eliminar elementos de la carpeta elementos recuperables de buzones basados en la nube en retención](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="1ba4f-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="1ba4f-116">Para ayudar a evitar que la carpeta elementos recuperables se llene, los administradores pueden aumentar el límite de almacenamiento de la carpeta elementos recuperables para los buzones de correo en retención y configurar una directiva de retención de buzones que mueva los elementos de la carpeta elementos recuperables al buzón de archivo del usuario.</span><span class="sxs-lookup"><span data-stu-id="1ba4f-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="1ba4f-117">Consulte [aumentar la cuota de elementos recuperables para los buzones de correo en retención](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="1ba4f-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
