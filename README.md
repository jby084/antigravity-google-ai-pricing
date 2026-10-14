# Antigravity Google AI Pro 订阅指南：$19.99 的额度怎么算？免费版和 Plus 够不够用？Ultra 两档值不值？（附优惠码立减入口）

在 Google Antigravity 里跑 agent，额度从来不按 Antigravity 单独卖，而是打包在 Google AI 订阅里。所以搜「Antigravity Google AI Pro」的人，真正想弄清楚的一般是三件事：这 $19.99 一个月到底买到什么、免费版能不能凑合用、以及要不要直接上 $100 或 $200 的 Ultra。

先把结论放在前面：**对大多数独立开发者，Google AI Pro 是合理的第一个付费档**。免费版适合评估，Plus 更像存储捆绑包，Ultra 两档只在你的额度反复被打断时才有意义。下面按实际会遇到的顺序讲清楚。

## 先弄懂：Antigravity 的订阅结构变过一次

2026 年 5 月的 Google I/O 上，Antigravity 更新到 2.0，产品拆成一个统一的 harness 加两个入口：重新设计的桌面端，和一个独立的 CLI。顺带一提，桌面端刚上线时曾把终端访问和 Git 工具砍掉，三个月后在 2.10.0 版本才恢复，对这条产品线的迭代节奏保留一点预期管理不算多余。

订阅结构也跟着动了：原来唯一的高端选择，每月 $250 的 Google AI Ultra，被拆成两档，新增 $100/月的中档 Ultra，顶配降到 $200/月。

额度机制有个重要变化。以前 Gemini Flash 和 Gemini Pro 各有独立的速率限制，现在合并成一个共享池，按 API 定价折算扣减。举个例子：如果 Flash 在 API 定价上比 Pro 便宜 8 倍，同样一份额度，你可以全花在 Pro 上，也可以换成 8 倍量的 Flash，或者两者任意组合。比原来“官方替你固定好比例”灵活不少。

两个例外要知道：

- 非 Gemini 模型（Claude、GPT-OSS 等）因为容量紧张，仍然单独走一个固定的速率限制池。
- AI credits 从 5 月起不再包含在 Google AI 基础订阅里，只作为额度用完之后的超额付费机制。

另外，Google 没有公布任何档位的固定 token 数或任务数，并明确保留根据算力情况调整限额的权利。所有“5 倍”“20 倍”都是相对于 Pro 档的倍数，绝对数值会浮动。

## 全部套餐与价格一览

