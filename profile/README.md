<div align="center">

# KeraDB

**A lightweight, embedded NoSQL document database with vector search, written in Rust**

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)]()
[![Rust](https://img.shields.io/badge/rust-1.70%2B-orange)]()
[![License](https://img.shields.io/badge/license-MIT-blue)]()

</div>

---

## What is KeraDB?

KeraDB is a **single-file, embedded document database** designed for simplicity and performance. Think SQLite, but for JSON documents with built-in **vector search** capabilities!

### Key Features

| Feature | Description |
|---------|-------------|
| **Single-file database** | One `.ndb` file contains everything |
| **Fast** | Written in Rust with zero-cost abstractions |
| **Memory-safe** | Rust's guarantees prevent crashes and data corruption |
| **Vector Search** | HNSW index for fast approximate nearest neighbor search |
| **Delta Compression** | LEANN-style compression with up to 97% storage savings |
| **Multi-language SDKs** | Rust, Node.js, Python, Go, C#, and more |

---

## Repositories

| Repository | Description |
|------------|-------------|
| [**keradb**](https://github.com/KeraDB/keradb) | Core database engine and CLI |
| [**keradb-labs**](https://github.com/KeraDB/keradb-labs) | Desktop GUI app with Tauri + React |
| [**keradb.github.io**](https://github.com/KeraDB/keradb.github.io) | Documentation website |

---

## Quick Start

```bash
# Install KeraDB CLI
curl -sSf https://keradb.github.io/quickstart.sh | sh

# Create a database and start the shell
keradb shell myapp.ndb

# Insert and query documents
keradb> insert users {"name": "Alice", "age": 30}
keradb> find users
```

---

## Performance

- **Sub-40us** vector search on 10K vectors
- **~50K ops/sec** document lookups
- **~9K vectors/sec** bulk insert rate
- **Up to 97%** compression for similar vectors

Check out our latest benchmark [here](https://keradb.github.io/blog/keradb-vs-sqlite-benchmark-v0-1-0)
---

## Contributing

We welcome contributions! Check out our repositories and feel free to open issues or submit pull requests.

---

<div align="center">

**Built with Rust**

[Documentation](https://keradb.github.io) | [Getting Started](https://github.com/KeraDB/keradb#quick-start)

</div> 
