---
title: Solucionar problemas de sincronización de contraseñas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664943"
---
# <a name="troubleshoot-password-synchronization"></a>Solucionar problemas de sincronización de contraseñas

Para solucionar problemas de sincronización de contraseñas, empiece con esta tarea de solución de problemas de AAD Connect para determinar por qué las contraseñas no se sincronizan. Para empezar, vaya a [Manage Direct Sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Abra una nueva sesión de Windows PowerShell en su servidor de Azure AD Connect y seleccione la opción **Ejecutar como administrador** .

2. Ejecute Set-ExecutionPolicy RemoteSigned o Set-ExecutionPolicy Unrestricted.

3. Inicie el Asistente de Azure AD Connect.

4. Vaya a la página tareas adicionales > **solucionar problemas**a  >  **continuación**.

5. Seleccione **iniciar** para abrir el menú solución de problemas de PowerShell.

6. Seleccione **solucionar problemas de sincronización de contraseñas**.

    El problema suele ser que una contraseña no está sincronizada para una cuenta de usuario específica.

    **Notas** Se produce un error en la sincronización de contraseña si la última sincronización de contraseña correcta ha transcurrido algún tiempo.

Para obtener más información sobre cómo solucionar problemas de sincronización de contraseñas, vea [solucionar problemas de sincronización de hash de contraseña con Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).