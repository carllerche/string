# String

A UTF-8 encoded string with configurable byte storage.

[![Crates.io](https://img.shields.io/crates/v/string.svg?maxAge=2592000)](https://crates.io/crates/string)
[![Build Status](https://travis-ci.org/carllerche/string.svg?branch=master)](https://travis-ci.org/carllerche/string)

[Documentation](https://docs.rs/string)

## Usage

To use `string`, first add this to your `Cargo.toml`:

```toml
[dependencies]
string = "0.1"
```

Next, add this to your crate:

```rust
extern crate string;

use string::{String, TryFrom};

let s: String<[u8; 2]> = String::try_from([b'h', b'i']).unwrap();
assert_eq!(&s[..], "hi");
```

See [documentation](https://docs.rs/string) for more details.

# License

`string` is primarily distributed under the terms of both the MIT license and
the Apache License (Version 2.0), with portions covered by various BSD-like
licenses.

See LICENSE-APACHE, and LICENSE-MIT for details.
