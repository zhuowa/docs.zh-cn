---
title: 如何：创建网格元素
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- Grid control [WPF], creating [WPF], grid instance
ms.assetid: b2f07626-9df8-43b8-8d36-492f3cb42837
ms.openlocfilehash: b93bb859c4a0df50da2fa00587a28fda3776fd09
ms.sourcegitcommit: c93fd5139f9efcf6db514e3474301738a6d1d649
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/27/2018
ms.locfileid: "50185779"
---
# <a name="how-to-create-a-grid-element"></a>如何：创建网格元素
## <a name="example"></a>示例  
 下面的示例演示如何创建和使用的实例<xref:System.Windows.Controls.Grid>通过使用[!INCLUDE[TLA#tla_xaml](../../../../includes/tlasharptla-xaml-md.md)]或代码。 此示例使用三种<xref:System.Windows.Controls.ColumnDefinition>对象和三个<xref:System.Windows.Controls.RowDefinition>对象创建一个网格，其中具有九个单元格，例如工作表。 每个单元都包含<xref:System.Windows.Controls.TextBlock>表示数据，而顶部行的元素包含<xref:System.Windows.Controls.TextBlock>与<xref:System.Windows.Controls.Grid.ColumnSpan%2A>应用属性。 若要显示的每个单元格边界<xref:System.Windows.Controls.Grid.ShowGridLines%2A>启用属性。  
  
 [!code-csharp[Grid#3](../../../../samples/snippets/csharp/VS_Snippets_Wpf/Grid/CSharp/Grid_Code.cs#3)]
 [!code-vb[Grid#3](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/Grid/VisualBasic/grid_vb.vb#3)]
 [!code-xaml[Grid#3](../../../../samples/snippets/xaml/VS_Snippets_Wpf/Grid/XAML/default.xaml#3)]  
  
  这两种方法将生成一个用户界面，看起来都非常相同的如下所示。

  ![屏幕截图描绘了一个 WPF 用户界面，其中包含一个网格，分成三个列。  它具有 2018年产品提供了跨顶部行的所有列的标题，并具有三列每个销售数字与特定季度。  底部行具有跨两个列并显示消息的文本总单位数： 300000](./media/how-to-create-a-grid-element/how-to-create-a-grid-element.png)
## <a name="see-also"></a>请参阅  
 <xref:System.Windows.Controls.Grid>  
 [面板概述](../../../../docs/framework/wpf/controls/panels-overview.md)
