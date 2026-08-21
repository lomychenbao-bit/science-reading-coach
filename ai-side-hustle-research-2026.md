# AI 自动化副业深度调研报告

> 调研目标：找到**主要消耗 AI tokens、人类参与极少**的副业模式
> 调研日期：2026-06-14
> 约束条件：有 Coding Plan，不能太简单（如做游戏需动手多），重点关注卖素材等方向

---

## 总览：按「Token 消耗量 x 人类参与度」评估

| 排名 | 副业方向 | Token消耗 | 人类参与 | 现实月收入 | 启动难度 | 推荐度 |
|------|----------|-----------|----------|------------|----------|--------|
| 1 | AI 素材/模板批量售卖 (Etsy/Gumroad) | 高 | 低 | $500-$2,500 | 低 | 5/5 |
| 2 | AI 图库图片批量上传 (Adobe Stock等) | 很高 | 低 | $200-$1,500 | 低 | 4/5 |
| 3 | AI 自动化 Niche 网站 + 联盟营销 | 很高 | 中 | $500-$5,000 | 中 | 4/5 |
| 4 | AI 短视频批量生产 (抖音/YouTube) | 高 | 中 | 500-10,000RMB | 中 | 3/5 |
| 5 | AI Prompt 包/工具包售卖 | 中 | 低 | $200-$3,000 | 低 | 4/5 |
| 6 | GPT Wrapper / Micro-SaaS | 很高 | 高 | $0-$100,000 | 高 | 3/5 |
| 7 | AI 自动化工作流服务 (n8n) | 中 | 高 | $1,000-$10,000 | 中 | 3/5 |
| 8 | AI 有声书/播客自动化 | 高 | 低 | $100-$1,000 | 中 | 3/5 |
| 9 | AI KDP 低内容书籍 (涂色书等) | 中 | 低 | $100-$2,000 | 低 | 3/5 |
| 10 | AI 自动化 POD (Print-on-Demand) | 高 | 低 | $500-$3,000 | 中 | 4/5 |

---

## 第一梯队：强烈推荐（Token 消耗大 + 人类参与少 + 可行）

---

### 1. AI 素材/数字模板批量售卖 (Etsy/Gumroad) -- 最推荐

#### 模式
用 AI 批量生成数字产品模板，上架到 Etsy/Gumroad，实现"一次制作、反复销售"。

#### 具体产品类型
- **Planner/日程管理模板**：ADHD planner、fitness tracker、budget planner
- **Notion 模板**：项目管理、习惯追踪、CRM、财务规划
- **Canva 模板**：社交媒体模板包、简历模板、名片模板
- **PPT 演示模板**：商业提案、教育课件、营销方案
- **电子表格模板**：财务追踪、库存管理、项目计划
- **Digital Paper/数字纸**：花纹纸、背景纸、季节主题纸
- **Seamless Pattern/无缝图案**：面料花纹、壁纸图案、包装纸设计

#### 实际收入数据
- **$2,522/月** (Medium 博主实测)：Etsy $1,430 + Gumroad $1,092
- 主要时间投入：**每月约一个下午**上传新产品
- 从第一笔 $27 做到 $2,500/月，逐步积累
- 不需要已有粉丝、不需要付费推广、不需要库存

#### Token 消耗分析
- **市场调研**：用 LLM 分析热门搜索词和竞品缺口（每次约2K tokens）
- **内容生成**：批量生成模板文案、描述、标签（每个产品约1K tokens）
- **预览图生成**：AI 生成产品预览图（每次约500 tokens）
- **批量放大**：从一个母模板批量生成多个主题变体
- **估计日消耗**：50K-200K tokens/天（取决于批量规模）

#### 工作流自动化方案
```
[LLM 市场调研] -> [Canva API 批量生成模板] -> [AI 生成预览图] -> [自动上架 Etsy/Gumroad]
       ^                                                                              |
[每月检查销量 & 调整方向] <-------------------------------------------------------------+
```

