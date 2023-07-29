![SHINN - Interchain Credential Network (ICCN) _share (1)](https://github.com/yuk6ra/shinn/assets/59524938/18dab4dd-76cb-4bca-9399-10f778b72c10)

# SHINN
## Overview
### Vision
次世代の信用インフラストラクチャーによって新しい社会システムを実装する

### Mission
世の中のあらゆるクレデンシャル・データのコンポーザビリティ（Composability）とスケーラビリティ（Scalability）をなめらかにする

### Problem
既存のオンチェーン・クレデンシャル・プラットフォームは、マルチチェーンが主流であるため相互運用性に欠けている状況にあり、新興チェーンやその上に展開するDAppsのプロジェクトにとって将来的に柔軟性がないサービス設計になっている。

### Solution
クレデンシャルデータ特化L1パブリック・ブロックチェーン 『SHINN Network』

### How to develop
- Cosmos SDKを活用したApplication-Specific Blockchainの運用
- Interchain NFT (ICS721), Interchain Account (ICS27)によってチェーン間移動可能なクレデンシャル・データの発行プロトコルの運用

### Business Models
- クレデンシャル・データのブロックチェーン・エキスプローラ『ICCN Scan』のAPI提供（課金）
- クレデンシャル・データ管理ツール『SHINN』の課金 （SaaS）
- クレデンシャル・データのマーケットプレイス（Interchain NFT Marketplace）の手数料（2.5%）
- 各プロジェクト同士のコラボレーション支援手数料

## Background
企業にブロックチェーン・アプリケーションをDBの機能の一部として開発依頼されたときに、チェーン選定が必ず議論になる。その結果、現状どこかのチェーンに依存する提案になる。まずエコシステムが既に発展しているチェーン上にDAppsとして展開し、ユーザを集めることが１つの選択肢になる。しかし、発展したときにDAppsからチェーンに展開(dydx方式)、または別チェーンにDappsを展開する際は、既存のオンチェーン・クレデンシャル・データは扱いづらい。データの取得手段と真贋性はAPIなどに依存している。オンチェーンのデータ（NFT）も単一のブロックチェーンに縛られてしまう現状がある。現在、オンチェーンのクレデンシャル・データはコンポーザビリティがあるとは言えない。

![image](https://github.com/yuk6ra/shinn/assets/59524938/6b642049-816e-4f85-998c-1536302500c4)


## Problems
特定のブロックチェーン上のDApps間でコンポーザビリティは発揮されるが、クレデンシャル・データは単一のチェーンに依存してしまうため、将来を見据えた拡張性がない。そして、ユーザのアイデンティティを示すデータはチェーン間で自由に移動することができない。つまり、現在のオンチェーン・クレデンシャル・データのプラットフォームは『スケーラビリティがない』という課題がある。

![クレデンシャルデータにおける上位のコンポーザビリティ](https://github.com/yuk6ra/shinn/assets/59524938/469b3057-10c6-4740-aab1-3b33424a000a)

## Solution

**クレデンシャル・データ特化のCosmos系パブリック・ブロックチェーン**によって、**Interchain Credential Network**（ICCN）を構築する。

![On-Chain Credential Data Dilemma](https://github.com/yuk6ra/shinn/assets/59524938/e0b07a4a-4231-4902-b1e0-5626f014f02b)

簡単に言えば、Interchain版の[Galxe](https://docs.galxe.com/)である。オンチェーンのクレデンシャル・データに特化したApplication-Specific Blockchainを構築し、データ自体をInterchain NFTで管理することにより、ユーザがCosmos IBCに対応するどのチェーンにもデータを自由に移動できるようにする。そして、それらのクレデンシャル・データの利活用を促進し、これまでの社会になかった企業/プロジェクト/コミュニティ/個人の連携を実現する。

![Solution](https://github.com/yuk6ra/shinn/assets/59524938/c3473015-394f-4a96-ac91-f02143b4698f)

### Composability
自然発生的にWeb3プロジェクトの運営者やそれらのユーザが集まるエコシステムをApplication-Specific Blockchainによって構築し、それぞれがWeb3クレデンシャル・データに基づいて、サービス連携を実施しやすくする。

### Scalability
ユーザが発行するクレデンシャル・データは、将来的にスケーラビリティがある形で提供し、ユーザが自己管理できることが理想である。Interchain NFTを利用することで、Cosmos IBCに対応するどのチェーンにもデータを移行し、さらにオンチェーンレベルで通信することを可能にする。

## Value Proposition
### Web3 Projects
新興チェーンやDApps、Web3コミュニティなどのプロジェクト運営者は、柔軟性のあるクレデンシャル・データを簡単に発行できる。シームレスなロイヤリティ・プログラムとユーザとの新しいチャネル、コラボレーションの機会を提供する。

### Users
ユーザは自分の行動や履歴データを完全にコントロールできる。新しいインセンティブ機会と行動・履歴データの自律性を提供し、１つのブロックチェーンに縛られることなく資格証明などのトークンを自由に移動できるような選択肢を提供する。

## Ecosystem
![image](https://github.com/yuk6ra/shinn/assets/59524938/34857ffe-aad2-42cf-a3a2-29dc469fb2dc)

### Legend
![image](https://github.com/yuk6ra/shinn/assets/59524938/507d01c5-8c8b-455a-9b0f-f81233d1f338)

### Details
#### 前提
`Chain_A`には、`DApps_A`や`DApps_B`がある。とあるユーザは`EOA_A`を持ちトランザクションを実行する。

`Chain_B`は、SHINNが提供するブロックチェーンであり、`Interchain NFT Contract`や`Interchain Accounts`がデプロイされている。また、`Interchain NFT Marketplace`もデプロイされている。`Interchain NFT`は、Off-Chain上の`SHINN Frontend`を通して簡単に各プロジェクトが発行できるようになっている。

`Chain_C`には、`DApps_A`、`EOA_A`や`EOA_B`がある。このとき、`EOA_A`の所有者と`EOA_B`の所有者は同一人物である。`EOA_B`で`Chain_A`の`DApps_A`を利用したことがある。

#### フロー
1. `Chain_A`の`DApps_A`はクレデンシャル・データを作成するために、`SHINN Services`を利用して、`Chain_B`に`Interchain NFT Contract`をデプロイする。
2. とあるユーザが持つ`EOA_A`は、今回デプロイされたクレデンシャル・データを発行する権利を持っているので、決定論的に生成された`ICA_A`（Interchain Account）を通して`ICS721_A`（Interchain NFT）をそのウォレットに発行する。
3. 同時期に`Chain_A`の`DApps_B`は独自のキャンペーンをしていて、`ICS721_A`を持っているユーザにエアドロップを実施していた。
4. しかし、そのエアドロップも興味はなく、`ICS721_A`を持っているメリットも他にないため、`Interchain NFT Marketplace`でリストした。
5. とあるユーザが持つ`EOA_B`も`Interchain NFT Contract`から`ICS721_B`というNFTを`ICA_B`に発行した。
6. `ICS721_B`は今後`Chain_C`に`DApps_A`が展開される可能性があり、`EOA_A`で保有しているとインセンティブがあるかもしれない。`EOA_B`から`ICA_B`にトランザクションを送り、`ICS721_B`を`Chain_C`の`EOA_A`に移動させた。

### Example
Interchain NFTがどのように利用され、Interchain NFT Marketplaceがどのように機能するのかの例を示す。

![image](https://github.com/yuk6ra/shinn/assets/59524938/0d6a5b91-6dfd-401d-b4b4-a0b7bc6f450b)


#### 前提
`Chain_A`は、「ポケモンチェーン」というブロックチェーンである。その上には「ポケモンカード」のDAppsがある。

`Chain_B`は、SHINNが提供するブロックチェーンであり、それぞれのチェーンからデプロイされた`Interchain NFT`のコントラクトがあり、それらを売買する `Interchain NFT Marketplace`がある。

`Chain_C`は、「週刊少年ジャンプチェーン」というブロックチェーンである。その上には「ワンピースカード」のDAppsがある。

#### フロー
1. `Chain_A`の`ポケモンカード`DAppsと`Chain_C`の`ワンピースカード`がコラボレーションし、キャンペーンを実施することになった。
2. `Chain_A`の`ポケモンカード`DAppsは、元々`Contract_X`と`Contract_Y`と`Contract_Z`というクレデンシャル・データを発行するコントラクトを持っていた。
3. 今回のコラボレーションのキャンペーンに参加して、新しいNFT（ICS721）を発行するには、`ICS721_α`/`ICS721_β`/`ICS721_γ`の3つを入手する必要がある。
4. しかし、とあるユーザは`ICS721_γ`だけ持っていなかったので、`マーケットプレイス`で購入した。条件としては、最初にミントしたかどうかというクレデンシャル・データは必要がなく、NFTのみが必要であった。
5. 3つのNFTを集めたユーザは、`Contract_A`によって`ICS721_Δ`を発行することができた。これはクレデンシャル・データではなく、記念的なNFTである。
6. 受け取った記念NFTは、個数が制限されているため、`マーケットプレイス`で高額で売買されることもできる。
7. `Chain_A`に移動したとき、その記念NFTは「リザードン」のポケモンカードとしてリビールされ、`Chain_C`に移動したとき、その記念NFTは「シャンクス」のワンピースカードとしてリビールされた。

## Technology Stack
| Title | Description |
| :----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Cosmos SDK](https://docs.cosmos.network/main) | Cosmos SDK is the world’s most popular framework for building application-specific blockchains. |
| [Cosmos IBC](https://tutorials.cosmos.network/academy/3-ibc/1-what-is-ibc.html) | The Inter-Blockchain Communication Protocol (IBC) (opens new window)is a protocol to handle authentication and transport of data between two blockchains |
| [Interchain NFT (ICS721)](https://github.com/cosmos/ibc/tree/main/spec/app/ics-721-nft-transfer) | Interchain NFTs enable users to transfer their digital assets across previously fragmented networks, providing the flexibility to choose which chains their NFTs use|
| [Interchain Account (ICS27)](https://github.com/cosmos/ibc/tree/main/spec/app/ics-027-interchain-accounts) | Interchain Accounts is the Cosmos SDK implementation of the ICS-27 protocol, which enables cross-chain account management built upon IBC. |

### Interchain NFT
![195717720-8d0629c1-dcdb-4f99-8ffd-b828dc1a216d](https://github.com/yuk6ra/shinn/assets/59524938/e8865511-3b20-4c5a-8197-19c0c037a25d)
出典: public-awesome. ICS721. 2023. https://github.com/public-awesome/ics721

### Interchain Account
![1_KwITe2fXgaTUQwvO6Nf7rA](https://github.com/yuk6ra/shinn/assets/59524938/cf09cfaf-93dd-4938-b6a8-13a1f31efd64)

出典: Why Interchain Accounts Change Everything for Cosmos Interoperability. 2020. https://medium.com/chainapsis/why-interchain-accounts-change-everything-for-cosmos-interoperability-59c19032bf11


## Business Models

### Interchain NFTのブロックチェーン・エキスプローラ
主要なクレデンシャル・データとなるInterchain NFTの取引履歴をわかりやすく表示するブロックチェーン・エクスプローラー『ICCN Scan』のウェブアプリケーションを提供し、WalletやPortfolioなどクレデンシャル関連サービスにAPIを提供します。

### クレデンシャル・データ管理ツール
Interchain NFTや顧客となるユーザのウォレットアドレスの管理など行う総合ツール『SHINN』を提供します。このツールでは、マーケティング、キャンペーンや広告の運用、NFTの発行サポート、適切なタイミングによるユーザへの通知などを制御します。

### クレデンシャル・データのマーケットプレイス（Interchain NFT Marketplace）
必要に応じて自身が集めたクレデンシャル・データを売買できるようなInterchain NFTのマーケットプレイスを提供します。デジタル証明書やライセンスなどは対象になりませんが、キャンペーンで配布されたNFTを対象にエアドロップされるような条件だった場合、その特定のNFTは高額で売買されるかもしれません。（事例: Adidas POAP）

### 各プロジェクト同士のコラボレーション支援
相性の良いプロジェクトとのコラボレーションを促進する機会を提供します。DAppsのトランザクションやウォレットのオンチェーン分析による自動レコメンド等も構想中。

## Business Strategy
将来の展開が読めないからこそ、迷ったらとりあえず利用されるクレデンシャル・エコシステムへ
- ユーザのコントラクトウォレットを自動生成する
- ガスレス、無料デプロイ、無料発行（回数制限あり）→POAP感覚で利用できるUI/UX
- 既に発行されたERC721のICS721への変換支援

## Future
- ERC721 to ICS721, ICS721 to ERC721のネイティブ・サポート
- ZKPを活用した個人情報の秘匿化
- 分散型コンテンツプラットフォームの構築
- 経済取引の増加によりクレデンシャルの拡張
- クレデンシャル・ウォレット実装

### ERC721 to ICS721

[![image](https://github.com/yuk6ra/shinn/assets/59524938/ad7922e7-faea-451d-8f6b-087f812dac83)](https://www.youtube.com/watch?v=qpSU19DDgGY)
出典：https://www.youtube.com/watch?v=qpSU19DDgGY

![eth-to-cosmos](https://github.com/yuk6ra/shinn/assets/59524938/da6cb36c-d939-4b63-ab40-65f808e68071)

出典: https://github.com/EmpowerPlastic/Gravity-Bridge/blob/game-of-nfts-stargaze/GAME_OF_NFTS.md

## Discussion
- Interchain NFTのユースケースは？どのような場面で利用できるのだろうか？
- Chain AとChain Bに存在するInterchain NFTはNon-FungibleなTokenなのだろうか？
- クレデンシャル・データのAPIを活用したデータ移行の真贋性はどこまで担保されるのだろうか？
- オンチェーンの信用データは既存の社会でどう役立つのだろうか？どう結びつくのか？
- クレデンシャル・データの存在により、取引にポジティブな影響はあるのだろうか？
- チェーン間の通信速度はアプリケーションのUI/UXにどのように影響を与えるのか？
- IBCで通信可能なデータをChain AからChain Bに移行するモチベーションはどこだろうか？
- クレデンシャル・データ利用頻度の観点からのInterchain NFT化は必要か？
- Specific-chainまたはDappsで展開するそれぞれのメリデメはなんだろうか？
- UptickとGravityBridgeによるERC-721 to ICS-721の違いや機能はどうなっているのか？

## Slide
| Title | Note |
| :----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|[SHINN v0](https://www.canva.com/design/DAFptydpLG8/rlL88iDgzl-KUl5CRbXYIQ/view?utm_content=DAFptydpLG8&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)| Draft  |


## References
- Web3 Credentials – All You Need To Know. 2023. https://thehyperstack.com/blog/web3-credentials-all-you-need-to-know/
- Interchain NFT: a protocol for bridging assets between chains. The Interchain Foundation. 2023. https://medium.com/the-interchain-foundation/interchain-nft-a-protocol-for-bridging-assets-between-chains-9473cd47cba7
- Gjermund Garaba, kwarantyna. NFTokenizer. 2023. https://dorahacks.io/buidl/6484

