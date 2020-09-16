---
title: S/MIME en Outlook en la Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772315"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="2d553-102">Cifrar mensajes de correo electrónico en Outlook</span><span class="sxs-lookup"><span data-stu-id="2d553-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="2d553-103">El cifrado de mensajes de Microsoft 365 se basa en Microsoft Azure Rights Management (Azure RMS), que forma parte de Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="2d553-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="2d553-104">Si su suscripción incluye Azure Rights Management o Azure Information Protection, **no necesita realizar ninguna acción para habilitar o activar manualmente** el servicio Rights Management.</span><span class="sxs-lookup"><span data-stu-id="2d553-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="2d553-105">En función de los comentarios de los clientes, ya no se habilitarán las reglas de flujo de correo de Exchange para cifrar automáticamente el correo saliente que contiene determinados tipos de información confidencial en el espacio empresarial de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="2d553-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="2d553-106">En su lugar, proporcionamos instrucciones detalladas sobre cómo puede hacerlo usted mismo.</span><span class="sxs-lookup"><span data-stu-id="2d553-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="2d553-107">Para obtener más información sobre cómo crear una regla de transporte para cifrar información confidencial, consulte [este artículo](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="2d553-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="2d553-108">Si usa Outlook en la web (anteriormente, **OWA**): al redactar un mensaje de correo electrónico, simplemente haga clic en **proteger** en OWA.</span><span class="sxs-lookup"><span data-stu-id="2d553-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="2d553-109">Se aplicará el permiso "no reenviar".</span><span class="sxs-lookup"><span data-stu-id="2d553-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="2d553-110">Haga clic en **Cambiar permiso** y elija **cifrar** para cifrar solo el mensaje.</span><span class="sxs-lookup"><span data-stu-id="2d553-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="2d553-111">Si usa el **cliente de Outlook**: para enviar un mensaje cifrado desde Outlook 2013 o 2016 o Outlook 2016 para Mac, seleccione **Opciones**  >  **permisos**y, a continuación, seleccione la opción de protección que necesite.</span><span class="sxs-lookup"><span data-stu-id="2d553-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="2d553-112">Para **cifrar automáticamente todo el correo electrónico** enviado a determinados destinatarios o organizaciones de asociados externos, debe crear una regla de transporte de flujo de correo en el centro de administración de Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d553-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="2d553-113">Se proporcionan instrucciones detalladas en [este artículo de soporte técnico](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="2d553-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