#### 自动化程度：80%+
- 初始搭建需要 1-2 周
- 之后每月仅需几小时检查和调整
- Canva 的批量创建功能可以从一个模板快速生成几十个变体

#### 关键成功因素
- **Niche 选择**：ADHD planner、婚礼策划、宠物护理等垂直领域
- **SEO 优化**：正确使用 Etsy 标签和关键词
- **季节性**：提前准备节日/季节主题（圣诞、开学季、新年等）
- **差异化**：不要做通用模板，要做细分场景

#### 风险提示
- 竞争日趋激烈，需要持续找新 niche
- 平台可能限制纯 AI 生成内容
- 初期收入可能很低（$0-$100/月），需要 3-6 个月积累

---

### 2. AI 图库图片批量上传 (Adobe Stock / Shutterstock / Freepik)

#### 模式
用 AI (Midjourney/DALL-E/Stable Diffusion) 批量生成高质量图片，上传到图库平台，按下载收费。

#### 实际收入数据
- **Adobe Stock 约$7,300/年** (Reddit 用户2025年真实数据)
- **Shutterstock 约$1,069/年**（同一用户，Shutterstock 上传少）
- **13,000+ AI 图片**在 Adobe Stock 上（一个创作者 9 个月的积累）
- 单张收入很低（$0.01-$0.50/次下载），靠量取胜

#### Token/算力消耗分析
- **本地 Stable Diffusion**：无 token 消耗，主要是电费/显卡折旧
- **Midjourney**：$10-60/月订阅，不限量生成
- **DALL-E API**：约$0.02-0.08/张，批量 1000 张 = $20-80
- **Flux/其他 API**：类似成本

#### 工作流
```
[关键词研究] -> [批量 prompt 生成] -> [AI 批量出图] -> [质量筛选] -> [批量上传+标注]
     |                |                  |              |               |
  LLM tokens      prompt模板        SD本地/API      人工5-10%      Adobe Stock API
```

#### 自动化程度：75%+
- 批量生成可完全自动化（ComfyUI workflow）
- 上传可通过 Adobe Stock API 自动化
- 唯一需要人工的是质量筛选（但可以快速浏览跳过）

#### 最佳品类
- **商业场景**：办公室、团队协作、远程工作
- **概念插画**：AI/科技/区块链/未来主题
- **背景/纹理**：抽象背景、自然纹理、几何图案
- **季节性**：节日、四季、天气
- **多元文化**：不同种族/文化场景（市场缺口大）

#### 关键注意
- Adobe Stock 要求标注 AI 生成内容
- 质量要求较高，手指/文字等细节不能有 AI 瑕疵
- 需要持续上传保持曝光，建议每周 50-200 张
- Getty + Shutterstock 合并（2025年），市场格局在变化

---

### 3. AI 自动化 Niche 网站 + 联盟营销 (Affiliate Marketing)

#### 模式
用 AI 批量生成某个垂直领域的内容网站，通过 SEO 获取自然流量，再通过联盟营销链接变现。

#### 收入数据
- 成功 Niche 网站：$500-$5,000/月（6-12个月建设期）
- 程序化 SEO (Programmatic SEO)：有人 3 小时建 13,000+ 页面
- 但 Google 在 2025-2026 年大幅打击纯 AI 内容农场

#### Token 消耗分析
- **极高**：每篇文章约3K-5K tokens
- 1000 篇文章 = 3-5M tokens 生成成本
- 加上关键词研究、内链优化等，总消耗更大
- **月消耗**：1M-10M tokens（规模化运营）

#### 现实评估
| 优势 | 劣势 |
|------|------|
| 消耗 token 多 = 自动化程度高 | Google 打击 AI 内容越来越严 |
| 一旦排名上去，收入很被动 | 建设期长（6-12个月） |
| 可以程序化批量生成 | 需要一定的 SEO 知识 |
| 联盟营销佣金可观 | 纯 AI 内容质量不够，需要人工润色 |

