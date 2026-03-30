# namefyi

[![crates.io](https://img.shields.io/crates/v/namefyi.svg)](https://crates.io/crates/namefyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Korean romanization, Five Elements, and CJK stroke lookup — API client for [namefyi.com](https://namefyi.com).

> **Try the interactive tools at [namefyi.com](https://namefyi.com)**

## Install

`cargo add namefyi`

## Quick Start

```rust
use namefyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("minjun").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install namefyi` | [PyPI](https://pypi.org/project/namefyi/) |
| **npm** | `npm install namefyi` | [npm](https://www.npmjs.com/package/namefyi) |
| **Go** | `go get github.com/fyipedia/namefyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/namefyi-go) |
| **Rust** | `cargo add namefyi` | [crates.io](https://crates.io/crates/namefyi) |
| **Ruby** | `gem install namefyi` | [rubygems](https://rubygems.org/gems/namefyi) |

## Embed Widget

Embed [NameFYI](https://namefyi.com) widgets on any website with [namefyi-embed](https://widget.namefyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/namefyi-embed@1/dist/embed.min.js"></script>
<div data-namefyi="entity" data-slug="minjun"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.namefyi.com)

## Links

- [NameFYI](https://namefyi.com) — Main site
- [API Documentation](https://namefyi.com/developers/)
- [OpenAPI Spec](https://namefyi.com/api/openapi.json)
- [Glossary](https://namefyi.com/glossary/)

## License

MIT
