---
title: Problema de activación/inicio de sesión-el módulo de plataforma de confianza no funciona correctamente
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: 13e6fcd18047e511452f0180dc2e4677466d4db3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697538"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corrección de las aplicaciones de Microsoft 365 "el módulo de plataforma de confianza del equipo no está funcionando correctamente" mensaje

Para corregir este error, siga estos pasos:

1. Abra una aplicación de Office y [cierre sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) en las cuentas de usuario existentes.   
2. Uso de **Settings**  >  **cuentas**  >  de configuración de Windows cuentas de **& de correo electrónico**, quitar cuentas de trabajo existentes. 
3. Uso de cuentas de **configuración**  >  **Accounts**  >  de Windows**acceso a trabajo o escuela**, desconecte cuentas existentes. 
4. Restablezca el estado de activación de Office. [Obtenga más información](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Pruebe el [proceso de recuperación del usuario](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corregir los errores del módulo de plataforma de confianza (TPM).