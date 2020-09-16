---
title: 1491-búsqueda-no-devolución-resultados-esperado
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740491"
---
# <a name="content-search-not-returning-expected-results"></a>La búsqueda de contenido no devuelve los resultados esperados

Al ejecutar búsquedas de contenido desde el centro de seguridad & cumplimiento de Microsoft 365, es posible que reciba resultados de búsqueda inesperados. Tenga en cuenta lo siguiente que puede afectar a los resultados de la búsqueda:

- **Ubicaciones de contenido y condiciones de búsqueda**: Asegúrese de que ha seleccionado las ubicaciones de contenido y las condiciones de búsqueda adecuadas. Si ha ejecutado una búsqueda grande (con muchas ubicaciones), considere la posibilidad de dividirla en varias búsquedas.

- **Elementos parcialmente indizados**: los  [elementos indexados parcialmente](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) de los buzones se incluyen en los resultados de búsqueda estimados. Sin embargo, los elementos parcialmente indizados de sitios de SharePoint y OneDrive no se incluyen en la estimación de la búsqueda.

- **Errores de búsqueda**: al buscar en un gran número de buzones (más de 100.000 buzones), es posible que obtenga errores de búsqueda, con códigos de error como CS008-009 y CS012-002). En este caso, vuelva a intentar la búsqueda solo para las ubicaciones de contenido con error. Consulte  [este artículo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para obtener más información.
