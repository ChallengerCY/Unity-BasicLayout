**Unity-RectTransform**
>列举了几种RectTranform中不同Anchors的摆放得到的UI布局效果
![Modify Anchors](https://github.com/ChallengerCY/Unity-RectTransform/blob/master/TestRectTransform/Picture%26Gif/Anchors.gif)

**Pivot**
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; UI元素的旋转，大小和缩放围绕着Pivot来改变，所以中心点的位置影响旋转，大小修改和缩放的结果。当工具栏被设置为Pivot模式时，就可以对Pivot进行拖动。


**Anchors**
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RectTransofrm包含一个叫做Anchors的布局概念。在场景中它的外形像是四个小三角形手柄，它的信息可以在Inspector中查看。如果一个带有RectTransform组件物体的父物体也同样包含RectTransform，那这个子物体的Anchors可以固定到父物体RectTransform中的任何位置。<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Anchors有两个属性**Anchor min**和**Anchor Max**。Anchor min对应左下角的Anchor，Anchor Max对应右上角的Anchor。它们的有效范围值在0~1中间(也就是对应的百分比)。当Anchors完全被分开始时会显示Left, Right, Top 和 Bottom。此时对应的数值是UI元素四条边和Anchors所成矩形的四条边的距离（正负关系是由Anchors所成矩形的四条边减去UI元素四条边），如果Anchors水平拉开，则会显示left和right。如果垂直拉开，则显示top和bottom。