| 套餐 | 月费（USD） | Antigravity 额度 | 其他权益 | 开通入口 |
| --- | --- | --- | --- | --- |
| Individual（个人版） | $0 | 无限 Tab 补全、无限 Command 请求，基础每周 agent 额度 | — | [ 免费开始使用](https://bewild.ai/?code=ACCPAY) |
| Google AI Plus | $4.99 | agent 请求受限，不可购买 AI credits | 400 GB 存储 | [ 查看 Plus 档](https://bewild.ai/?code=ACCPAY) |
| Google AI Pro | $19.99 | 每 5 小时刷新一次，直到触及每周上限；可购买 AI credits | 5 TB 存储、每月 $10 Google Cloud credits | [ 开通 Google AI Pro](https://bewild.ai/?code=ACCPAY) |
| Google AI Ultra 5x | $99.99 | 5 倍 Pro 额度，优先访问 | 20 TB 存储、每月 $40 Cloud credits | [ 开通 Ultra 5x](https://bewild.ai/?code=ACCPAY) |
| Google AI Ultra 20x | $199.99 | 20 倍 Pro 额度，每 5 小时刷新 | 30 TB 存储、每月 $100 Cloud credits | [ 开通 Ultra 20x](https://bewild.ai/?code=ACCPAY) |
| Organization（组织版） | 按用量计费 | 走 Google Cloud 条款，接入 Gemini Enterprise Agent Platform | Google Cloud 项目集成 | [ 了解组织版接入](https://bewild.ai/?code=ACCPAY) |

看这张表时有两点容易踩坑。

第一，网上不少文章还在写 $249.99 的 Ultra，那是改版前的旧价，看到这个数字的页面内容至少落后了三个月。

第二，Pro 档捆绑的每月 $10 Cloud credits 属于开发者计划权益，不能拿来抵 Antigravity 的超额费用，是两笔账。

### Individual（$0）：拿来测试，别拿来干活

免费档是正式可用版本，不是限时试用。Tab 补全（行内自动补全）和 Command 请求（非 agent 的单次指令）不限量，agent 调用则有基础额度，按周刷新。

定价卡上列的模型相当多——Gemini 3.5 Flash、Gemini 3.1 Pro、Gemini 3 Flash、Claude Sonnet 和 Opus 4.6、gpt-oss-120b——但官方文档同时把第三方模型访问列为 Ultra 权益，低档位实际能选到哪些模型，以你登录后模型选择器里显示的为准。

免费档真正的墙是 agent 额度。连续跑几个 agent 任务，一天的量可能就见底。它适合的场景：以补全和单次指令为主、在旁项目上评估 agent 工作流、偶尔跑个大任务且不着急。如果你的日常交付已经依赖 agent，每周额度会把忙碌的周二变成等额度的好几天。

### Google AI Plus（$4.99）：买的是捆绑包，不是稳定的开发日

Plus 档在官方对比页里，Antigravity agent 请求被标注为“受限”（limited），而且这个档位不能购买 AI credits，额度用完没有任何补救通道。它包含 400 GB 存储和一批消费级 AI 权益。

判断很简单：如果这 400 GB 和那批权益你本来就需要，买 Plus 顺带用 Antigravity 没问题；但如果你图的是稳定的 agent 开发体验，这一档给不了。

### Google AI Pro（$19.99）：默认答案

Pro 是第一个“能干活”的档位。额度节奏从免费版的按周刷新，变成每 5 小时恢复一次、直到触及每周上限。上午把 agent 额度跑空，下午晚些时候能回一部分血；但每周上限才是真正的天花板，触及之后 5 小时刷新也帮不了你。它还允许在基础额度耗尽后购买 AI credits，这是和 Plus 的关键区别之一。

消耗方面要有个预期：Antigravity 2.0 的并行子代理（subagents）确实好用，但额度也是并行烧的。CLI 场景下，一个自然语言目标可能在不提示的情况下触发十多次模型调用。有 Pro 档用户反馈，开并行子代理跑重活时，大约两千行生成代码就会把每周额度用掉。稳妥的做法是把并行子代理控制在三到五个，重活之前先用 /usage 看一眼余量，agent 自己看不到剩余额度。

每天用 agent 处理生产代码的独立开发者，这一档基本就是对的选择。

### Ultra 两档：为并行编排和长任务准备的

**Ultra 5x（$99.99）**提供 5 倍 Pro 额度，价格也差不多是 Pro 的 5 倍，折算下来每个“Pro 等价额度单位”的成本还是 $20 左右。它买的是容量，不是折扣。适合已经习惯这套工作流、但每周不止一次撞到 Pro 天花板的人。

**Ultra 20x（$199.99）**提供 20 倍额度，价格是 Pro 的 10 倍，单位成本降到约 $10，这是全部档位里唯一一个单位成本下降的档。从 5x 升到 20x 多花 $100/月，多拿 15 个等价单位，增量成本约 $6.67/单位，前提是这些量你真的用得掉。

还有一个务实的玩法：这些订阅都按月计费，可以“冲刺期上 Ultra，平时降回 Pro”。额度这种东西，用不掉就是纯成本。

## 额度用完了怎么办：AI credits 的正确用法

Pro 和 Ultra 在基础额度耗尽后，可以购买 AI credits 续命。设置里有一个 AI Credit Overages 开关，两档选择：

- **Never**：模型撞到基础额度就停下，等刷新。
- **Always**：自动开始消耗 credits 余额，刷新后切回基础额度。

credits 有 2,500、5,000、20,000 几种包，消耗速度取决于功能和模型。要特别小心自动补购：它可以一天内最多触发 5 次购买，一个模糊的额度表就这样变成一条开放的账单。另外，日本区目前不能购买 Antigravity credits。

建议默认用 Never。等你设好现金预算、观察过所用模型真实的消耗速度之后，再考虑打开 Always。

在上付费档之前，也有几件事能实打实省额度。日常的代码生成和重构交给默认的 Gemini 3.5 Flash 就够，重推理任务再切大模型。prompt 写具体一点，“修一下这个函数”产生的废案比“用三元表达式重写这个函数：输入大于 0 返回 positive，等于 0 返回 zero，否则返回 negative”贵得多，被丢弃的输出是最贵的消耗。分类、格式化、短摘要这类轻活可以丢给本地跑的模型（比如 Gemma 4 配 Ollama），一点云端额度都不占。

## Gemini CLI 停用之后：CLI 用户要换工具了

如果你以前用 Gemini CLI，它在 6 月 18 日已经对所有个人档位停用，替代品是 Antigravity CLI（命令是 agy）。迁移本身不难：安装脚本一条命令，环境变量从 GEMINI_API_KEY 换成 AV_API_KEY，~/.gemini/ 目录下的 GEMINI.md 全局指令会自动继承。

但额度口径变了。旧的 Gemini CLI 按天算，每天 1,000 次请求；Antigravity CLI 按周算一个叫 "Work Done" 的计算量，统计口径包含输入输出 token、隐藏思考 token 和工具调用开销，具体数字不公开。如果你的 CLI 用量习惯是照旧口径校准的，把迁移后的第一周当作测量周，别急着定档位。

## 怎么订阅：官方渠道和优惠码

订阅入口是 Google AI 计划本身：在官方订阅页选档，Antigravity 的访问权限随之解锁。Pro 支持月付和年付，但公开页面只展示 $19.99/月，年付的折后总价要登录到结账页才能看到；考虑到年付通常不退，建议先按月跑一两个月、证明这套工作流对你有效，再考虑长约。

如果官方渠道的支付方式对你不方便，也可以走第三方开通平台，比如 Bewild，下单时填优惠码 **ACCPAY** 可以立减 1 美元：[👉 前往 Bewild，用 ACCPAY 开通](https://bewild.ai/?code=ACCPAY)。1 美元不多，不值得为它改变决策，但本来就要开通的话，顺手填上就是了。

## 常见问题

**Antigravity 本身免费吗？**
是。Individual 档永久免费、正式可用，agent 调用带每周限额，Tab 补全和 Command 不限量。

**订 Google AI Pro 就能用 Antigravity 了吗？**
能。Antigravity 不单独计费，访问权限打包在 Google AI 订阅里，Pro 及以上档位都包含。

**额度到底怎么算的？**
Google 用一个叫 "Work Done" 的计算口径统计，包含输入、输出、隐藏思考 token 和工具调用开销，具体数值和上限都不公开，消耗随任务复杂度、模型选择和 agent 工作量浮动。这也是为什么“多少钱一个合并的 pull request”这类计算做不出来。

**怎么判断自己该上哪一档？**
别看平均用量，看被打断的频率。花两周记录两件事：额度打断你几次、当时并行跑了几个 agent。一周被打断 0–1 次，留在 Pro；只在并行重活的日子被打断、且这种日子经常有，上 Ultra 5x；几乎天天被打断，直接 Ultra 5x 起步，持续饱和再考虑 20x。账也好算：按每次打断浪费半小时估算，时薪 × 半小时 × 每月次数，超过 $80（正是 Pro 到 Ultra 5x 的差价）就值得换档。

**公司团队怎么买？**
组织版不走个人订阅，而是通过 Google Cloud 接入 Gemini Enterprise Agent Platform，按用量计费，部分 Gemini Enterprise 订阅包含访问权限。让采购去谈云协议，比把一堆个人订阅凑成团队方案靠谱。
