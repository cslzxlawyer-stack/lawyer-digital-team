# 律师数字团队 Skill

适用于Codex的中国大陆律师工作流：按刑事、民事、行政诉讼、非诉分别处理，再按需要安排数字员工协作。

## 四条路线

| 类型 | 核心方法 |
|---|---|
| 刑事 | 角色×阶段×任务；指控/控告、证据、构成要件、程序及阶段策略 |
| 民事 | 请求权基础、否认与抗辩、举证责任、诉求金额、程序及执行 |
| 行政诉讼 | 被诉行为、可诉性、主体与期限、复议衔接、行政行为审查和救济 |
| 非诉 | 业务目标、交易结构、合同审改、尽调、法律顾问与专项合规落地 |

## 8个逻辑岗位

法律项目统筹、刑事主办、民事主办、行政诉讼主办、非诉主办、法律检索、案卷证据、质量复核。主会话统筹，按任务需要派工；不为小任务启动整队。

这是一套可安装的Skill，不是8个自动常驻的机器人。是否支持子智能体、命名角色和并发，以当前客户端为准；无子智能体时可顺序执行。安装不会修改模型、权限、MCP、全局AGENTS.md或并发设置。

## 安装到Codex

也可以让Codex的skill-installer安装本仓库中的skills/lawyer-digital-team目录。手动安装：

```bash
git clone https://github.com/cslzxlawyer-stack/lawyer-digital-team.git
mkdir -p ~/.codex/skills
cp -R lawyer-digital-team/skills/lawyer-digital-team ~/.codex/skills/
```

如果已有同名Skill，先比较并备份自定义内容。项目级安装可将目标换为项目的.agents/skills/。新聊天中能否自动发现以实际技能目录为准；也可显式调用。

## 使用

> 使用 $lawyer-digital-team。我方是民事买卖纠纷被告，请审查诉请、抗辩与举证责任，核对金额后修改答辩状，并安排质控。

还可以请求刑事阅卷/控告分析、行政程序与合法性审查、合同实际修改、尽调或顾问方案。尽量给出代表方、目标、阶段、地域、材料位置及紧急节点。
原件不覆盖；重要结论有来源；未核事实和法律保留待核；具体期限当次核验。用户已有且适用的刑事阅卷等方法可以继续使用，本包不复制用户私有技能。

## 目录

- [Skill入口](skills/lawyer-digital-team/SKILL.md)
- [分类方法与岗位](skills/lawyer-digital-team/references/)
- [虚构验证场景](tests/scenarios.md)
- [公开版来源与改编说明](skills/lawyer-digital-team/references/attribution.md)
- [来源版本与文件哈希](third_party/provenance.json)

## 许可

基于**卓建律师事务所蔡诗爽律师**主导的爽律Skill **v0.40公开共创版**CC BY-SA 4.0文本改编；新增行政路线与Codex岗位协作。固定提交和修改说明见[NOTICE](NOTICE.md)。

本项目文本采用[CC BY-SA 4.0](LICENSE)，不是上游官方版本，不使用其后续受限版本或品牌标识。没有附带案件材料或专业数据库；法律规则与案例仍需运行时核验，实质性对外成果由律师最终复核。

