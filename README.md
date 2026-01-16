[![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)](https://github.com/ThiagoAVicente/sfs-cli)
# Semantic File Search

A semantic file search system that uses vector embeddings to enable natural language queries across your documents.

## Overview

SFS allows you to index files and search their content using natural language queries. Instead of searching for exact keywords, you can ask questions like "what does this say about deployment?" and get relevant results.

## Architecture

![[architecture.png]]
## Components

| Component       | Description                                            | Link                                                    |
| --------------- | ------------------------------------------------------ | ------------------------------------------------------- |
| **sfs-api**     | FastAPI backend with vector search and file management | [GitHub](https://github.com/ThiagoAVicente/sfs-api)     |
| **sfs-desktop** | Cross-platform desktop GUI built with Tauri + React    | [GitHub](https://github.com/ThiagoAVicente/sfs-desktop) |
| **sfs-cli**     | Command-line interface to use SFS                      | [GitHub](https://github.com/ThiagoAVicente/sfs-cli)     |

> **Note:** Desktop and CLI don't provide the same features

## Quick Start

### CLI

Lightweight and easy to use, the CLI provides a command-line interface for uploading and searching documents. Has more features such as `Watch` to auto upload files when they are modified.

### Desktop App

More intuitive than the CLI, the desktop app provides a graphical interface for uploading and searching documents.
> see [sfs-desktop README](https://github.com/ThiagoAVicente/sfs-desktop)

## Hosting 
### Self-Hosting

See the [sfs-api README](https://github.com/ThiagoAVicente/sfs-api) for deployment instructions using Docker Compose.

## Features

- **Semantic Search**: Query documents using natural language
- **File Storage**: S3-compatible storage server
- **Async processing**: Distribute work for parallel processing
- **Encryption**: Server-side encryption for stored files

## Tech Stack

- **Backend**: Python, FastAPI, Minio, Qdrant
- **Frontend**: React, Tauri, TypeScript
- **CLI**: Go, Cobra

## License

See individual repositories for license information.
