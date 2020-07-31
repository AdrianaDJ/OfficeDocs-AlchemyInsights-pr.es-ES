---
title: Mover mensajes de correo electrónico al buzón de archivo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522788"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mover el correo electrónico al buzón de archivo

Si desea que se ejecuten comprobaciones automatizadas para la configuración que se menciona a continuación, seleccione el botón atrás <--en la parte superior de esta página y, a continuación, escriba la dirección de correo electrónico del usuario que tiene problemas para mover el correo electrónico a su buzón de archivo.

1. Confirme que se ha habilitado un **buzón de archivo** . Si no es así, siga los pasos de [este artículo](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) para habilitar el buzón de archivo.

2. Para archivar mensajes automáticamente en el buzón de archivo, se debe establecer una etiqueta de retención con la acción **mover a archivo** para que se **aplique automáticamente a toda la etiqueta del buzón (predeterminado)**. Siga los pasos que se describen aquí para crear la etiqueta: [archivar la etiqueta predeterminada](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. A continuación, agregue la etiqueta de **archivo** a la Directiva de retención. En el centro de administración de Exchange, seleccione **directivas de retención** > agregue la **etiqueta mover a archivo** a la Directiva > **Guardar**.

4. Ahora [asigne la Directiva de retención](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) al buzón de correo del usuario específico. La misma directiva se aplicará al buzón **principal** y al buzón de **archivo** .

Puede que sea necesario forzar la ejecución del Asistente para carpeta administrada (MFA) y aplicar la nueva configuración al buzón de correo del usuario. Ejecute el comando siguiente mientras [está conectado a Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar el Asistente para carpeta administrada para un buzón específico:
  
Start-ManagedFolderAssistant-Identity<name of the mailbox>

Para obtener más información sobre cómo configurar una directiva de archivo, consulte [configurar una directiva de archivo y eliminación para los buzones](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  