# Fantasy 生命感人像摄影

**FANTASY / 梵想美学 · 摄影与照片转译**

围绕人物状态、事件、亲密镜头和光色关系，升级生活照或构建原创电影化人像。新增 **MODE D 胶片模式**：支持自然颗粒、柔高光、浓影和不同光线下的生活胶片观感。

**[快速开始](#start)** · **[胶片模式](#film)** · **[下载与安装](#install)** · **[完整规则](SKILL.md)** · **[全部视觉 Skills](https://github.com/dacnay816y62-hub?tab=repositories)**

| 视觉示例 01 | 视觉示例 02 |
| :---: | :---: |
| ![Fantasy 生命感人像摄影 · 示例 1](assets/atmosphere/rooftop-before.jpg) | ![Fantasy 生命感人像摄影 · 示例 2](assets/atmosphere/rooftop-after.jpg) |

<a id="start"></a>

## 一分钟开始

| 你提供 | 这套 Skill 组织的交付 |
| --- | --- |
| 生活照、参考人像或一个拍摄主题 | 保留身份的照片升级，或原创人像方向与样片 |

```text
用 $fantasy-life-force-portrait-photography 处理这张生活照。保留人物身份、表情、服装与原场景，重新组织光线和景深，让人物状态自然，面部干净清透。
```

**生成说明：** Skill 组织设计判断、提示词与执行流程；图片由当前环境中可用的图像工具生成或编辑。示例用于理解视觉方向，具体来源以本仓库记录为准，不能据此保证每次得到相同效果。

胶片模式可以直接这样调用：

```text
用 $fantasy-life-force-portrait-photography 开启胶片模式，处理这张照片。保留人物、动作、衣服、场景和原构图；按原光线选择配方，增加细密自然颗粒，柔化高光，保留黑位与真实肤色。
```

<a id="install"></a>

## 下载与安装

**[下载当前分支 ZIP](https://github.com/dacnay816y62-hub/fantasy-life-force-portrait-photography/archive/refs/heads/main.zip)** · **[阅读 Skill 规则](SKILL.md)**

1. 下载并解压仓库。
2. 将仓库根目录（包含 `SKILL.md`）放入当前助手支持的技能目录。
3. 安装文件夹命名为 **`fantasy-life-force-portrait-photography`**，确保入口是 `fantasy-life-force-portrait-photography/SKILL.md`。
4. 在支持技能调用的会话中使用 **`$fantasy-life-force-portrait-photography`**。如果列表未刷新，新开一个任务。

Codex CLI / IDE 的用户级目录是 `~/.agents/skills/`，项目级目录是 `.agents/skills/`；Windows 用户目录可写为 `%USERPROFILE%\.agents\skills\`。以 [OpenAI 官方安装说明](https://learn.chatgpt.com/docs/build-skills#where-codex-loads-local-skills) 为准。ChatGPT 与其他宿主请按各自的技能加载方式使用。

仓库名与调用名可能不同，以上以 `SKILL.md` 中的名称为准。安装不包含图像服务、账户或生成额度；实际出图取决于你使用的环境。

---

## 模式总览

支持照片升级、原创样片、氛围增强和胶片模式。A/B/C 保留原默认风格；只有指定胶片观感时切换 D：

| 模式 | 输入 | 适合做什么 | 输出 |
| --- | --- | --- | --- |
| MODE A｜普通照片升级 | 一张普通照片、游客照、生活随拍或手机废片 | 保留原人物，把照片改得更有光影、景深、情绪和摄影完成度 | 图像编辑方向、重绘提示词、氛围感大片方案 |
| MODE B｜最高标准原创样片 | 一个主题、人物设定、场景或风格关键词 | 不依赖原图，从零生成原创生命感人像样片 | 原创人像提示词、成组样片方案、作品集方向 |
| MODE C｜氛围增强 | 一张希望保留人物与事件的生活照 | 重点调整光线、景深与环境气氛 | 保留身份和事件的氛围感图像编辑方向 |
| MODE D｜胶片模式 | 原片、拍摄主题或胶片风格参考 | 根据光线模拟颗粒、影调、高光、色彩与扫描质感；支持同人连续组照 | 保留身份的胶片编辑、原创胶片样片或提示词 |

<a id="film"></a>

## MODE D｜胶片模式

胶片模式把颗粒、柔高光、有密度的暗部、肤色与环境色分离、轻柔的镜头微反差一起考虑。它支持明亮日晒、室内近照、浓影硬光和安静的生活瞬间；不用统一泛黄、全幅灰雾或大噪点表达“复古”。

| 配方 | 适合的画面 | 主要质感 |
| --- | --- | --- |
| F01 温润日常 | 厨房、咖啡馆、窗边 | 米白木色、自然暖肤、中细颗粒 |
| F02 晴日空气 | 明亮街巷、海边、白墙 | 奶油白、柔青蓝、日晒感与柔高光 |
| F03 室内颗粒 | 车内、沙发、近距离生活照 | 明显而细密的颗粒、暖肤、冷灰环境、深黑 |
| F04 暖光逆照 | 逆光旅行、窗边关系照 | 有光源依据的局部光幕、透光发丝与浓暗部 |
| F05 浓影硬光 | 木门、树影、强日光 | 暖亮面、冷深影、大光比与柔高光顶端 |
| F06 森林绿 | 草地、林下、乡间 | 绿色分层、米桃肤色、细颗粒 |
| F07 家庭相册 | 家庭日常、儿童活动 | 鲜活红蓝点色、温暖自然与生活抓拍 |
| F08 清透微颗粒 | 树荫近照、花间侧光、玻璃反射 | 极细弱颗粒、清楚肤质、克制色调 |

强度支持 **轻 / 标准 / 浓**，默认标准。可单独指定“颗粒更明显”“高光更柔”“保留黑位”“不要光晕”或“只要胶片色彩，不加颗粒”；不会因此把每种效果同时拉满。

```text
用 $fantasy-life-force-portrait-photography，胶片模式 F03 室内颗粒，标准强度。保留这张原片的表情和构图，颗粒可见但不要变成雀斑，不要泛黄，不要光晕。
```

```text
用 $fantasy-life-force-portrait-photography，生成同一个成年人物的 3 张咖啡馆胶片组照，F01 温润日常。保持人物、衣服与调色连续，变化景别和生活动作，每张独立输出。
```

高光会区分三件事：亮部柔溢 **bloom**、极轻暖边 **halation**、有方向的镜头眩光 **flare**。它们按现场光源启用，阴天或普通树荫不强加太阳光斑；自然光照亮皮肤也不等于把皮肤做成油膜。

这次升级分析了 20 张上传参考，其中第 17、18 张重复，共 19 份独立参考。第 7、13 张的明显颗粒较弱，主要用于清透肤色与光线分支。仅凭这些经过处理的图片无法确认实际胶片、ISO 或冲扫流程；八个配方是自定义视觉模拟，不是某品牌胶片的精确测量还原。

**[逐图分析](references/film-reference-analysis.md)** · **[胶片执行规范](references/film-mode.md)** · **[提示词模板](references/film-prompts.md)**

原始参考照片不随仓库发布。现有下方图库仍为原模式示例，不代表新版胶片模式的实测输出。

**测试状态：** 首轮胶片样片被反馈“没有胶片感”；后续校准仍出现数码锐度残留、过度柔焦和伪颗粒纹路。已据此补充实际参考图输入、同尺度对比和失败判定规则，尚未将这批结果列为合格胶片样片。见 [测试记录与限制](references/film-validation-notes.md)。

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

MODE B 的默认审美不是街头纪实，而是“唯美的电影化人像大片”：默认中国/东亚人物，高饱和、高对比、镜头效果明确，人物漂亮但不油腻，画面有电影情境和光学记忆点。面部必须干净清透，皮肤是柔润哑光，不是油亮反光；人物地域与面貌以当前用户要求为准；避免脏脸、过量油光和模板化网红修图。

新版 MODE B 会刻意避开几类容易跑偏的结果：

- 不默认外国人或欧美广告模特脸。
- 不把题材拍成街头摄影、普通纪实或粗粝生活抓拍。
- 不做影楼写真、网红写真或廉价广告摆拍。
- 不把老人或劳动者拍成暗黑炉火、硬汉工匠广告、沉重男性肖像。
- 不把“清透皮肤”做成油光皮肤：额头、鼻梁、脸颊、下巴不能大片镜面反光。
- 不把人脸做成 AI 娃娃脸、完美白瓷脸、统一大眼小脸模板。
- 优先让水花、玻璃、布料、发丝和背景散景承担镜头效果，脸部保持自然松弛。
- 先建立一个唯美电影情境，再加入强色彩对比、侧逆光、焦散、色散、旋焦、前景遮挡等镜头效果。

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

原模式的镜头效果根据场景选择一到两种。胶片模式将颗粒、曲线和配色作为成像基础，附加光晕可以关闭，不强制加入色散。

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
- 把生活照处理成不同颗粒与高光观感的胶片风格，或生成同一人物的连续胶片组照。
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
- 不做油腻审美：避免油亮皮肤、满脸高光、水光肌过度、湿身诱惑、媚态姿势、夜店霓虹和擦边网红感。
- 不默认生成外国人，不做欧美广告模特脸。
- MODE B 要唯美，但不能变成廉价影楼写真；优先电影化人像大片、人物情境和镜头效果。
- 面部不能脏也不能油：避免灰脸、黑脸、脏黄暗部、重对比、HDR 脏纹理、额头鼻梁脸颊大片反光。
- 参考图只用于分析摄影语言，不用于复刻人物、场景和构图。

以上默认审美在 D 中按胶片配方调整：允许普通衣服、自然素颜、可见颗粒、生活抓拍、浓影与合理受光面；保留身份和真实肤质。编辑原片保持原人物，同人组照保持连续性，不执行原创样片的换脸差异要求。

AI 生成照片时，到底应该先生成「好看」，还是先生成「活着」？

拿一张你觉得很普通的照片来试试，看看它还能不能被重新看见。

## FANTASY / 梵想美学

**让想象先被看见。** 将视觉判断与创作流程整理成可以继续使用的方法。

**[浏览全部视觉 Skills](https://github.com/dacnay816y62-hub?tab=repositories)** · [Character Casting Studio](https://github.com/dacnay816y62-hub/character-casting-studio-skill) · [Street Photo Illustration](https://github.com/dacnay816y62-hub/street-photo-illustration-skill)