#### 可行方案
- **最佳路径**：AI 生成 80% + 人工编辑 20%
- 用程序化 SEO 做比较/评测类内容（"best X for Y"）
- Niche 选择要精准：如"best standing desk for short people"
- 配合 YouTube/社交做内容矩阵

#### 自动化程度：60%
- 内容生成可自动化，但 SEO 优化和质量管理需要人工
- 需要持续监控 Google 算法变化

---

## 第二梯队：值得尝试

---

### 4. AI 短视频批量生产

#### 工具
- **MoneyPrinterTurbo** (GitHub 44K+ stars)：一键生成 HD 短视频
- **MoneyPrinterPlus**：支持批量发布到抖音/快手/小红书/视频号
- **ComfyUI + AnimateDiff**：更高质量的视频生成

#### 收入模式
- 平台创作激励（抖音/B站/YouTube）
- 带货佣金
- 账号矩阵变现

#### 现实评估
- **收入不稳定**：受平台算法影响极大
- **平台限流风险**：AI 内容可能被降权
- **法律风险**：2026 年有博主因搬运 300 条 AI 视频被判赔 100,000 RMB
- **质量瓶颈**：自动生成的视频缺乏创意和连贯性
- 需要人工筛选主题、审核质量

#### Token 消耗
- 脚本生成：LLM tokens
- TTS 配音：API 消耗
- 素材搜索/生成：多模态模型消耗
- **日消耗**：100K-500K tokens（批量生产）

#### 自动化程度：50-60%
- 视频生成自动化程度高
- 但质量把控和发布策略需要人工参与
- 不建议完全自动化，容易被平台检测

---

### 5. AI Prompt 包/工具包售卖

#### 模式
将精心设计的 AI prompt 打包成产品，在 Etsy/Gumroad/PromptBase 上售卖。

#### 产品类型
- **Midjourney Prompt 包**：特定风格（水彩、赛博朋克、产品摄影等）
- **ChatGPT Prompt 包**：特定职业（营销人、教师、程序员等）
- **Stable Diffusion Prompt + 参数包**
- **完整工作流模板**：ComfyUI workflow + prompt 组合

#### 收入数据
- 单个 Prompt 包售价 **$9-$47**
- 头部创作者月入 **$3,000+**（但需要大量营销）
- 普通创作者 **$100-$500/月**

#### 自动化程度：70%
- 可以用 AI 自动生成和优化 prompt
- 测试和验证需要一些人工
- 产品交付完全自动

#### 注意
- 市场正在饱和
- 需要差异化（垂直领域、独特风格）
- PromptBase 竞争激烈，Etsy 可能更有利

---

### 6. AI POD (Print-on-Demand) 自动化

#### 模式
AI 生成设计图案 -> 上传到 Redbubble/Merch by Amazon/TeePublic -> 用户下单后平台自动印制发货

#### 收入数据
- **8,000 个设计**在 Merch by Amazon：$2,000-$3,000/月
- **5,000+ 销售**通过 AI + 自动化 scaling Redbubble
- 旺季（圣诞）收入翻倍

#### Token/成本分析
- AI 设计生成：Midjourney $10-60/月 或本地 SD
- 自动化上传工具：Merch Titans / PODTurbo $20-50/月
- 无库存、无物流成本

#### 自动化程度：75%
- 设计生成可批量自动化
- 上传可通过工具自动化
- Niche 研究和趋势跟踪需人工

#### 关键成功因素
- 量大取胜：需要数千个设计
- Niche 选择：节日、爱好、职业、meme
- 趋势敏感：快速跟热点

---

## 第三梯队：高风险或高参与度

---

### 7. GPT Wrapper / Micro-SaaS

#### 现实评估
- **90% 的 AI wrapper 创业将在 2026 年底前失败**
- **60-70% 产生零收入**
- 但成功案例：$10K-$100K/月（极少数）
- 一个创始人看着 $250K/年 的业务在 48 小时内崩塌

