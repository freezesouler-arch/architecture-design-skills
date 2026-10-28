# 白模提示词模板

用项目实际信息替换尖括号内容；删去不适用项，不带着占位符调用。

## 通用中文

以输入图1为唯一几何与相机依据，深化为精细建筑事务所白模分析渲染。<图2若存在，仅作风格参考，不引入其布局或构件。>

建筑采用哑光暖白色，保留原有立面分格、檐口、栏板、屋顶与入口细节；玻璃浅灰半透明。植物为精细白色叶片，保持原有树种形态、位置与高度，针叶树保持针叶。草地低饱和淡灰绿，铺装浅灰，水面平静淡蓝灰。柔和自然光，轻盈且有层次的阴影，干净清晰、淡雅克制。

严格保持原图相机、透视、朝向、画幅比例与裁切。不得改变楼栋数量、位置、轮廓、尺度、层数、高低错落、楼间距及立面开口；入口、花园、水池、河道、桥梁、运动场与景观节点的几何关系不变。不新增构件、植被、人物或水域。<本图独有锚点。>

只在原有水域表达水面。河道对岸的陆地必须连续，不把建筑后方陆地补成水或孤岛；青色运动场、铺装和竖向池壁不是水面或瀑布。树木贴图不是建筑片墙。圆环亭保留中庭开口。车辆保持室外位置，不进入大堂。

用光照与材质取代黑色建模描边，避免粗白盒、塑料高光、黑重树影、过曝、重纹理、颗粒和锐化光晕。不加文字、Logo、水印或边框。

## English equivalent

Use case: style-transfer.
Input 1 is the sole geometry and camera authority. <Input 2 is style only; never import its layout.>
Create a refined architectural-office white-clay analysis render. Matte ivory-white architecture; preserve existing facade bays, cornices, roofs and entrances. Pale-gray translucent glazing, detailed white foliage preserving species/positions/heights, pale gray-green lawns, light-gray paving, calm pale blue-gray water. Soft natural daylight, gentle readable shadows, clean restrained luminous atmosphere.
Strictly lock input camera, projection, orientation, framing and aspect ratio; every building count, footprint, position, scale, floor count, stepped height, spacing and opening; all entrance, garden, pool, pavilion, court, riverbank and bridge geometry. <View-specific anchors.> Do not redesign or add objects.
Water ONLY within original water boundaries. Far-bank towers sit on continuous dry mainland, not islands; no blue water outside the original river. Cyan courts and paths are land facilities. Vertical pool walls are not waterfalls; tree billboard planes are not walls; ring pavilions retain open centers. Cars remain outside the lobby.
Replace sketch outlines with physical shading. Avoid grain, harsh black shadows, overexposure, plastic shine, oversharpening, invented facade detail, text, logos and borders.

## 按视图补充，非默认改设计

- 整体鸟瞰：<本图幼儿园/配套在左下或右下>；<主河道在何侧>；<高层、洋房、叠墅分布>。背景体块保留简模，主体按原分格细化，不用风格参考的低层替换当前住宅。
- 近景鸟瞰：明确可见的入口—公共花园—水庭—亭廊顺序；保留被树遮住的空间尺度，不能靠加树抹平节点。
- 俯视：保持原有旋转方向和投影，不自动北向上；水池长宽、台地、座椅与环亭开口清楚可读。
- 入口人视：保留原入口体量、雨棚及落客/步行关系，不增高门厅、不把车移入室内，不增加遮挡通道的片墙。
- 水庭人视：保留现有树种、池边、岛式树池、台阶、座椅；竖向池壁用白色实体表达，只有原模型有跌水才表达跌水。

## 定点修复：误扩水域示例

Use case: precise-object-edit.
Image 1 is the render to fix; Image 2 is authoritative source geometry.
Change ONLY <错误区域>. Replace the incorrect water behind the far-bank context towers with continuous pale gray-green dry land matching Image 2. Preserve the original river width and banks, bridges, all buildings and trees, camera, geometry and lighting. Do not add islands, pools or new paths. Keep the rest of Image 1 as unchanged as possible.

## 提示词归档

每图保存：输入底图路径/版本、参考图角色、最终主提示词、修复提示词（如有）、选定输出路径、服务/模式、实际像素宽高。前后方案与相机不同，应分别记录，不用通用提示词掩盖输入差异。
