---
title: Las directivas de retención del centro de administración de Exchange no funcionan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522824"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Directivas de retención en el centro de administración de Exchange

Si desea que se ejecuten comprobaciones automatizadas para la configuración que se menciona a continuación, seleccione el botón atrás <--en la parte superior de esta página y, a continuación, escriba la dirección de correo electrónico del usuario que tiene problemas con las directivas de retención.

 **Problema:** Las directivas de retención recién creadas o actualizadas en el centro de administración de Exchange no se aplican a los buzones o los elementos no se mueven al buzón de archivo o se eliminan. 
  
 **Causas principales:**
  
- Esto puede deberse a que el **Asistente para carpeta administrada** no ha procesado el buzón del usuario. El Asistente para carpeta administrada intenta procesar todos los buzones de correo de la organización basada en la nube una vez cada siete días. Si cambia una etiqueta de retención o aplica una directiva de retención diferente a un buzón, puede esperar hasta que la carpeta administrada Ayude a procesar el buzón o puede ejecutar el cmdlet Start-ManagedFolderAssistant para iniciar el Asistente para carpeta administrada para procesar un buzón específico. La ejecución de este cmdlet es útil para probar o solucionar problemas de configuración de una directiva de retención o de una etiqueta de retención. Para obtener más información, visite [ejecutar el Asistente para carpeta administrada](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solución:** Ejecute el siguiente comando para iniciar el Asistente para carpeta administrada para un buzón específico:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Esto también puede ocurrir si **RetentionHold** se ha **habilitado** en el buzón de correo. Si el buzón se ha colocado en un RetentionHold, la Directiva de retención en el buzón no se procesará durante este período. Para obtener más información sobre la configuración de RetentionHold, vea: conservación de la [retención de buzones de correo](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Soluciones**
    
  - Compruebe el estado de la opción RetentionHold en el buzón específico en el [PowerShell Exo](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Ejecute el siguiente comando para **deshabilitar** RetentionHold en un buzón específico:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Ahora, vuelva a ejecutar el Asistente para carpeta administrada:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Nota:** Si un buzón tiene menos de 10 MB, el Asistente para carpeta administrada no procesará automáticamente el buzón.
 
Para obtener más información sobre las directivas de retención en el centro de administración de Exchange, consulte:
- [Etiquetas de retención y directivas de retención](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Aplicar una directiva de retención a los buzones](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Agregar o quitar las etiquetas de retención](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Cómo identificar el tipo de retención en un buzón](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
