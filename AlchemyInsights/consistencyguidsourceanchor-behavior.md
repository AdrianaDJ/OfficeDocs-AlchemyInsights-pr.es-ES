---
title: Comportamiento de ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756300"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f7102-102">Comportamiento de ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="f7102-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f7102-103">Azure AD Connect (versión 1.1.524.0 y After) ahora facilita el uso de msDS-ConsistencyGuid como atributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="f7102-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="f7102-104">Cuando se usa esta característica, Azure AD Connect configura automáticamente las reglas de sincronización para:</span><span class="sxs-lookup"><span data-stu-id="f7102-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f7102-105">Use msDS-ConsistencyGuid como atributo sourceAnchor para objetos de usuario.</span><span class="sxs-lookup"><span data-stu-id="f7102-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="f7102-106">ObjectGUID se usa para otros tipos de objeto.</span><span class="sxs-lookup"><span data-stu-id="f7102-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f7102-107">Para un objeto de usuario de AD local dado cuyo atributo msDS-ConsistencyGuid no está rellenado, Azure AD Connect vuelve a escribir el valor de objectGUID en el atributo msDS-ConsistencyGuid de Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="f7102-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="f7102-108">Una vez que se haya rellenado el atributo msDS-ConsistencyGuid, Azure AD Connect exportará el objeto a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f7102-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f7102-109">**Nota:** Una vez que un objeto de AD local se importa a Azure AD Connect (es decir, se importa en el espacio de conector de AD y se proyecta en el metaverso), no puede cambiar su valor de sourceAnchor ya.</span><span class="sxs-lookup"><span data-stu-id="f7102-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="f7102-110">Para especificar el valor sourceAnchor para un objeto AD local determinado, configure su atributo msDS-ConsistencyGuid antes de importarlo a Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f7102-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f7102-111">Para obtener más información sobre SourceAnchor y ConsistencyGuid, consulte lo siguiente: [Azure ad Connect: conceptos de diseño](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f7102-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

