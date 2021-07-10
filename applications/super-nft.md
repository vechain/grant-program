# **VeChain General Grant**

# **Application Template**

## **Project Overview** 

- Project: 基于权益绑定与个人 IP 的 NFT 平台 SuperNFT

—— 人人都可以建立自己的 NFT IP 中心

- Team Name: SUIBE-BlockChain 
- Payment Address: 0x769699506f972A992fc8950C766F0C7256Df601f

⚠️ The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.

### Overview

Please provide the following:

- A brief description of the project.

目前，在我担任 CTO 的区块链教育公司（柏链教育）在区块链技术培训方面已经具备一定业务量。在现有业务上挖掘更多的区块链玩法，以及挖掘新的业务点是公司今年的重要战略。

在此基础上，我们设计了一种基于权益绑定与个人 IP 的 NFT 平台  SuperNFT，将NFT 作为权益证明，这个平台的玩法用如下的图来进行说明：

- **核心玩法1——权益绑定**

![](https://tva1.sinaimg.cn/large/008i3skNgy1grmjwp3an6j30xx0u0afu.jpg)

在上层业务设计上，让玩法突破现有的「 NFT - 艺术品模式」，将 NFT 和权益进行绑定。

NFT 持有者和权益发放方签订合同（例：NFT持有者每年给权益发放方社区拉新1000人，权益发放方则奖励NFT持有者10000元），通过多重权益的方式，确保 NFT 的独一无二性与价值性。

- **核心玩法2——NFT分裂与组合**

<img src="https://tva1.sinaimg.cn/large/008i3skNgy1grmjx3oro2j30rn2atjxq.jpg" style="zoom:50%;" />

核心玩法2是核心玩法1的升级，NFT持有人可以将其NFT分裂，发放给任意用户群体（如粉丝群）。NFT的分裂也意味着权益的分裂，原有权益将通过NFT树，发放给最终的NFT持有人。

**（核心玩法2的逻辑支撑是「粉丝经济/粉丝商业」）**

此外，分裂的NFT也能再次重组！

- **分布式特性——支持独立部署**

如 SLOGAN 中所阐述的那样：人人都可以建立自己的 NFT IP 中心

本项目完全开源，支持一键部署，在项目设计理念中贯彻分布式思想。

- An indication of why your team is interested in creating this project within the VeChain Ecosystem.

**在更长远的规划中，NFT 将和 实体实现 1：1挂钩，因此需要选择和物联网技术（如 NFC）技术契合度最好的公链。**

- If relevant, an indication of how you will integrate tools and features (e.g., Sync2/Connex, fee delegation protocols, MTT, etc) to enhance your project. 

事实上，在 Vechain 的发展战略中，也在强调和实体挂钩的 [eNFT](https://medium.com/vechain-foundation/the-future-of-vechainthor-enterprise-nft-enft-ecosystem-137589e53974)，所以我们项目的规划和 Vechain 的发展战略是契合的。

此外，如果有生态中的企业推出NFT Wallet（浏览器/App）（e.g. [sync2](https://github.com/vechain/sync2))，我们也会全力配合，让 NFT-PLus 和 NFT Wallet 兼容。

### Project Details

We expect the teams to already have a solid idea about the project's expected final state. Therefore, we ask the teams to submit (where relevant):

- Mockups/designs of any UI components
- API specifications of the core functionality
- An overview of the technology stack to be used
- Documentation of core components, protocols, architecture, etc. to be deployed
- PoC/MVP or other relevant prior work or research on the topic

- **NFT+ 设计**

NFT+ 是 NFT 的升级，这个升级借助于 Evidencer 存证合约，无需对原有的 NFT 进行改造，从而确保与已有的 NFT 业务/系统兼容。

NFT+ 包含如下元素：

**属性元素：** ERC721

- NFT Token ID 代币唯一编号（Chain ID + Contract Addr + Token ID => 唯一性）
- NFT URI 资源地址

**注：** 上述内容用 ERC 721 可实现。

- NFT 专属名称
- NFT  详细描述（可用以描述权益）
- NFT 相关URI
- NFT 生效日期
- NFT 失效日期
- 父 NFT 唯一编号
- 附加额外属性：通过 JSON 形式存储额外属性，使 NFT+ 即保证兼容性也保证可扩展性。

**注：** 上述内容结合 Evidencer 存证合约实现。

- **太上 NFT 炼金炉**

**进展：**

**开发中——** https://github.com/WeLightProject/Tai-Shang

太上 NFT 炼金炉是 Super-NFT 的重要组成部分，但其同时也是一个独立提供服务的基础设施。

太上在不改变原有 NFT 合约的基础上，通过附加「存证合约」，赋予 NFT 组合、拆解、生命周期、权益绑定等能力，锻造 NFT +，创造无限创新玩法与想象空间。

![太上 NFT 炼金炉简述 (6)](https://tva1.sinaimg.cn/large/008i3skNgy1grmjzznaeyj31iy0u0qa2.jpg)

**太上 NFT 炼金炉玩法示意图**

- **NFT-Parser**

**进展：**

**开发中——** https://github.com/WeLightProject/NFT-Parser-0x01

NFT Parser，中文 NFT 解析器，将 NFT+ 解析并展示。

将 NFT Parser 与其它组件独立，实现 NFT 的解析方式和 NFT 本身解耦，同一个 NFT 通过不同的 NFT Parser 呈现出不同的表现状态，从而赋予 NFT 流动性与价值想象空间。

​                 ![2s45O5DLmCfMgkI30wQNMQ?w=1706&h=1080](https://tva1.sinaimg.cn/large/008i3skNgy1grmjyppcq4j31be0u0tfs.jpg)

**NFT Parser 玩法示意图**

- **主平台**

**进展：设计中**

![pxLZ-w0CRANKLD_uxWgkgw?w=3189&h=2424](https://tva1.sinaimg.cn/large/008i3skNgy1grmjz3u9gxj313h0u0dta.jpg)

**主平台架构图**

「区块链层」与「区块链生态组件」为主平台提供区块链基础能力支撑，设计支持 VeChain 唯链、FISCO BCOS 联盟链、Ethereum 以太坊、基于Substrate的框架的区块链（如波卡）等。

「链上-本地同步层」负责链上信息和本地数据库的同步，已实现链上信息规范化存储，同时方便本地进行调用。

「功能层」为具体的NFT功能，包括链上DID数字身份模块、NFT管理模块、权益模块、NFT交易模块。

主平台与外部程序（如 NFT Parser 等）通过「API接口层」和下层相连。

用户层包括管理机构（个人/企业IP运营团队）、普通用户（粉丝群）、权益机构（可选）三种角色。

### Ecosystem Fit

Are there any other projects similar to yours? If so, how is your project different?

1. **社区将 NFT 用于权益证明的实践案例**

目前有区块链社区，如ZenLink，使用NFT作为社区成员的权益证明：

> Zenlink 将赋予该限量版社区 NFT 社区属性及经济属性 ，持有者将能够获得一定的权益。
>
> - 经济属性：NFT 的发行目的并不是炒作，但由于其总量有限、设计精美，并与 Zenlink 未来的发展具有强绑定关系，因此该 NFT 将具备如下经济属性及权益。
> - NFT 增值属性 ：Zenlink 社区 NFT 将邀请知名艺术家进行定制设计且全球限量发行，持有该 NFT 卡意味着拥有了一张限量版的 NFT 艺术品，随着项目的发展将具备更大升值空间。
> - 治理权益 ：Zenlink 计划设立 DAO 组织，DAO 将单独支配一个资金池，Zenlink 限量版社区 NFT 持有者将有更高优先级的加入权限；DAO 成员将有权发起 DAO 资金池支配提案。
> - ZLK 空投权益 ：参与 Zenlink 发起的相关活动，比如，参与 Zenlink DEX Beta 版本的测试，将有机会赢取 NFT，NFT 持有人将拥有获得 ZLK 空投的权益，具体细节即将公布，敬请期待。
> - 其他权益 ：Zenlink 限量版社区 NFT 持有者还将拥有获得 Zenlink 官方周边产品的权益。

2. **个人社交代币实践案例**

https://www.matataki.io/

**总结：**

社区使用 NFT 治理是一种很好的思路，我们设计的平台再往前走出一步，一方面在设计上将 NFT 发行机构和权益发放的社区组织进行解耦，让平台更具备想象空间与可扩展性；另一方面支持 NFT 发行机构/个人、权益发放社区/个人入驻，实现去中心化。

传统社交代币在个人 IP 治理方向上，往前迈出了一大步，但是相对于同质化代币，我们团队认为，非同质化代币更适合与个人 IP 相结合（粉丝更希望拿到独一无二的偶像签名照而不是希望拿到没有区别的偶像代币）。

## **Team** 

### Team members

- 李骜华
- 刘峰、汤会枫、黄杰、王宁波、肖越、利牧

### Team Website

- https://suibe.net/
- https://weimang.cyberemd.com
- http://lab.cyberemd.com

### Team's experience

**荣誉奖项**

| 2020首届 BSN 开发者大赛 \| 优秀奖      | 2020.03 |
| -------------------------------------- | ------- |
| 2020区块链技术与教育高峰论坛 \| 三等奖 | 2020.01 |
| 2020第二届 BSN 开发者大赛 \| 金奖      | 2020.08 |
| 2020第四届中国区块链开发大赛 \| 二等奖 | 2020.08 |
| 2020微众金融科技大赛 \| 十强           | 2020.11 |

**作品列表**

多链聚合门户（Elixir）：

https://github.com/WeLightProject/WeLight-Portal

FISCO BCOS 区块链开发工具箱（Python）：

https://github.com/SUIBE-Blockchain/FISCO-BCOS-Toolbox

基于 Elixir/Java 的供应链金融案例（Elixir&Java）：

https://github.com/BailianBlockchain/Bailian_Supply_Chain

https://github.com/WeLightProject/supply-chain-demo

### Team Code Repos

- https://github.com/SUIBE-Blockchain/Super-NFT

**基于权益绑定与个人 IP 的 NFT 平台 SuperNFT**

- https://github.com/WeLightProject/Tai-Shang

**子项目同时也是独立项目：支持多链的 NFT 基础设施 —— TaiShang 太上 NFT 炼金炉**

### Team LinkedIn Profiles

- [https://www.linkedin.com/in/%E9%AA%9C%E5%8D%8E-%E6%9D%8E-50bb94136/](https://www.linkedin.com/in/骜华-李-50bb94136/)
- https://www.linkedin.com/in/lekkoliu/

## **Development Roadmap** 

This section should break out the development roadmap into a number of milestones. Since the milestones will appear in the grant contract, it helps to describe the functionality we should expect, plus how we can check that such functionality exists in the product. Whenever milestones are delivered, we refer to the contract to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. For each milestone:

- Please indicate the milestone duration, workload in terms of full-time equivalent (FTE) and cost. 
- Please be sure to include a specification of the software. The level of details must be high enough so that we are able to verify that the software meets the specification.
- Please note that we require documentation (e.g. tutorials, API specifications, architecture details) in each milestone. This ensures that the code can be widely used by the community.
- Please provide a test suite, comprising unit and integration tests, along with a guide on how to run these.
- Please commit to providing dockerfiles for the delivery of your project.

### **Example Roadmap for a** DApp Application

#### **Overview**



|                            | **Milestone 1** | **Milestone 2** | **Milestone 3** |
| -------------------------- | --------------- | --------------- | --------- |
| Estimated Duration         | 60 d            | 60 d            | 60 d      |
| Full-time equivalent (FTE) | 2(4 Part-Time Worker)| 2(4 Part-Time Worker)  | 4(8 Part Time Worker) |
| Cost (up to $ 30,000)      | $ 10,000        | $ 10,000        | $ 10,000  |



#### **Milestone 1 — NFT 分解组合引擎的开发及完善**

##### 1. 开发计划

- [x] **抽象设计**

简述：设计NFT+中的额外属性。

见 [NFT+ 设计文档](NFT+ 设计文档.md)。

- [x] **区块链端**

**技术栈：** Solidity/WASM

**简述：** 标准erc721合约 + 存证合约

- [x] `evidence`

基于工厂设计模式，作为erc721+的存证合约。

- [x] `erc721`

标准erc721合约

---

- [ ] **炼金炉端**

**技术栈：** Elixir-Phoniex

**简述：** NFT 熔炼核心，支持界面/接口两种熔炼方式。

- [x] `Syncer`

支持多链的链上-本地同步器。

- [x] `Combiner`

  混合器，负责 NFT 的输入、处理与输出。

- [ ] `Caller`

  将 NFT 的输出结果通知 NFT 发行方。

- [ ] `可视化界面`

  基于 Phoniex 的炼金炉可视化界面，支持可视化「熔炼」NFT。

- [ ] `接口中心`

  通过接口进行 NFT 的「熔炼」。

---

- [ ] **解析端**

**技术栈：** 多语言。

**简述：** 适配该应用/该链，将 NFT + 实体化，如解析为「屠龙宝刀」、「游戏称号」等等等等。

- [ ] `Interactor`

和链进行交互。

- [ ] `Parser`

  - NFT Parser 0x01：基本款—— https://github.com/WeLightProject/NFT-Parser-0x01
  - NFT Parser 0x02：与二次创作玩法相结合的NFT关系树
  - ……

##### 2. 运营计划

- 在个人（李大狗）/企业（柏链）的多个公众号中及时宣发项目进展
- 「一点知道」学习 App 率先使用
- 通过 Vechain 的渠道进行项目宣发

##### 3. 开发计划

- **需要完成的目标：**

- 应用的开发（已完成）：

浏览地址：https://taishang.leeduckgo.com

- Vechain 测试网的适配：

完成接入。

- Vechain 上线：

基础设施独立上线。

#### **Milestone 2  —  平台主体打造**

##### 1. 研发计划

- 平台主体完成Vechain适配
- 平台前端实现
- 平台后端实现
- 文档完善
- 线上体验系统部署
- 钱包接入

##### 2. 运营计划

- 在个人（李大狗）/企业（柏链）的多个公众号中及时宣发项目进展
- 「一点知道」学习 App 率先使用
- 通过 Vechain 的渠道进行项目宣发
- 作为独立项目争取融资

##### 3. 需要完成的目标

- Vechain 测试网的适配：

  - 完成接入。
  - 流程闭环跑通。

- 项目主网上线

#### Milestone 3  —  链上-实体连接

##### 1. 研发计划

- IoT/NFC 相关部分的支持。
- 链上-实体绑定的实现。
- 平台主体升级
- NFT 分解组合引擎升级
- NFT Parser 升级

- **需要完成的目标：**


##### 2. 运营计划

- 在个人（李大狗）/企业（柏链）的多个公众号中及时宣发项目进展
- 「一点知道」学习 App 率先使用
- 通过 Vechain 的渠道进行项目宣发
- 商业逻辑完全跑通

##### 3. 需要完成的目标

- Vechain 测试网的适配：

  - 完成接入。
  - 流程闭环跑通（现实实体——NFT打通）。

- 生产环境项目升级

#### **Community engagement**

As part of the Program, we require that you produce and publish at least one article/tutorial (e.g., on Medium). It should explain your work done as part of the grant.

## **Future Plans**

Please include the team's long-term plans and intentions.

**愿景1：** 助力所有 NFT，让其具备无限商业想象空间与无限玩法。

**愿景2：** 人人都可以建立自己的 NFT IP 中心。

**目标：**

1）服务企业已有业务需求，包括教育业务与集团内部治理业务；

2）成功跑通 NFT + 个人 IP 商业模式。

## **Additional Information** 

無。