#### 为什么风险高
- 护城河极低：任何人都能套壳
- OpenAI/Anthropic 随时可以出同类产品
- 需要持续维护和客服
- 需要营销获客能力

#### 可行的 Micro-SaaS 方向
- Email Tone Converter (8,400 搜索/月)
- AI Resume Tailor
- AI Meeting Summarizer
- Niche-specific AI tools（如法律文书、医疗笔记）

#### Token 消耗
- 极高：每个用户的每次交互都消耗 tokens
- 需要精细的成本管理（否则亏钱）

---

### 8. AI 自动化工作流服务 (n8n/Make)

#### 模式
帮企业搭建 AI 自动化工作流，按月收费或一次收费。

#### 收入
- 单个项目 $500-$5,000
- 持续维护费 $100-$500/月
- 头部服务商月入 $10,000+

#### 问题
- **人类参与度极高**：需要理解客户需求、定制方案
- 不符合"低人类参与"的要求
- 但如果做出通用模板可以卖（automationworkflows.io）

---

## 针对你的情况的推荐方案

基于你的约束条件（有 Coding Plan、不想做需要大量手动操作的项目、关注卖素材），我的推荐排序：

### 方案 A：AI 素材/模板 + 图库 双轨并行（最推荐）

```
                    +---> Etsy/Gumroad (模板/Planner/Notion模板) --> 被动收入
AI 生成能力 --------+
                    +---> Adobe Stock/Freepik (图片/矢量/纹理) --> 被动收入
```

**为什么最推荐：**
1. Token 消耗量大（批量生成内容）
2. 人类参与极低（每月只需几小时检查和上传）
3. 收入可叠加（产品越多，被动收入越高）
4. 可以用编程能力做自动化工作流
5. 两条线互相补充，分散风险

**具体执行计划：**
- **第1周**：市场调研，确定 3-5 个 Niche
- **第2-3周**：搭建批量生成工作流（ComfyUI + LLM + Canva API）
- **第4周**：第一批产品上架（50-100个）
- **第2-3月**：每周新增 20-50 个产品，持续优化
- **第4-6月**：根据销售数据调整方向，重点投入高转化品类

**预计投入：**
- Token/API 成本：$20-50/月
- 平台费用：Etsy 每个listing $0.20，Gumroad 10% 抽成
- 时间：初期每周 5-10 小时，稳定后每月 5-10 小时

**预计收入：**
- 第 1-3 月：$0-$100/月（积累期）
- 第 4-6 月：$100-$500/月
- 第 7-12 月：$500-$2,500/月（如果有 500+ 产品）

---

### 方案 B：Niche 网站 + 联盟营销（次推荐）

**适合你如果：**
- 愿意投入 6-12 个月建设期
- 有 SEO 基础知识或愿意学习
- 能持续投入 token 生成高质量内容

**不适合你如果：**
- 想要快速见效
- 不想处理 Google 算法变化

---

### 方案 C：POD + 短视频（组合打法）

**适合你如果：**
- 想做国内市场（抖音/小红书）
- 愿意投入更多时间做内容运营

---

## 关键工具和资源

### 生成工具
| 工具 | 用途 | 成本 |
|------|------|------|
| ComfyUI | 图片批量生成（本地） | 免费（需显卡） |
| Midjourney | 高质量图片生成 | $10-60/月 |
| Claude/GPT API | 文案/市场调研/prompt生成 | 按 token 计费 |
| Canva | 模板设计 + 批量创建 | $13/月 Pro |
| banana-slides | AI 批量生成 PPT | 开源 |

