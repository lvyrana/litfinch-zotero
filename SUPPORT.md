# Support

## 新版试用常见问题

本节对应当前正式版 0.10.0。已在 macOS / Zotero 10.0.6 使用当前内容构建验证主要阅读入口；完整的个人 AI 生成、卡片/汇报、导出、恢复和重启保留仍需按发布记录逐项验收。旧 0.3.0 只有网页导入入口；安装与连接见 [README](README.md#安装与连接)。Windows 与 Linux 尚未原生验收，反馈请注明平台。

| 问题 | 处理方式 |
|---|---|
| 没有「研雀」入口 | 先看插件版本，再确认已打开 PDF；旧公开包仍显示 PaperMind，不能按新版阅读台寻找按钮 |
| 显示登录尚未启用 | 向维护者反馈版本和提示；这是配套服务配置待完成，不需要提交 Zotero 密码或自行创建文库 Key |
| Zotero 已同步登录，研雀仍要求登录 | 两者会话分别管理；按阅读台的登录入口完成身份确认 |
| 登录后仍无 AI 权限 | 邀请与额度独立生效，记录具体提示，由维护者核对 |
| 当前页没有可读取文字 | 改试摘要或有文字层的页面；当前原生阅读台不提供扫描页 OCR |
| 插件卡片未出现在网页 | 当前未实现自动同步；返回原服务、原账号和原论文查找，不删除本地阅读目录 |
| 回答能显示但解释不准确 | 单列为内容问题，记录页码及错误类型，区分数字错误、关系解释和结论过强 |

一条消息即可反馈：入口与版本、最后一个操作、期望结果、实际提示、系统及 Zotero 版本、大致时间。截图裁剪到必要区域；不要为复现问题反复切换账号或公开完整文献。

## 问题与需求 / Bugs and feature requests

可复现的插件问题和功能建议请提交到 [GitHub Issues](https://github.com/lvyrana/papermind-zotero/issues/new/choose)。Bug 表单会要求：

- 研雀插件版本；
- Zotero 版本和操作系统；
- 问题发生在哪个阅读操作；
- 简短复现步骤和期望结果；如界面显示报错，再附上不含敏感信息的准确文字。

功能建议表单不要求先判断版本或复现 Bug，只需说明实际阅读问题、建议怎样改，以及现在是否有绕过方法。

维护规则：新 Issue 目标在 2 个工作日内确认收到并完成第一次分流；需要更多材料时写清缺什么，确认是问题时关联修复版本或 PR，需要作者取舍时标明待决定事项。每周维护还会清点本周新增、仍未关闭和超过 7 天没有维护者响应的 Issue，防止漏看。该时限是维护目标，不代表问题会在 2 个工作日内修复。

Please use [GitHub Issues](https://github.com/lvyrana/papermind-zotero/issues/new/choose) for reproducible bugs and feature requests. The maintainer aims to acknowledge and triage new issues within two working days. The weekly review also checks new, open and unanswered-for-more-than-seven-days issues as a backstop.

不要附加受版权保护的 PDF，也不要提交个人链接、设备 ID、API 密钥、患者信息或未公开敏感资料。涉及安全漏洞时不要创建公开 Issue，改用下方私密入口。

## Data deletion

Do not post a device ID in GitHub Issues. Request server-data deletion through「设置 → 用户反馈」while using the original identity or signed-in account. Describe the requested scope without pasting credentials or personal links. A request is not confirmation that deletion has completed.

Server records, account ownership/sessions, local `papermind-reading/` files, exported Zotero notes and backup copies require separate handling. Logging out or uninstalling the plugin does not delete all of them. The older anonymous-UUID deletion script does not cover the account database or local plugin files; it must not be reported as complete account deletion. Follow [PRIVACY.md](PRIVACY.md#5-保存与删除) and obtain a scope-specific completion report from the service maintainer.

## Security reports

安全漏洞必须通过仓库的 [私密安全报告](https://github.com/lvyrana/papermind-zotero/security/advisories/new) 提交，流程见 [SECURITY.md](SECURITY.md)。周检只核对私密入口是否仍可用，不复制或汇总漏洞详情。
