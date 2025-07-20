# 🌀 index_permute

A minimal, **in-place**, and **non-cloning** array permutation library for Rust.

This crate allows you to **reorder a slice in place by an index array**, even when the element type is **not `Clone` or `Copy`**. It ensures safety via a wrapper type `PermuteIndex` that checks index validity ahead of time.

---

## ✨ Features

- ✅ In-place permutation of non-`Copy`, non-`Clone` data.
- ✅ Memory-safe: no element dropped or cloned during permutation.
- ✅ Index validation: ensures the index is a true permutation (`0..N`).
- ✅ Safe, ergonomic API.
- 🚧 `parallel` feature is defined but **not yet implemented**.

---

## 📦 Installation

Add this to your `Cargo.toml`:

```toml
[dependencies]
index_permute = 0.1