### 销售平台
| 平台 | 类型 | 抽成 | 适合 |
|------|------|------|------|
| Etsy | 数字模板/素材 | $0.20/listing + 6.5% | 模板、planner |
| Gumroad | 数字产品 | 10% | 模板包、prompt包 |
| Adobe Stock | 图片/矢量 | 33-60% | AI 生成图片 |
| Freepik | 图片/矢量 | 按下载分成 | AI 图片 |
| Redbubble | POD | 按件计酬 | 设计图案 |
| PromptBase | Prompt | 20% | AI 提示词 |

### 自动化
| 工具 | 用途 |
|------|------|
| n8n | 工作流自动化（开源） |
| Make (Integromat) | 自动化连接各平台 |
| Etsy API | 自动上架/管理产品 |
| Adobe Stock API | 批量上传图片 |
| Merch Titans | POD 自动化上传 |

---

## 重要风险和注意事项

### 1. 平台政策风险
- Etsy 可能限制纯 AI 生成内容
- Adobe Stock 要求标注 AI 内容
- Google 打击纯 AI SEO 内容
- 抖音/小红书对 AI 内容限流

### 2. 市场饱和风险
- AI 素材/模板赛道竞争加剧
- Prompt 包市场已趋饱和
- POD 设计量大但头部效应明显

### 3. 质量风险
- AI 生成内容质量参差不齐
- 需要人工筛选和质量控制
- 低质量内容会损害店铺信誉

### 4. 收入预期
- 大多数"月入过万"的案例是卖课/卖工具的人在赚钱
- 实际被动收入需要 3-6 个月的积累期
- 真正的被动收入不存在——需要持续优化和调整

### 5. 法律风险
- AI 生成内容的版权归属仍不确定
- 有博主因搬运 AI 视频被判赔偿
- 需要注意不侵犯他人版权/商标

---

## 建议的实验路径

**不要一开始就 all-in，建议按以下顺序实验：**

### Phase 1 (第 1-2 周)：最小可行实验
1. 选 1 个 Niche（如 ADHD productivity planner）
2. 用 AI 生成 10 个产品
3. 上架 Etsy
4. 观察是否有自然流量和购买

### Phase 2 (第 3-4 周)：验证和扩展
1. 根据 Phase 1 数据，选择表现好的 Niche
2. 批量生成 50-100 个产品
3. 同时开始 Adobe Stock 上传图片
4. 搭建自动化工作流

### Phase 3 (第 2-3 月)：规模化
1. 每周新增 20-50 个产品
2. 扩展到 3-5 个 Niche
3. 优化 SEO 和标签
4. 开始看到收入趋势

### Phase 4 (第 4-6 月)：优化和聚焦
1. 砍掉表现差的产品线
2. 重点投入高转化品类
3. 考虑加入 POD 或联盟营销
4. 目标：$500+/月被动收入

---

## 参考来源

