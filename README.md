# Bazel C++ Hello, World!

シンプルな Bazel + C++ の "Hello, Bazel!" プロジェクトです。

## 前提
- Bazel（または Bazelisk）
- C++ コンパイラ（`clang` または `g++`）

macOS で Bazel がない場合:

```bash
brew install bazelisk  # `bazel` コマンドとして利用可
```

## ファイル構成
- `WORKSPACE`: 空のワークスペース定義
- `BUILD`: `hello_world` バイナリのビルドルール
- `main.cc`: 標準出力に "Hello, Bazel!" を表示

## ビルド
```bash
bazel build //:hello_world
```

## 実行
```bash
bazel run //:hello_world
# 期待される出力:
# Hello, Bazel!
```

## クリーン
```bash
bazel clean
```

## メモ
- 依存関係はなく、空の `WORKSPACE` で動作します。
- Bazelisk を使うと Bazel のバージョン管理が容易です。
