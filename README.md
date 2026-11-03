# NODE COFFEE ROASTERS (Project NODE)

> **A culture-hub specialty coffee ecosystem designed with scalable, event-driven, and decoupled architecture.**

藤沢・茅ヶ崎エリアにおけるスペシャルティコーヒーの「結節点（Node）」となるロースタリーカフェの立ち上げプロジェクト。  
単なる飲食店の1プレーヤーではなく、地域のショップや愛好家、アート、食を結び、カルチャーを共創・牽引するプラットフォームを目指します。

---

## 1. Concept & Vision

- **Core Mission**: コーヒーを通じて日常に確かな「幸せ」と豊かな循環を届ける。
- **Hub Strategy**: 近隣のコーヒーショップを排他的な競合とせず、相互紹介や合同イベント等を通じてエリア全体のコーヒー消費・カルチャーを底上げする「ハブ」として機能する。
- **Design Philosophy**: エンジニアリング思想に基づく高可用性・スケーラビリティ・属人性排除（No SPOF）。

---

## 2. Architecture & Operations

現場オペレーションを極限までモジュール化・標準化し、少人数（スタッフ1〜2名）で高品質な体験を提供しつつ、オーナーが現場に張り付かない体制を構築します。

### System Overview

| Module | Implementation | Characteristics |
| :--- | :--- | :--- |
| **Black Coffee** | Batch Brew (浅煎り / 深煎り 日替わり2種) | 提供レイテンシを極小化。安定した抽出品質を保証し、朝のクイック需要にも対応。 |
| **Espresso** | On-demand Extraction | 注文ごとに抽出。カフェラテ等で本格的なシズル感と高品質を提供。 |
| **Bake / Food** | OEM Outsource (ecomo Bakery 想定) | 店舗仕込みを排し、地域で絶大な支持を得る高品質な英国式スコーンを提供。リベイク提供のみ。 |
| **POS / Cashier** | Square (完全キャッシュレス) | 現金管理・締め作業のゼロ化。購買データ取得とCRM連携。 |
| **Roasting Engine** | aillio Bullet R1 (Phase 1) | Roastime によるプロファイルの完全データ化・再現性の担保。 |
| **Staff Role** | Front-end Communication | ルーチンワークから解放された時間を「試飲提案」「豆の紹介」「WS告知」などの高付加価値な対話に全振り。 |

---

## 3. UI / Space Design

「ストイックな専門性」と「心地よいコミュニティ感」が共存する洗練された空間設計。

- **Base Tone (70%)**: Matte Black / Dark Charcoal / Mortar
  - aillioのマットブラック筐体やデータモニターが美しく溶け込むダークモード的ストイックさ。
- **Assort Tone (20%)**: Houseplants (Greenery)
  - 大型の観葉植物や塊根植物による有機的な温もりと生命感。
  - 黒い壁面に映えるコントラスト。
- **Accent Tone (10%)**: Pop Art & Graphics
  - ビビッドな色彩と遊び心のあるアートピースを配置（地元クリエイターの展示機能も兼ねる）。
- **Food Presentation**: 
  - 黒のマットプレート（波佐見焼等）に黄金色のスコーン、白いクロテッドクリーム、赤いジャムを美しく際立たせる。

---

## 4. Business Model & Unit Economics

### Revenue Streams
1. **In-Store**: ドリンク（バッチブリュー／ラテ）、スコーンペアリング
2. **Retail**: 自家焙煎豆（100g〜200g）、抽出器具、オリジナルマーチ
3. **Event-driven**: 焙煎・抽出・飲み比べワークショップ（高粗利モジュール）

### Phase Roadmap

- **Phase 1: Minimum Viable Node (本店プロトタイプ)**
  - エリア: 茅ヶ崎・辻堂・藤沢（12〜15坪、客席10〜12席 + アイランドカウンター）
  - 機材: aillio Bullet R1
  - 体制: オーナー（週1〜2日焙煎・WS講師・提携開拓）＋ 常時スタッフ1〜2名
  - マイルストーン: 地域のハブとしての認知獲得、黒字化、マニュアルの完成
- **Phase 2: Scale & Dominant (セントラル化とサテライト展開)**
  - 大型焙煎機（5kg〜10kgクラス）導入によるセントラルロースタリーの確立。
  - 近隣駅前・生活動線へのサテライト店舗（5〜10坪の軽量スタンド）ドミナント出店。
  - 湘南コーヒーフェス等のエリア規模イベントの主導。

---

## 5. Next Milestones (Backlog)

- [ ] 物件選定スペックシートの策定（電気容量・排気・坪数12〜15坪・アイランド配置可否）
- [ ] ecomo Bakery への提携・仕入れ交渉プロトコル設計
- [ ] 収支計画（損益分岐点・初期投資・ランニングコスト）のモデル化
- [ ] ブランドVI（ロゴ・フォント・カラースキーム）の設計
- [ ] スタッフ向けオペレーションマニュアル（Notion等）のプロトタイプ作成
