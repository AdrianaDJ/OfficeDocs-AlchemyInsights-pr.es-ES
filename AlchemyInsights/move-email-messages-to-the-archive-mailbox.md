---
title: Mover mensajes de correo electrónico para el buzón de archivo
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/15/2019
ms.locfileid: "28314452"
---
<span data-ttu-id="80e29-p101">Problemas de los elementos en el buzón de archivo de archivado. Asegúrese de que haber realizado los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="80e29-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="80e29-p102">Confirme que se ha habilitado un **buzón de correo de archivar** . Si no es así, siga los pasos de [este artículo](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) para habilitar el buzón de archivo.</span><span class="sxs-lookup"><span data-stu-id="80e29-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="80e29-106">En el centro de administración de Exchange, seleccione **Las etiquetas de retención** en **Administración de cumplimiento de normas**, crear una **etiqueta de retención** con la acción **mover a archivo** que contiene la **Antigüedad de retención**de deseada.</span><span class="sxs-lookup"><span data-stu-id="80e29-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="80e29-107">En el centro de administración de Exchange, seleccione **Las directivas de retención**, crear una **Directiva de retención** y agregar la etiqueta de retención **mover a archivo** a esa directiva.</span><span class="sxs-lookup"><span data-stu-id="80e29-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="80e29-p103">[Asignar la directiva de retención](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) para el buzón de un usuario específico. La misma directiva se aplicará a la **principal** y el buzón de **archivo** .</span><span class="sxs-lookup"><span data-stu-id="80e29-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="80e29-p104">El buzón del usuario ahora debería tener una directiva de archivo para mover los elementos en el buzón de archivo. Es posible que sea necesario forzar la administrados carpeta Ayudante (MFA) para ejecutar y aplicar la nueva configuración para el buzón del usuario. Ejecute el siguiente comando mientras [conectado a EXO de PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar el Asistente para carpeta administrada para un buzón específico:</span><span class="sxs-lookup"><span data-stu-id="80e29-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="80e29-113">Desea obtener más información acerca de cómo configurar una directiva de archivo, vea [Configurar una directiva de eliminación y de archivo para los buzones de correo](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="80e29-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  
