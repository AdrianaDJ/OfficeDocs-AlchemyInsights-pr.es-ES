---
title: Escritorio de Outlook recuperar o reemplazar un mensaje de correo electrónico
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502336"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="b0704-102">Recuperar o reemplazar un mensaje de correo electrónico de Outlook</span><span class="sxs-lookup"><span data-stu-id="b0704-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="b0704-103">Como administrador, puede **recuperar mensajes en nombre de los usuarios mediante PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="b0704-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="b0704-104">No puede recuperar mensajes del centro de administración.</span><span class="sxs-lookup"><span data-stu-id="b0704-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="b0704-105">Solo puede **recuperar los mensajes que se envían a las personas de su organización**.</span><span class="sxs-lookup"><span data-stu-id="b0704-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="b0704-106">Si el mensaje se envió a una dirección de gmail, por ejemplo, no puede recuperarlo.</span><span class="sxs-lookup"><span data-stu-id="b0704-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="b0704-107">Solo puede **recuperar los mensajes enviados desde Outlook 2016 en el equipo PC**.</span><span class="sxs-lookup"><span data-stu-id="b0704-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="b0704-108">Si un usuario envía un mensaje con Outlook para Mac o Outlook en la web, no puede recuperarlo.</span><span class="sxs-lookup"><span data-stu-id="b0704-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="b0704-109">Para recuperar o reemplazar un mensaje de correo electrónico:</span><span class="sxs-lookup"><span data-stu-id="b0704-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="b0704-110">En el panel de carpetas en la parte izquierda de la ventana de Outlook, seleccione la carpeta elementos enviados.</span><span class="sxs-lookup"><span data-stu-id="b0704-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="b0704-111">Haga doble clic en el mensaje que desea recuperar para abrirlo.</span><span class="sxs-lookup"><span data-stu-id="b0704-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="b0704-112">Seleccione la pestaña **mensaje** y, a continuación, seleccione **acciones**  >  **recuperar este mensaje**.</span><span class="sxs-lookup"><span data-stu-id="b0704-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="b0704-113">Seleccione **eliminar copias no leídas de este mensaje** o **eliminar copias no leídas y reemplazarlas con un nuevo mensaje**y, a continuación, seleccione **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="b0704-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="b0704-114">Si va a enviar un mensaje de reemplazo, Redacte el mensaje y, a continuación, seleccione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="b0704-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="b0704-115">El éxito o el fracaso de una recuperación de mensajes depende de la configuración del destinatario en Outlook.</span><span class="sxs-lookup"><span data-stu-id="b0704-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="b0704-116">Para conocer los pasos para comprobar la recuperación, consulte [este artículo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="b0704-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="b0704-117">Buscar y eliminar mensajes de correo electrónico en la organización</span><span class="sxs-lookup"><span data-stu-id="b0704-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="b0704-118">Si no es un administrador global, la cuenta debe agregarse a la función Administrador de eDiscovery o la función administración de búsqueda de cumplimiento para buscar mensajes.</span><span class="sxs-lookup"><span data-stu-id="b0704-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="b0704-119">Para eliminar mensajes, debe unirse al grupo de funciones de administración de la organización o al rol de administración de búsqueda y depuración.</span><span class="sxs-lookup"><span data-stu-id="b0704-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="b0704-120">Los permisos para estos roles se asignan en el [centro de seguridad y cumplimiento](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="b0704-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="b0704-121">[Cree una búsqueda de contenido](https://docs.microsoft.com/microsoft-365/compliance/content-search) para buscar el mensaje que se va a eliminar.</span><span class="sxs-lookup"><span data-stu-id="b0704-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="b0704-122">[Conéctese a PowerShell del centro de seguridad y cumplimiento](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b0704-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="b0704-123">Si está usando la autenticación multifactor, consulte [conectarse a PowerShell del centro de seguridad y cumplimiento de Microsoft 365 mediante la autenticación multifactor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b0704-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>