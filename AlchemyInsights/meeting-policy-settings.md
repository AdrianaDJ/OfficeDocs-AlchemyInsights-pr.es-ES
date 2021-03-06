---
title: Configuración de la Directiva de reunión
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794351"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrar directivas de reuniones en Microsoft Teams

**Nota: los cambios en la Directiva pueden tardar hasta 24 horas en surtir efecto para los usuarios.** Es posible que no pueda realizar cambios en las directivas recién creadas inmediatamente; Espere 4 horas e intente volver a modificar una Directiva recién creada.

Las directivas de reunión se usan para controlar las características que están disponibles para los participantes de la reunión en las reuniones programadas por los usuarios de la organización. Es posible que algunas características de las directivas de reunión no se implementen todavía en el centro de administración de Microsoft Teams (se les etiqueta "próximamente" en la documentación). En este caso, o si recibe un error como "no se puede actualizar la Directiva en este momento, pero vuelva a intentarlo más tarde" en el centro de administración de Microsoft Teams, se recomienda usar PowerShell para crear o modificar las directivas de reunión de Teams. 

Para obtener más información acerca de las directivas de reunión, vea los siguientes recursos:

- Para obtener información sobre cómo crear directivas, realizar cambios y asignar usuarios a la Directiva, consulte [Administrar directivas de reuniones en Microsoft Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para realizar cambios en la Directiva con los cmdlets de PowerShell, vea [Team PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Debe usar el módulo de [PowerShell de Skype empresarial](https://www.microsoft.com/download/details.aspx?id=39366) para las directivas de reunión de Microsoft Teams. 
    - Para obtener más información, consulte la documentación de los [cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

