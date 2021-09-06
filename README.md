[![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/gogo-pats/rust-webassembly)
[![Rust](https://img.shields.io/badge/Rust-b7410e.svg?longCache=true)](https://www.rust-lang.org/ja)

## Rustバージョン確認

```
cargo --version
rustc -V
rustup -V
rustup show
```

---

## インストール作業

### Rust で WebAssemblyを構築するためのツール

```
cargo install wasm-pack
```

### テンプレートプロジェクトを生成してくれる便利ツール(1度だけ)

```
cargo install cargo-generate
```

### プロジェクトを生成(1度だけ)

```
cargo generate --git https://github.com/rustwasm/wasm-pack-template --name myproject
cd myproject
```

---

## コンパイル

### WebAssembly パッケージコンパイル
```
cd myproject
wasm-pack build
```

### Webプロジェクトを生成

```
cd myproject
npm init wasm-app www
```
index.jsを編集


### 依存パッケージをインストール
```
cd myproject/www
npm install
```

### ローカルのパッケージリンク

```
cd myproject/pkg
npm link

cd myproject/www
npm link myproject
```

---

## 実行 ここは毎回

```
cd myproject/www
npm run start
```
