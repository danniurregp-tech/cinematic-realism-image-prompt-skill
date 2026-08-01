# 真实感与负面提示

## 降低 AI 味的核心方法

### 1. 不要用“质量词”代替结构

低效：

> masterpiece, 8K, best quality, super detailed

有效：

> 肩胛骨随前肢发力向上推起；湿毛贴在胸肌和前臂上；水面在爪子前方形成两层波纹；后腿仍被水面遮住。

### 2. 让环境影响主体

- 红墙向皮肤反射轻微暖色；
- 冷白荧光灯只照亮异兽背部；
- 水面向动物下颌提供微弱冷色反光；
- 雨水压低毛发并沿骨角滴落；
- 泥地被脚掌压出形变；
- 风只吹动较轻的袖口和碎发。

### 3. 让主体影响环境

- 老虎前爪推动水体；
- 异兽遮挡灯光并投下阴影；
- 人物衣摆扫过花瓣；
- 动物身体打断水面倒影；
- 呼吸使近处雾气产生微弱扰动。

### 4. 控制完美度

避免：

- 对称脸；
- 对称兽角；
- 每朵花一致；
- 所有毛发同样清晰；
- 所有区域同样亮；
- 所有材质都光滑；
- 主体永远位于画面中心。

## 通用负面提示词

按任务选择，不要无差别全部堆入：

- AI generated look
- digital painting
- oil painting
- illustration
- anime
- game CGI
- concept art
- plastic texture
- waxy skin
- oily fur
- metallic fur
- oversharpening
- excessive HDR
- fake bokeh
- artificial Gaussian blur
- uniform lighting
- unexplained rim light
- glowing eyes
- magic particles
- oversaturated colors
- teal-orange filter
- poster composition
- perfect symmetry
- duplicated objects
- malformed anatomy
- extra limbs
- floating subject
- incorrect reflection
- inconsistent shadows

## 人物专项

避免：

- AI 网红脸；
- 欧美化骨相；
- 尖下巴；
- 夸张大眼；
- 塑料皮肤；
- 过度磨皮；
- 假睫毛；
- 浓重影楼妆；
- 手指错误；
- 不自然肩颈；
- 没有重量的衣服；
- 正中站立摆拍；
- 刻意摸花、闻花、看镜头。

## 动物专项

避免：

- 毛发像油漆或金属；
- 条纹/斑纹不随身体结构弯曲；
- 肌肉像健美人体；
- 肩胛、肘部和后腿关节错误；
- 爪子悬浮；
- 牙齿过白；
- 发光眼睛；
- 总是咆哮；
- 怪兽海报式仰拍；
- 毛发每根都被锐化。

## 异兽专项

避免：

- 多种动物机械拼装；
- 左右绝对对称；
- 每个部位都有装饰纹；
- 金色光环；
- 火焰翅膀；
- 盔甲式皮肤；
- 没有呼吸和重量；
- 灯光不影响它；
- 地面没有阴影和接触；
- 与背景清晰度、噪点或色温不一致。

## 水中场景专项

避免：

- 水花像玻璃雕塑；
- 水滴大小完全一致；
- 水面不受身体影响；
- 身体下半部穿透水面；
- 倒影完整而不被波纹破坏；
- 湿毛仍然蓬松；
- 水下结构异常清晰；
- 水珠没有运动方向；
- 水花遮挡全部肌肉结构；
- 所有水滴同时冻结且边缘超锐。

## “油感”的来源与修正

常见来源：

- 全身均匀镜面高光；
- 高饱和暖色；
- 微对比和锐化过强；
- 毛发被描述为“闪耀、光滑、发光”；
- 湿润效果没有区分毛束和皮肤；
- 高光没有光源方向。

修正：

- 写“碎片化局部高光”；
- 保留大面积哑光毛发；
- 高光只出现在朝向主光的湿毛束；
- 暗面毛发保持低反射；
- 降低饱和度与局部对比；
- 使用 soft highlight roll-off 和 subtle optical softness。
