---
title: Solución de Microsoft 365 apps no se pudieron encontrar las licencias de Office mensaje asociado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580458"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Corrección del mensaje "no se pudieron encontrar las licencias de Office asociadas" en Microsoft 365 apps

Si recibe este mensaje, pruebe lo siguiente:

1. Compruebe el firewall, el software antivirus y la configuración de proxy para confirmar que no están bloqueando el acceso a Internet a las aplicaciones de Microsoft 365. Consulte [direcciones URL e intervalos de direcciones IP de 365 de Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Quite y [reasigne la licencia de Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) para el usuario afectado. 
3. Abra una aplicación de Office y [cierre la sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de las cuentas de usuario existentes.
4. Vaya a configuración de Windows **> cuentas**de  >  **correo &** cuentas y quite todas las cuentas de trabajo excepto la cuenta afectada.
5. Vaya a configuración de Windows > **cuentas**  >  **tienen acceso a trabajo o escuela**y desconectan todas las cuentas de trabajo, excepto la cuenta afectada.
6. Restablezca el estado de activación de Office. [Obtenga más información](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Inicie sesión](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.

Para obtener soluciones adicionales para la solución de problemas, consulte [errores de activación y de producto sin licencia en Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).