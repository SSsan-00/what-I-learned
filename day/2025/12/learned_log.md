# 2025/12/01
## Rust
- 範囲
  -  `std::ops::Ranze<T>`
- スライス
  - 実際にコードを組んで体で覚える
  - なんか便利そう程度の解像度。。。
  - スライシング
    > 配列やベクターからスライスを切り出す
  - 空のスライス
    ```Rust
    let arr = [55, 33, 66, 22];
    let _r1 = 4..4;
    ```
  - usize型が要求される

# 2025/12/02
## Rust
- 文字列の文字コードは`UTF-8`

## React
- ReactElement
- `React.createElement(・・・)`
- コンポーネント思考
  - MVCの考え方と違う
  > どっちがいいのやら。。<br>
  > 慣れているのは圧倒的にMVC
- jsxはXMLだからHTML以外でもインポート次第で表現できる
  > ex)react native
- JSXのトップレベルは要素が一つでないといけない
- フラグメント
  > `<></>`<br>
  > トップレベルの要素を一つにして無駄な親要素を作らないで済んで便利
- JSXで戻り値がBoolean型なら何もレンダリングしない

# 2025/12/03
## Rust
- イテレータ
  - カーソルとも
  - いわゆるforeachのアレ
  > 引数の文字列と文字コード(10進数)を出力するコード⇩
  ```Rust
  fn main() {
    fn print_codes(s: &str) {
      for c in s.chars() {
        println!("{}: {}", c, c as u32);
      }
    }
    print_codes("aあ1");
  }
  ```

# 2025/12/04
- Windowsセットアップ
  - Chromeインストール＆同期
  - ChatGPTログイン
  - WIndowsアップデート
  > エディタはNeoVimにしてみようかな笑
## 行脚アプリ要件定義
### プログラミング言語・フレームワーク
  - TypeScript
  - Tailwind CSS
  - Next.js
### DB
  - Supabase(PostgresSQL)
パッケージマネージャ
  - pnpm
### テストフレームワーク
  - Vitest
  - React Testing Library
### CI/CD
  - Github Actions
### デプロイ先
- Vercel
### エディタ
- vscode
### その他
- TDDでスモールステップで進める
- 開発を共有できるように環境がある程度整ったらDockerファイルを作成する
	- 開発ログとして0から環境を0から作成する手順も記録していく


# 2025/12/05
## 行脚アプリ
- 環境構築
```
// プロジェクトの初期化
pnpm dlx create-next-app@latest angya-app \
	—typescript \
	—tailwind \
	—eslint \
	—app \
	—src-dir false \
	—import-alias “@/*”

cd angya-app

// パッケージのインストール
pnpm install
// サーバーの起動
pnpm dev

// 以下のパスにブラウザでアクセス
http://localhost:3000
```
# 2025/12/06
- JS解析
  > JSのリーディング久しぶりにやったけど楽しい
  > ライブラリの処理になった瞬間カロリー爆増(事前知識がない。。)

# 2025/12/07
- スタンドアローンテストランナー作成

# 2025/12/08
- テストランナー改修
