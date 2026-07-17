# DIKWP-MANDATE²

**Multi-Actor Authorization and Negotiated Deployment with Accountability, Termination and Evolution**

中文：**DIKWP公共行动授权、可逆试点、独立结算与联邦复制协议系统**。

DIKWP-MANDATE²补充的是开源系统从“可运行代码”走向“可被公共机构、社区、大学、公益组织和多方共同采用”的授权与责任交易层。它不授予现实权力，也不替代法律、民主程序、专业伦理或受影响群体的同意。它只把公共行动必须回答的问题编译成可检查、可版本化、可撤回的协议对象。

## 为什么需要它

一个系统可以有完整的语义模型、预测、证据、标准、资金和代码，却仍然不具备开展公共行动的正当权限。缺失的问题包括：

- 谁受到影响，谁能代表他们；
- 哪些权利不能被多数票或模型分数取消；
- 提案者、出资方、运营方、审计方和结算方如何分权；
- 授权的范围、期限、预算、禁止项和退出方式是什么；
- 事故发生后谁先恢复权利、谁赔偿、谁调查；
- 一个本地试点的证据如何被别处复用，而不把本地价值判断强行复制过去。

## DIKWP不是阶段阶梯

本系统使用完整的25类DIKWP×DIKWP有向变换。M0—M6只是现实授权的程序状态，不是D/I/K/W/P的层级。每个状态内部都允许D、I、K、W、P相互生成、反驳、修订和回滚。

## 核心对象

- Public Challenge Dossier
- Actor and Conflict Registry
- Affected-Party Rights Card
- Observer-indexed DIKWP Semantic Mesh
- Option Set（必须包含“不行动”基线）
- Evidence and Counterfactual Contract
- Public Mandate Envelope
- Pilot Charter
- Funding and Procurement Ledger
- Incident, Appeal and Repair Ticket
- Independent Settlement Record
- Replication Passport
- Fork, Exit and Sunset Record

## 快速运行

```bash
PYTHONPATH=src python -m dikwp_mandate2.cli demo --root . --trials 15000 --seed 7172026
python -m unittest discover -s tests -v
```

打开 `outputs/dashboard.html` 查看离线仪表盘。

单独审计一个行动档案：

```bash
PYTHONPATH=src python -m dikwp_mandate2.cli evaluate examples/community_ai_transition_pilot.json
```

## 关键安全边界

- 不执行任何现实网络、支付、行政、福利、身份或执法动作。
- 不允许AI成为基本权利拒付的最终决策者。
- 不把合法性压缩为一个平均分；权利、代表、申诉、角色分离和可逆性为硬门。
- 不允许提案者单独结算自己的项目。
- 不允许一个地方的成功试点直接成为其他地方的授权。
- 所有示例分数与模拟均为合成或启发式结果。

## License

Apache-2.0. See `LICENSE`.
