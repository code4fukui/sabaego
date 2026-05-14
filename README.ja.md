# sabaego

地域の共同探索と課題報告を目的とした位置情報ゲーム（コードネーム: 鯖江GO）。このプロジェクトは、[Taisuke Fukuno](http://fukuno.jig.jp/1326)氏による[gsimaps](https://github.com/gsi-cyberjapan/gsimaps)の改修版です。

## 機能
- **チームベースのゲームプレイ**: 開始・終了時刻や探索エリアを割り当てたチームを編成できます。
- **リアルタイム位置情報トラッキング**: チームメンバーの現在位置を地図上でリアルタイムに確認できます。
- **課題報告**: 地域の課題（`sabarepo`）を報告し、報酬としてバーチャルアイテム（文化財など）を収集できます。
- **ゲーミフィケーション**: 収集したアイテムの数や種類に基づくスコアリングシステム。
- **ポスティングツール**:
    - 建物タイプ（集合住宅、戸建てなど）の区別。
    - 「ポスティング禁止」エリアのマーキングと識別。
    - 既にカバー済みのエリアに対する警告の受信。
    - カスタムの地図上ボタンを使用したデータ入力（例：「ポスティングNG」「手渡し」「富裕度評価」）。
    - 既存顧客など、特定の住所に対するアラート設定。

## デモ（ベースプロジェクト）
本プロジェクトは改修されたフォーク版であるため、ベース機能についてはオリジナルの `gsimaps` プロジェクトをご参照ください:
- **公式 地理院地図:** http://maps.gsi.go.jp/
- **地理院地図（リポジトリデモ）:** http://gsi-cyberjapan.github.io/gsimaps/

## 使い方
1. 本リポジトリをダウンロードまたはクローンします。
2. ファイル一式をWebサーバーに配置します。
3. ブラウザで `index.html` を開きます。

*注: ローカルのファイルシステムから `index.html` を開いても多くの機能は動作しますが、ベクタータイルデータの処理など、すべての機能を完全に動作させるにはWebサーバーが必要です。*

## 依存関係
- [地理院地図](https://github.com/gsi-cyberjapan/gsimaps)（国土地理院）ベース
- [Leaflet](LICENSE_LIBRARIES.md)
- [jQuery 1.11.1](jquery/jquery-1.11.1.min.js) & [jQuery UI](jquery/jquery-ui.min.js)
- [ZeroClipboard 2.0.2](jquery/ZeroClipboard2.0.2/)

## 外部サービスとAPI
- [東京大学CSIS](http://newspat.csis.u-tokyo.ac.jp/geocode/)のジオコーディングサービスを利用しています。
- **免責事項:** サーバーサイドのサービスは、常に稼働していること、および永続的に稼働していることは保証されません。また、事前通知なしに更新または廃止される可能性があります。

## 関連ツール（gsimapsより）
- レイヤ定義ファイル編集ツール *(demo unavailable)*
- [レイヤ定義仕様書](https://github.com/gsi-cyberjapan/layers-dot-txt-spec)

## ライセンス
国土地理院（GSI）によるオリジナルの著作物は、2-clause BSD licenseの下で提供されています。詳細は[LICENSE](LICENSE)および[LICENSE_LIBRARIES.md](LICENSE_LIBRARIES.md)を参照してください。
