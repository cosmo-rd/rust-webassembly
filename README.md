## Rustバージョン確認

```
cargo --version
rustc -V
rustup -V
rustup show
```

## インストール作業

### Rust で WebAssemblyを構築するためのツール

```
cargo install wasm-pack
```

### テンプレートプロジェクトを生成してくれる便利ツール

```
cargo install cargo-generate
```

### プロジェクトを生成

```
cargo generate --git https://github.com/rustwasm/wasm-pack-template --name myproject
cd myproject
```

### コンパイル

```
wasm-pack build
```




