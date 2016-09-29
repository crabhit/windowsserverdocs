---
title: Web SSO Design
description:
author: billmath
ms.author:  billmath
manager: femila
ms.date: 09/28/2016
ms.topic: article
ms.prod: windows-server-threshold
ms.service: active-directory
ms.technology: identity-adfs
---

# Web SSO Design

>Applies To: Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

In the Web Single\-Sign\-On \(SSO\) design in Active Directory Federation Services \(AD FS\), users must authenticate only once to access multiple AD FS\-secured applications or services. In this design all users are external, and no federation trust exists because there are no partner organizations. Typically, you deploy this design when you want to provide individual consumer or customer access to one or more AD FS–secured services or applications over the Internet, as shown in the following illustration.  
  
![](media/adfs2_WebSSODesign.gif)  
  
With the Web SSO design, an organization that typically hosts an AD FS\-secured application or service in a perimeter network can maintain a separate store of customer accounts in the perimeter network, which makes it easier to isolate customer accounts from employee accounts.  
  
You can manage the local accounts for customers in the perimeter network by using either Active Directory Domain Services \(AD DS\), SQL Server, or a custom attribute store.  
  
This design coincides with the deployment goal in [Provide Your Active Directory Users Access to Your Claims-Aware Applications and Services](Provide-Your-Active-Directory-Users-Access-to-Your-Claims-Aware-Applications-and-Services.md).  
  
For a list of detailed tasks that you can use to plan and deploy your Web SSO design, see [Checklist: Implementing a Web SSO Design](../../ad-fs/deployment/Checklist--Implementing-a-Web-SSO-Design.md).  
  
## See Also
[AD FS Design Guide in Windows Server 2012](AD-FS-Design-Guide-in-Windows-Server-2012.md)