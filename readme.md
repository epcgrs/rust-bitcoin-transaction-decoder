# Transaction Decoder

A Rust-based utility for decoding transaction data from raw bytes.

## Overview

This project provides functionality to parse and decode transaction data structures, starting with version information extraction from transaction byte arrays.

## Features

- **Version Reading**: Extract version information from transaction byte streams
- **Transaction Parsing**: Decode raw transaction bytes into structured data
- **Hex Support**: Built-in support for hexadecimal data handling

## Dependencies

- `hex 0.4.3` - For hexadecimal encoding/decoding operations

## Project Structure

```
transaction-decoder/
├── src/
│   └── main.rs          # Main application logic
├── Cargo.toml           # Project configuration and dependencies
└── readme.md           # Project documentation
```

## Getting Started

### Prerequisites

- Rust 1.70+ (using Rust 2024 edition)
- Cargo package manager

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd transaction-decoder
```

2. Build the project:
```bash
cargo build
```

3. Run the application:
```bash
cargo run
```

### Usage

The main functionality revolves around the `read_version` function which extracts version information from transaction byte arrays:

```rust
fn read_version(transaction_bytes: &mut &[u8]) -> u32 {
    // Implementation for reading version from byte stream
}
```

## Development

### Building

To build the project in release mode:
```bash
cargo build --release
```

### Testing

Run tests with:
```bash
cargo test
```

## Configuration

The project is configured to use:
- **Rust Edition**: 2024
- **Version**: 0.1.0

## Course
For a comprehensive guide on Rust programming, consider enrolling in the course: [Intro to Rust and Bitcoin](https://btcdemy.thinkific.com/courses/intro-to-rust)

## License

MIT