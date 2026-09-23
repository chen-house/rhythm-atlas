# 节奏图鉴 Rhythm · 项目说明与进度

> 位置：`Downloads/leaning/作品集/rhythm-site/`
> 本文件为项目主线记录，随进度更新。最后整理：见对话。

---

## 一、目标

做一个**会不断生长的节奏库网站**：把各类音乐节奏"听得见、也讲得清"。
入口是一张目录，每种节奏类型一页，点开即学。最终发布到 GitHub Pages，可分享、可持续补充。

**每一页的固定结构（三段式）：**
1. **听**：可播放的鼓点网格演示（Web Audio，切换多种律动 + 调速）。
2. **读**：内容讲解（这个节奏怎么运作、历史文化、与其他乐器的配合、给鼓手的落地建议）。
3. **再听**：代表作推荐，分「历史典型 / 现代典型」，每首带音乐家介绍 + 试听链接。

---

## 二、任务拆解

| 模块 | 说明 |
|---|---|
| 站点骨架 | `index.html`（目录）+ 共享 `style.css`；明亮暖色主题 |
| 各节奏类型页 | funk / bossa / jazz / blues / gospel / soul / rnb / cumbia / hiphop … 每类一页 |
| 方法论页 | `method.html`：怎么学一个节奏、听歌如何选节奏、何时做变形 |
| 节奏地图 | `map.html`：3-3-2 → 古巴/巴西家族 → 北上，血缘全景 |
| 发布 | 推到 GitHub `chen-house/rhythm-atlas` + 开 Pages |

加新类型的动作：目录里加一个入口 + 新建一个 html 页（复用 style.css）。

---

## 三、完成标准

- **不编造**：内容先核实再写；链接必须与内容一致；来源就近标注（不堆到文末）。
- **诚实标注局限**：鼓点网格是"抓特征的简化范式"，非逐音符扒带；无法用网格表达的味道（醉拍、靠后 backbeat、swing 比例）明确写出"去原曲用耳朵找"。
- **结构无错**：HTML 标签平衡、JS 无语法错误、可播放网格正常。
- **视觉成套**：各页同一套版式与交互，仅封面色区分节奏。
- **可迁移到用户的练习**：给鼓手的建议要能落到架子鼓练习记录（如"第 4 个 16 分治抢拍""feathering 练轻控"）。

---

## 四、参考链接

**核实用的一手来源（bossa/拉丁家族页内已就近标注）：**
- Tresillo：https://en.wikipedia.org/wiki/Tresillo_(rhythm)
- Habanera：https://hearingtheamericas.org/s/the-americas/page/habanera
- Spanish tinge：https://en.wikipedia.org/wiki/Spanish_tinge
- Clave（Berklee PULSE）：https://pulse.berklee.edu/?id=4&lesson=14
- Bossa nova：https://www.thejazzpianosite.com/jazz-piano-lessons/jazz-genres/how-to-play-bossa-nova/
- Dembow（Berklee）：https://www.berklee.edu/berklee-now/news/what-is-dembow-tracing-the-roots-of-a-global-phenomenon
- Son cubano / Danzón / Samba / Baião / Bateria / Pandeiro：Wikipedia 对应词条

**Emmet's Place 年份核实（jazz 页已改正为 2020–）：**
- DownBeat：https://downbeat.com/news/detail/emmet-cohen-emmets-place-at-the-top
- syos：https://syos.co/en-us/blogs/news/live-from-emmet-s-place-a-21st-century-take-on-a-harlem-tradition

**试听链接方案（歌名+艺人搜索直达，不造 track ID）：**
- 网易云：`https://music.163.com/#/search/m/?s=歌名+艺人`
- Spotify：`https://open.spotify.com/search/歌名+艺人`
- 直播系列类（如 Emmet's Place）：单给 YouTube 搜索链

**用户自有素材（可继续接入）：**
- `music/knowledge/09_曲目库/002_爵士标准曲100首专题.md`
- `爵士新生代_听歌清单.md`（含 knkx / FZINE / Grammy / allmusic 来源）

---

## 五、完成程度

