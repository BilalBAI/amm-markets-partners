# AMM Markets 技术团队总体架构

## 目标

AMM Markets 是一个面向 LP 的交易平台和池子定价机制。平台帮助 LP 获得更合理的定价、风险补偿和执行条件，但不代管资金、库存或完整投资组合。

网站平台与高频链上算法系统分开运行。网站不依赖高频系统的 Ethereum 节点，也不保存用户私钥；EOA、Safe 和 Safeheron 用户在自己的钱包中审核并签名交易。

## 五个核心角色

```text
AMM Protocol & Research Lead
        │  Hook、费率、价格边界、AMM 研究
        ▼
Web3 Platform Engineer ─────── Blockchain & Market Data Platform Engineer
网站、钱包、交易流程                 链上/CEX 数据、中央数据平台
        │                              │
        └───────────┬──────────────────┘
                    ▼
Infrastructure, Architecture & Security Engineer
总体架构、服务器、网络、部署、安全、灾备

Ecosystem, Growth & LP Partnerships Lead
对外推广、社区、LP 获取、机构合作和渠道建设
```

## 协作关系

- Protocol & Research Lead 定义协议逻辑、费率机制和 AMM 研究方向。
- Web3 Platform Engineer 将协议能力转化为网站、钱包和交易预览流程。
- Blockchain & Market Data Platform Engineer 提供可追溯的链上与链下数据。
- Infrastructure, Architecture & Security Engineer 保证系统隔离、安全、可部署和可恢复。
- Ecosystem, Growth & LP Partnerships Lead 连接 LP、机构、钱包、托管方和生态伙伴。

所有对外指标（例如 fee income、fee yield、APR）都应先经过数据和协议负责人确认口径。增长团队不承诺投资回报，也不发布未经验证的数字。

## 组织原则

- 不以学历、名校、公司背景或固定工作年限作为硬门槛；以真实能力、作品和判断力为主。
- 协议安全、数据正确性、系统安全和客户资金边界必须有人明确负责。
- 智能合约审计、渗透测试和必要的法律/合规评估可由外部专家独立完成。
- 创始人/产品负责人负责产品方向、关键机构关系和最终业务取舍。
