# Fantasy 生命感人像摄影 Skill

拆解了 100 张照片，我终于找到了「生命感」的生成方式。

这一次，完整开源。

这个 Skill 用来把普通游客照、生活随拍、手机废片或参考人像，转化为色彩鲜明、镜头亲密、真实鲜活、适合社交媒体发布的高级生命感人像摄影作品；也可以从零生成原创生命感人像样片、摄影提示词、风格方案和图像编辑指令。

## 模式总览

这个 Skill 主要有两个入口：

| 模式 | 输入 | 适合做什么 | 输出 |
| --- | --- | --- | --- |
| MODE A｜普通照片升级 | 一张普通照片、游客照、生活随拍或手机废片 | 保留原人物，把照片改得更有光影、景深、情绪和摄影完成度 | 图像编辑方向、重绘提示词、氛围感大片方案 |
| MODE B｜最高标准原创样片 | 一个主题、人物设定、场景或风格关键词 | 不依赖原图，从零生成原创生命感人像样片 | 原创人像提示词、成组样片方案、作品集方向 |

## MODE A｜普通照片升级

MODE A 的核心不是“换一张脸”，也不是把普通人重生成陌生模特。

它做的是：

- 保留原人物身份、表情、动作、服装和主要场景关系。
- 重新判断画面的光线、景深、色温、前景、背景和裁切。
- 把原本像随手拍的照片，升级成更像摄影师认真拍过的氛围感大片。

适合输入：

- 天台、街边、咖啡馆、书店、酒店、商场、地铁等日常场景照片。
- 构图普通但人物状态还不错的照片。
- 想保留真实感，但希望画面更高级、更有光影记忆点的照片。

### MODE A 示例图

<table>
  <tr>
    <th>原图</th>
    <th>升级后</th>
  </tr>
  <tr>
    <td><img src="assets/atmosphere/rooftop-before.jpg" alt="天台人像原图" width="330"></td>
    <td><img src="assets/atmosphere/rooftop-after.jpg" alt="天台人像升级后效果" width="330"></td>
  </tr>
  <tr>
    <td><img src="assets/atmosphere/cafe-before.jpg" alt="咖啡馆人像原图" width="330"></td>
    <td><img src="assets/atmosphere/cafe-after.jpg" alt="咖啡馆人像升级后效果" width="330"></td>
  </tr>
  <tr>
    <td><img src="assets/atmosphere/bookstore-before.jpg" alt="书店人像原图" width="330"></td>
    <td><img src="assets/atmosphere/bookstore-after.jpg" alt="书店人像升级后效果" width="330"></td>
  </tr>
</table>

这类改造的判断顺序是：

**保留人物身份**  
→ **保留原始事件**  
→ **重新组织光线**  
→ **拉开主体和背景层次**  
→ **加入环境氛围记忆点**  
→ **最后做克制的质感增强**

## MODE B｜最高标准原创样片

MODE B 不需要上传原图。

它适合在你只有一个主题、一个场景、一个人物方向时，从零生成一组原创生命感人像。它会重新设计人物、事件、镜头、光线、色彩和质感，而不是反复套用同一种美女、同一种花海、同一种伸手动作。

适合输入：

- “夏日、逆光、年轻女性、近距离镜头”
- “老人、亮色丝巾、街头硬光、时髦一点”
- “儿童、风车、奔跑、低机位、高饱和”
- “书店、回头、暖色灯光、浅景深”

### MODE B 示例图

MODE B 的默认审美更偏鲜明、明亮、亲密、高饱和、高对比。它会优先生成有镜头吸引力的女性人像，但不会固定成同一张网红脸，也不会把所有画面都做成同一种动作和场景。

<table>
  <tr>
    <td><img src="assets/showcase/life-force-elderly-color.jpg" alt="老人、强阳光和鲜明色彩的人像样片" width="260"></td>
    <td><img src="assets/showcase/life-force-child-motion.jpg" alt="儿童、风车和奔跑感的人像样片" width="260"></td>
    <td><img src="assets/showcase/life-force-close-reach.jpg" alt="近距离伸手、花朵前景和阳光的人像样片" width="260"></td>
  </tr>
  <tr>
    <td><img src="assets/showcase/life-force-male-sun.jpg" alt="男性、硬光和街头现场感的人像样片" width="260"></td>
    <td><img src="assets/showcase/life-force-foreground-umbrella.jpg" alt="透明伞前景、雨水和遮挡的人像样片" width="260"></td>
    <td><img src="assets/showcase/life-force-water-caustics.jpg" alt="泳池、水花和焦散质感的人像样片" width="260"></td>
  </tr>
</table>

### MODE B 更多女性样片

