---
title: DLP no funciona como se esperaba
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679710"
---
# <a name="dlp-not-working-as-expected"></a>DLP no funciona como se esperaba

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Configuración de DLP**

¿Tiene problemas con la **prevención de pérdida de datos (DLP)** en Office 365 que no funciona como se esperaba? Si es así, asegúrese de que la **Directiva DLP** está correctamente configurada y de que los datos contienen lo que la **Directiva DLP** busca cuando se evalúa.
  
Las directivas de DLP le permiten identificar y proteger la información confidencial de su organización. Para configurar directivas de DLP, use la información que se muestra [aquí](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Qué buscan las directivas de DLP**
  
Al usar los **tipos de información confidencial integrados** en los centros de seguridad y cumplimiento, las directivas de DLP buscan patrones y elementos específicos al detectar estos tipos confidenciales.
  
- **Tipos de información confidencial integrados**

    Para obtener información sobre los tipos confidenciales integrados y qué busca una directiva DLP cuando se detecta el tipo confidencial, vea: [Qué buscan los tipos de información confidencial](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipos personalizados de información confidencial**

    Si está intentando crear tipos personalizados de información confidencial, use el siguiente artículo para obtener información sobre cómo crear un tipo confidencial personalizado: [crear un tipo personalizado de información confidencial](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Probar una directiva DLP**

Para probar los datos con un tipo de información confidencial integrado o personalizado, use la opción **tipo de prueba** en **clasificaciones**de  >  **información confidencial**. Para obtener más información, vea [probar tipos personalizados de información confidencial](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Informes**
  
- Obtenga información confidencial sobre los datos con [informes de DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Vea los detalles específicos del evento con un [Informe de incidentes](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
