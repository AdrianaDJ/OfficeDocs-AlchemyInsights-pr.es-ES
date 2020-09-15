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
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="8b646-102">DLP no funciona como se esperaba</span><span class="sxs-lookup"><span data-stu-id="8b646-102">DLP not working as expected</span></span>

<span data-ttu-id="8b646-103">**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="8b646-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="8b646-104">**Configuración de DLP**</span><span class="sxs-lookup"><span data-stu-id="8b646-104">**Setting up DLP**</span></span>

<span data-ttu-id="8b646-105">¿Tiene problemas con la **prevención de pérdida de datos (DLP)** en Office 365 que no funciona como se esperaba?</span><span class="sxs-lookup"><span data-stu-id="8b646-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="8b646-106">Si es así, asegúrese de que la **Directiva DLP** está correctamente configurada y de que los datos contienen lo que la **Directiva DLP** busca cuando se evalúa.</span><span class="sxs-lookup"><span data-stu-id="8b646-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="8b646-107">Las directivas de DLP le permiten identificar y proteger la información confidencial de su organización.</span><span class="sxs-lookup"><span data-stu-id="8b646-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="8b646-108">Para configurar directivas de DLP, use la información que se muestra [aquí](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="8b646-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="8b646-109">**Qué buscan las directivas de DLP**</span><span class="sxs-lookup"><span data-stu-id="8b646-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="8b646-110">Al usar los **tipos de información confidencial integrados** en los centros de seguridad y cumplimiento, las directivas de DLP buscan patrones y elementos específicos al detectar estos tipos confidenciales.</span><span class="sxs-lookup"><span data-stu-id="8b646-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="8b646-111">**Tipos de información confidencial integrados**</span><span class="sxs-lookup"><span data-stu-id="8b646-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="8b646-112">Para obtener información sobre los tipos confidenciales integrados y qué busca una directiva DLP cuando se detecta el tipo confidencial, vea: [Qué buscan los tipos de información confidencial](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="8b646-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="8b646-113">**Tipos personalizados de información confidencial**</span><span class="sxs-lookup"><span data-stu-id="8b646-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="8b646-114">Si está intentando crear tipos personalizados de información confidencial, use el siguiente artículo para obtener información sobre cómo crear un tipo confidencial personalizado: [crear un tipo personalizado de información confidencial](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="8b646-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="8b646-115">**Probar una directiva DLP**</span><span class="sxs-lookup"><span data-stu-id="8b646-115">**Test a DLP policy**</span></span>

<span data-ttu-id="8b646-116">Para probar los datos con un tipo de información confidencial integrado o personalizado, use la opción **tipo de prueba** en **clasificaciones**de  >  **información confidencial**.</span><span class="sxs-lookup"><span data-stu-id="8b646-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="8b646-117">Para obtener más información, vea [probar tipos personalizados de información confidencial](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="8b646-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="8b646-118">**Informes**</span><span class="sxs-lookup"><span data-stu-id="8b646-118">**Reports**</span></span>
  
- <span data-ttu-id="8b646-119">Obtenga información confidencial sobre los datos con [informes de DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="8b646-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="8b646-120">Vea los detalles específicos del evento con un [Informe de incidentes](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="8b646-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
