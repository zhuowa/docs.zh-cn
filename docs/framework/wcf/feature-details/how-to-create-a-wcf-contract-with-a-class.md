---
title: 如何：使用类创建 Windows Communication Foundation 约定
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
ms.assetid: 1ad69393-3915-4e7f-9b91-b6fc59c6f5ba
ms.openlocfilehash: 296f500532040aaebf0f6d7d37a7a9aae99a3451
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
ms.locfileid: "33491801"
---
# <a name="how-to-create-a-windows-communication-foundation-contract-with-a-class"></a>如何：使用类创建 Windows Communication Foundation 约定
创建 Windows Communication Foundation (WCF) 协定的首选的方法是使用接口。 有关详细信息，请参阅[如何： 定义服务协定](../../../../docs/framework/wcf/how-to-define-a-wcf-service-contract.md)。 本文介绍另一种方式，即创建一个类，然后直接对该类应用 <xref:System.ServiceModel.ServiceContractAttribute> 特性，并对该类中作为协定一部分的每个方法应用 <xref:System.ServiceModel.OperationContractAttribute> 特性。  
  
> [!WARNING]
>  `[ServiceContract]` 和 `[ServiceContractAttribute]` 的作用一样。 `[OperationContract]` 和 `[OperationContractAttribute]` 的作用一样。 在每种情况下，前者都是后者的简写。  
  
 有关服务协定的详细信息，请参阅[设计服务协定](../../../../docs/framework/wcf/designing-service-contracts.md)。  
  
### <a name="creating-a-windows-communication-foundation-contract-with-a-class"></a>通过类创建 Windows Communication Foundation 协定  
  
1.  创建一个新的类，使用 Visual Basic、 C# 中，或任何将其他公共语言运行时语言。  
  
2.  对该类应用 <xref:System.ServiceModel.ServiceContractAttribute> 类。  
  
3.  创建该类中的方法。  
  
4.  应用<xref:System.ServiceModel.OperationContractAttribute>到每个方法都必须作为公共 WCF 协定的一部分进行公开的类。  
  
## <a name="example"></a>示例  
 下面的代码示例演示定义服务协定的类。  
  
 [!code-csharp[c_HowTo_CreateContractWithClass#1](../../../../samples/snippets/csharp/VS_Snippets_CFX/c_howto_createcontractwithclass/cs/source.cs#1)]
 [!code-vb[c_HowTo_CreateContractWithClass#1](../../../../samples/snippets/visualbasic/VS_Snippets_CFX/c_howto_createcontractwithclass/vb/source.vb#1)]  
  
 默认情况下，应用了 <xref:System.ServiceModel.OperationContractAttribute> 类的方法使用请求-答复消息模式。 有关此消息模式的详细信息，请参阅[如何： 创建请求-答复协定](../../../../docs/framework/wcf/feature-details/how-to-create-a-request-reply-contract.md)。 您还可以通过设置属性 (Attribute) 的属性 (Property) 来创建和使用其他消息模式。 有关更多示例，请参阅[如何： 创建单向协定](../../../../docs/framework/wcf/feature-details/how-to-create-a-one-way-contract.md)和[如何： 创建双工协定](../../../../docs/framework/wcf/feature-details/how-to-create-a-duplex-contract.md)。  
  
## <a name="see-also"></a>请参阅  
 <xref:System.ServiceModel.ServiceContractAttribute>  
 <xref:System.ServiceModel.OperationContractAttribute>
