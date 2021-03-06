---
title: Solucionar problemas relacionados con la inscripción de dispositivos Windows en Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658895"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Solucionar problemas relacionados con la inscripción de dispositivos Windows en Microsoft Intune

Revise los recursos que se enumeran a continuación para resolver su problema ahora.
  
Algunos mensajes de error comunes y pasos de resolución:
  
 **El software no se puede instalar, 0x80cf4017:** El certificado de cuenta ha expirado. Vuelva a descargar el paquete de software cliente de PC en la consola de administración de Intune. Consulte esta documentación para obtener más información.
  
 **Código de error 0x801c0003:** El error puede producirse en las siguientes situaciones:
  
-  El usuario tiene más dispositivos inscritos que el límite del dispositivo. Revise estos documentos para [quitar un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [cambiar el límite del dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Los usuarios pueden unir dispositivos a Azure AD" se establece en "ninguno". Establézcalo en todos o seleccione usuarios. Consulte [esta documentación](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obtener más información.

-  El dispositivo ya está inscrito por otro usuario. Si ese es el caso, quite el dispositivo de la consola de Azure Intune o elimine la inscripción del dispositivo manualmente antes de volver a intentarlo.

-  El dispositivo es Windows 10 Home. Solo las SKU de Windows 10 Pro, Education y Enterprise pueden unirse a Azure Active Directory.

Recursos adicionales para ayudar a resolver el problema:
  
-  Use el [portal de solución de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar y resolver errores comunes de inscripción. Revise [este documento](https://docs.microsoft.com/intune/help-desk-operators) para obtener más información.

-  Consulte estos documentos para ver una lista de errores comunes que impiden la inscripción y las soluciones para cada uno: [Guía de solución de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) y [Documento de solución de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Obtenga información sobre cómo inscribir dispositivos Windows en Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
