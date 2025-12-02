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