**已建成（内容齐全）：9 个类型页 + 方法论 + 地图 + 目录**

| 页面 | 封面色 | 独有角度 | 结构校验 |
|---|---|---|---|
| funk.html | 橙 | the One、16 分鬼音 | ✅ 平衡 |
| bossa.html | 绿 | 五段递进，3-3-2→古巴/巴西家族 | ✅ 平衡 |
| cumbia.html | 砖红 | 16 分永动机、三大陆合成 | ✅ 平衡 |
| jazz.html | 蓝 | 三连音、乐器分工表 | ✅ 已修复 |
| blues.html | 深红 | shuffle + 12 小节曲式 | ✅ 已修复 |
| gospel.html | 金棕 | 功能性、vamp 推升 | ✅ 已修复 |
| soul.html | 棕红 | 三城打法（底特律/孟菲斯/费城）+ 黑胶推荐卡 | ✅ 已修复 |
| rnb.html | 酒红 | 军鼓 2/4 核心、年代骨架、摇摆量滑杆 | ✅ 已修复 |
| hiphop.html | 紫 | boom-bap / trap | ✅ 平衡 |
| method.html | 紫 | 学/选/变 三问 | ✅ 平衡 |
| map.html | — | 拉丁家族深度页（3-3-2→bossa） | ✅ 平衡 |
| **index.html** | — | **封面：五棵树 = 5 流派，点树进页 + 「完整目录」链 directory** | ✅ |
| directory.html | — | 9 流派 SVG 家族树目录（原 index，改名保留） | ✅ 平衡 |

**站点结构（已接通，0 断链）**：
`index.html 封面(树)` → 5 流派直达 + → `directory.html 目录`(全 9 流派) → 各流派页 / map / method；各页顶栏「返回目录」→ directory，品牌→封面。
封面源码在 `backup/rhythm-cover-gen.js`（Node 生成器），改树参数改它再 `node` 重跑覆盖 index.html。
`backup/` 存放：生成器、node_modules、废弃 v1 封面——不随站点发布。

**血脉主线已互相引用，连起来是一部美国黑人音乐节奏史：**
blues → gospel → soul → R&B → funk（另有 swing、bossa、cumbia、hiphop 支线）。

---

## 六、需要改进与继续

**A. 结构 bug —— ✅ 已修复**
- jazz / blues / gospel / soul / rnb 各缺的 2 个 `</div>`（演示区 `.player` + 推荐区 `#modernlist`）已补齐，全站 12 页 div/section 平衡、JS 无语法错误。

**B. 版式统一（尚未定案）**
- 目前混着三套壳：旧三段式（funk 等）、被另一会话改的新框架（上述 5 页）、更早规划的"唱片行新模板"（bossa/cumbia：分层搭建器 + 翻面唱片卡 + 四唱片箱）。**需要拍板走哪一套，然后统一。**
- soul 页新做的**黑胶唱片推荐卡 + 城市标签**样式，若认可，可回填到其余页。

**C. 内容层面**
- 继续核实各页事实（已抓出并改正：Emmet's Place 年份、soul 三城归属把阿拉巴马录音标「南方」不硬塞）。
- 费城之声正式名 **TSOP（The Sound of Philadelphia）** 可加一行小注。
- 待补类型：reggae/ska、rock、latin 细分等（首页已留占位）。

**D. 发布（未完成）**
- 目标：GitHub `chen-house/rhythm-atlas` + 开 Pages。
- 限制：沙盒能 `git push`，但 `api.github.com` 被代理挡（403），所以**建空仓库、开 Pages 需用户在网页手动操作**；token 由用户提供、用完不存。
- 步骤：① 用户建空仓库 `rhythm-atlas`（不勾任何初始化项）② 贴 token ③ 我推到 main ④ 用户在 Settings→Pages 选 main 分支。

**E. 文件夹清理 —— ✅ 已完成**
- 10 个原型稿与封面草稿（`_*.html` + `rhythm-cover.html`）已移到 `del/` 子文件夹（mv，可找回）。根目录现只剩 12 个正式页 + `style.css` + 说明 md。发布时 `del/` 不要推上去。
