# Why Rust and WebAssembly?

## Low-Level Control with High-Level Ergonomics

JavaScript Webアプリケーションは、信頼できるパフォーマンスを達成して維持するのに苦労しています。
JavaScriptの動的型システムとガベージコレクションの一時停止は役に立ちません。
一見小さなコード変更は、誤ってJITの幸せな道をさまよった場合、劇的なパフォーマンスの低下をもたらす可能性があります。

Rustは、プログラマーに低レベルの制御と信頼性の高いパフォーマンスを提供します。
JavaScriptを悩ませている非決定論的なガベージコレクションの一時停止はありません。
プログラマーは、間接参照、単相化、およびメモリーレイアウトを制御できます。

## Small `.wasm` Sizes

`.wasm`はネットワーク経由でダウンロードする必要があるため、コードサイズは非常に重要です。
Rustにはランタイムがなく、ガベージコレクターのように余分な肥大化が含まれていないため、小さな `.wasm`サイズが可能になります。
実際に使用する関数に対してのみ（コードサイズで）支払います。

## Do *Not* Rewrite Everything

既存のコードベースを破棄する必要はありません。
パフォーマンスに最も敏感なJavaScript関数をRustに移植することから始めて、すぐにメリットを得ることができます。
また、あなたの望む段階で移植をやめることができます。

## Plays Well With Others

RustとWebAssemblyは、既存のJavaScriptツールと統合されています。
ECMAScriptモジュールをサポートしており、npmやWebpackなどのすでに気に入っているツールを引き続き使用できます。

## The Amenities You Expect

Rustには、開発者が期待するようになった、以下のような最新のサービスがあります。

* `cargo` による強力なパッケージ管理、

* 表現力豊かな（そしてゼロコストの）抽象化、

* コミュニティへの歓迎！ 😊