### 实际案例和经验分享
- [AI Digital Products That Earn $2,500/Month - Medium](https://medium.com/illumination/my-2-500-month-ai-etsy-gumroad-system-3017804395b2)
- [I Tried Selling AI Images on Adobe Stock - YouTube](https://www.youtube.com/watch?v=w8zkhu9bACc)
- [Honest 2025 Stock Photo Earnings - Reddit](https://www.reddit.com/r/stockphotography/comments/1pygn1n/honest_breakdown_of_my_2025_earnings_selling/)
- [I Used AI + Automation to Scale Redbubble (5,000+ Sales) - YouTube](https://www.youtube.com/watch?v=i5PoeZNkR3I)
- [How I ACTUALLY Make Money Selling AI Coloring Books - Medium](https://medium.com/@lazargrr1/how-i-actually-make-money-selling-ai-coloring-books-on-amazon-full-marketing-guide-445b66c60c38)
- [How I Automate My Side Hustle for 2025 - Medium](https://medium.com/@hazelparadise/how-i-automate-my-side-hustle-for-2025-b59ce8e5a7a3)
- [我在Etsy上卖AI提示词 - 汇智网](https://www.hubwiz.com/blog/i-sell-ai-prompts-on-etsy/)

### GitHub 开源工具
- [MakeMoneyWithAI - GitHub](https://github.com/garylab/MakeMoneyWithAI)
- [aimoneyhunter - GitHub](https://github.com/bleedline/aimoneyhunter)
- [MoneyPrinterTurbo - GitHub](https://github.com/harry0703/MoneyPrinterTurbo) (44K+ stars)
- [ComfyUI - GitHub](https://github.com/comfyanonymous/ComfyUI) (89.8K stars)
- [n8n - GitHub](https://github.com/n8n-io/n8n) (143.7K stars)

### 行业分析和趋势
- [The AI Side Hustle Explosion in 2025 - Asrify](https://asrify.com/blog/ai-side-hustle-explosion) (28% 增长)
- [Hidden Labor behind the Hype - ACM](https://dl.acm.org/doi/full/10.1145/3772318.3790702) (学术论文)
- [AI Wrapper SaaS Bubble - Medium](https://medium.com/@gohlingyong3/the-ai-wrapper-saas-bubble-is-over-i-watched-my-250k-yr-business-die-in-48-hours-170bb9ddea24)
- [20 Micro-SaaS Ideas for 2026 - StartuPage](https://startupa.ge/blog/micro-saas-ideas-2026) (90% 失败率)
- [Where to Sell AI Images in 2025 - Shotkit](https://shotkit.com/where-to-sell-ai-images/)
- [AI Art Passive Income: 5 Set-and-Forget Methods - ZSky AI](https://zsky.ai/blog/ai-art-passive-income)

### 中文资源
- [2025年「AI+副业赚钱」实操路线图 - 知乎](https://zhuanlan.zhihu.com/p/1960796731907241363)
- [小红书2026最赚钱的4种不露脸AI玩法 - YouTube](https://www.youtube.com/watch?v=0lU4CjizXaM)
- [AI数字产品：Notion模板+AI提示词包 - TraeAI](https://www.traeai.com/ai-money/244f0188-e837-4832-aa7d-ff325e742b09)
- [如何零成本打造AI博客变现 - 知乎](https://zhuanlan.zhihu.com/p/29854216118)
- [联盟营销自动化完整指南 - UseArticle](https://www.usearticle.com/zh/blog/affiliate-marketing-automation-how-to-earn-more-by-doing-less-in-2025/)

### Reddit/社区讨论
- [Anybody experience with AI-based side hustles? - Reddit](https://www.reddit.com/r/sidehustle/comments/1f47a2r/anybody_experience_with_aibased_side_hustles_that/)
- [Can You Really Make Money Selling Digital Products? - Reddit](https://www.reddit.com/r/passive_income/comments/1dubtdx/can_you_really_make_money_selling_digital/)
- [Do AI Wrapper Startups Have a Real Future? - Reddit](https://www.reddit.com/r/LocalLLaMA/comments/1lcksww/do_ai_wrapper_startups_have_a_real_future/)
- [Realistic AI Business Ideas - Reddit r/AI_Agents](https://www.reddit.com/r/AI_Agents/comments/1jmi9pf/what_are_some_realistic_aigenerative_ai_business/)

---

## 核心结论

**最符合你需求的方向：AI 素材/模板批量售卖**

理由：
1. Token 消耗量大（批量生成内容需要大量 LLM 和图像生成 API 调用）
2. 人类参与极低（初始搭建后，每月仅需几小时维护）
3. 可以利用编程能力（自动化工作流、API 集成、批量处理）
4. 收入可叠加（产品越多，被动收入越高）
5. 启动成本低（$20-50/月的 API 费用即可开始）
6. 风险可控（即使失败，损失也有限）

**关键成功心态：**
- 把它当成"token 换被动收入"的生意
- 前期重积累量（500+ 产品是基础）
- 用数据驱动决策，砍掉不赚钱的品类
- 不要追求完美，追求"足够好 + 量大"
- 持续测试新 Niche，找到你的印钞机
