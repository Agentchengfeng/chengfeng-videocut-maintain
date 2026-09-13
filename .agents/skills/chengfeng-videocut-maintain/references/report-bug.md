# Bug 反馈模式

先读[公共接入](shared/plugin-access.md)。默认交付可公开的 Issue 草稿；对外提交前展示精确仓库、标题、完整正文并取得用户确认。不是剪辑任务，不为草稿安装 Runtime、启动服务、上传素材或执行付费转录。

## 确认事实与归属

Bug 是实际行为偏离已有契约/承诺；从未支持的能力属于功能建议，不伪装成 Bug。只收集复现所需最小事实，缺证据标“未验证”；必要诊断按[排查模式](diagnose.md)只读处理。

| 问题组件 | 如何确定仓库 |
|---|---|
| 本产品 Runtime / Studio / CLI / API / 渲染 | 产品仓库 `Agentchengfeng/chengfeng-videocut`，提交前核实实际可访问且允许 Issue |
| 独立 Skill | 从该已安装包的固定发行来源/支持说明确认；计划地址或 local-candidate 元数据不等于已存在的仓库 |
| 旧 Plugin / Marketplace / 安装编排 | 从实际宿主提供者及该版支持说明确认，不把所有 Skill 问题固定投到旧 skills 仓库 |
| 第三方产品 | 用户指定产品的已确认支持仓库；不提交到本产品仓库 |

不从当前 cwd 或任意 Git remote 猜仓库。跨组件选最先违反契约的所属方并说明关联；身份不明先问用户。仓库不可见、没有 Issue 能力或无权限时保留草稿，不改报其他仓库。

## 脱敏草稿

直接用当前 Agent 生成，无需安装 Node、Git 或 gh。草稿写 Summary、Steps to reproduce、Expected、Actual、Environment、Minimal evidence、Acceptance criteria；环境只列必要 OS/版本，不公开完整 doctor。

删除或替换 API Key、Token、Cookie、Authorization、密码、环境变量值、用户名、卷名、绝对路径、localhost 查询参数、客户名、原视频名、真实 projectId、私人仓库内容。未经许可不附视频、音频、截图、完整日志或转录正文；通读检查语义敏感内容，不能只依赖自动脱敏。

展示 repo、建议标签 bug、title 与完整脱敏正文。仅确认问题存在不等于允许公开；内容或目标变动必须重新预览确认。

## 确认后提交与回读

1. 使用当前 Agent 已可调用且已获授权的 GitHub Issue 查询/创建能力，先查精确重复项。
2. 有相同组件、复现与结果的 Issue，返回其 URL；不重复创建，也不自动追加评论。
3. 无重复才提交已展示的原内容；标签以仓库实际支持为准，标签缺失不触发创建标签或换仓库。
4. 回读 repo/title/body/URL，只有明确目标 Issue URL 才说“已上报”。

没有可用工具、未认证、无权限或返回不明时明确“未提交/结果未知”；不安装新工具、不切换账号或擅自用浏览器宏补发。结果未知先查原请求，不自动重试。精确确认不跨任务重放。

用户未要求公开时，交付脱敏草稿就结束；修复经验仍归所属模块，不能将用户私有证据写入公开 Skill 源码。