<table>
  <tr>
    <td><img src="assets/showcase/mode-b/strawhat-lake-closeup.jpg" alt="草帽、湖边和花朵前景的原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/soft-window-portrait.jpg" alt="柔光窗边原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/mountain-braid-portrait.jpg" alt="雪山、辫子和蓝天的原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/ethnic-silver-portrait.jpg" alt="民族服饰和银饰的原创女性人像样片" width="220"></td>
  </tr>
  <tr>
    <td><img src="assets/showcase/mode-b/lavender-field-portrait.jpg" alt="花田前景和浅景深的原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/fruit-garden-portrait.jpg" alt="递水果事件感的原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/flower-basket-reach.jpg" alt="花篮、伸手和近距离镜头的原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/blue-fabric-sun.jpg" alt="蓝色布料前景和阳光遮挡的原创女性人像样片" width="220"></td>
  </tr>
  <tr>
    <td><img src="assets/showcase/mode-b/red-board-motion.jpg" alt="红色道具和动态构图的原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/snow-red-scarf.jpg" alt="雪地、红围巾和高饱和色彩的原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/horse-travel-portrait.jpg" alt="马、旅行感和近距离镜头的原创女性人像样片" width="220"></td>
    <td><img src="assets/showcase/mode-b/spring-water-closeup.jpg" alt="泉水、硬光和水花质感的原创女性人像样片" width="220"></td>
  </tr>
</table>

## “生命感”到底是什么？

一开始，我也以为它只是一种调色。

高饱和、强对比、阳光、柔光、色散、风吹头发，这些特征确实经常出现。但只要单独模仿它们，画面很快就会变成：颜色很鲜艳，人物却还是没有活起来。

因为「生命感」不是某一种滤镜，而是人物、镜头和环境同时发生了关系。

> 生命感不是一种风格，而是一种正在发生的状态。

## 三个共同点

**01 人物不是在摆姿势**

他们在笑、回头、奔跑、挡太阳、递东西、推门、吃水果。动作不一定复杂，但一定能让人感觉到这一秒之前和之后还会继续发生。

**02 镜头不是旁观者**

手、花、布料、玻璃和植物会闯进画面，人物也可能贴得很近、被遮挡、被裁切。镜头像是参与到了现场。

**03 光线不是简单照亮**

硬光、逆光、树影、反射和色散，会真正落在人物皮肤和环境上。它们不是滤镜装饰，而是现场的一部分。

## 这不是一段万能提示词

我把「生命感写真」拆成了四层判断。

**第一层：人物层**

这一张照片里是谁？儿童、年轻人、中年人还是老人？不同年龄的人，不应该共享同一套动作和表情。

儿童更适合失控、好奇和奔跑；年轻人可以松弛、搞怪、靠近镜头；老人也可以时髦、酷，甚至有一点锋利。

**第二层：事件层**

他此刻正在做什么？

不是「站在花海里」，而是「把风车突然伸向镜头」。不是「坐在院子里」，而是「递来一块刚切开的水果」。

> 先确定事件，再生成照片。

**第三层：镜头层**

镜头离人物多近？是平视、低机位，还是轻微仰拍？

前景里有没有东西？脸需不需要完整出现？动作要不要冲出画面边缘？

这个 Skill 会让每一张照片重新选择拍摄距离、机位、遮挡和构图。

**第四层：质感层**

最后才处理高饱和与高对比、焦散柔光、轻微色散、旋焦、运动模糊和胶片空气感。

这些效果不能每张全部出现，而是根据场景选择一到两种。

> 质感是最后一层，不是生命感的起点。

## 工作流程

输入一个主题或一张普通照片后，Skill 会依次判断：

**人物是谁**  
→ **这一刻发生什么**  
→ **镜头如何靠近**  
→ **前景如何介入**  
→ **光线落在哪里**  
→ **用什么颜色建立记忆点**  
→ **最后加入哪一种镜头质感**

一句话流程：

> 人物 → 事件 → 镜头 → 光色 → 质感

所以它不会只生成同一种美女、同一种花海、同一种伸手动作、同一种滤镜。每一次都应该重新建立人物、事件、镜头和环境之间的关系。

## 可以用来做什么

- 生成不同年龄段的生命感写真。
- 为普通生活照提供二次构图与调色方向。
- 把普通照片升级成更有光影、景深和电影感的氛围感大片。
- 分析参考图的摄影语言，但不复制人物、场景和构图。
- 建立更丰富的动作、镜头和场景组合。
- 为 AI 图像生成或图像编辑整理更清晰的摄影提示词。

## 使用方式

将本仓库作为 Codex Skill 使用：

```bash
git clone https://github.com/dacnay816y62-hub/fantasy-life-force-portrait-photography.git
```

把仓库目录放入你的 Codex skills 目录后，即可在对话中这样触发：

```text
使用 Fantasy 生命感人像摄影 Skill，把这张普通生活照升级成更有生命感的人像。
```

普通照片变氛围感大片：

```text
使用 Fantasy 生命感人像摄影 Skill，保留人物身份和原场景，把这张普通照片改成有光影、景深和电影感的氛围感大片。
```

也可以用于从零生成：

```text
使用 Fantasy 生命感人像摄影 Skill，生成一组夏日、儿童、逆光、近距离镜头的原创生命感人像提示词。
```

## 边界

- 不换脸，不把普通人改成陌生模特。
- 不明星化，不复制真实人物的具体长相。
- 不用滤镜替代摄影判断。
- 不追求整齐摆拍的 AI 广告图。
- 参考图只用于分析摄影语言，不用于复刻人物、场景和构图。

AI 生成照片时，到底应该先生成「好看」，还是先生成「活着」？

拿一张你觉得很普通的照片来试试，看看它还能不能被重新看见。
