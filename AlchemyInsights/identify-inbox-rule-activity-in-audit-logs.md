---
title: Identificar la actividad de las reglas de entrada en los registros de auditoría
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779068"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar la actividad de las reglas de entrada en los registros de auditoría

Puede usar la búsqueda de registros de auditoría en el centro de cumplimiento de & de seguridad de Microsoft 365 para ver eventos de reglas de la bandeja de entrada (crear, modificar y eliminar reglas de la bandeja de entrada).

1. Inicie sesión en el [centro de cumplimiento de & de seguridad de Microsoft 365](https://protection.office.com/).

2. Vaya a la **Search**  >  Página de**búsqueda del registro de auditoría** de búsqueda.

3. Seleccione el intervalo de fechas en los campos **fecha de inicio** y **fecha de finalización** .

4. En **actividades de buzón de Exchange**, compruebe que el campo **actividades** está establecido en **nueva-InboxRule crear/modificar/habilitar/deshabilitar la regla de bandeja de entrada**.

5. Haga clic en **Buscar**.

En los resultados, seleccione un registro de auditoría. En el control flotante de detalles, haga clic en **más información**. La información sobre la configuración de las reglas de la bandeja de entrada se muestra en el campo **parámetros** .

Para obtener más información, vea [determinar si un usuario creó una regla de bandeja de entrada](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .
