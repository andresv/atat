# `AT Parser`

> A driver support crate for AT-command based serial modules, using the [embedded-hal] traits.


[embedded-hal]: https://crates.io/crates/embedded-hal

## [Documentation](https://docs.rs/at-rs/latest/at-rs/)

## Tests

> The crate is covered by tests using the [embedded-hal-mock] crate. These tests can be run by `cargo test --lib --target = x86_64-unknown-linux-gnu` or the `cargo th` alias.

[embedded-hal-mock]: https://crates.io/crates/embedded-hal-mock

## Examples

The crate has examples for usage with [cortex-m-rt] and [cortex-m-rtfm] crates.

Furthermore I have used the crate to build initial drivers for uBlox cell modules ([ublox-cell-rs]) and uBlox wifi modules ([ublox-wifi-rs])

[cortex-m-rt]: https://crates.io/crates/cortex-m-rt
[cortex-m-rtfm]: https://crates.io/crates/cortex-m-rtfm
[ublox-wifi-rs]: https://crates.io/crates/ublox-wifi-rs
[ublox-cell-rs]: https://crates.io/crates/ublox-cell-rs

## About

    - Minimum rustc version 1.31
    - Tested and built using nightly toolchain, but should work fine for stable as well

## Supported Crates

The following dependent crates provide platform-agnostic device drivers built on `embedded-hal` which also implement this crate's [`ATCommandInterface`] trait:

| Device Name | Description | Crate + Docs |
|-------------|-------------|--------------|
| [ublox-wifi-rs]  | Driver crate for UBlox host-based wifi devices with AT-command interface | [![crates.io][ublox-wifi-rs-crate-img]][ublox-wifi-rs] [![docs.rs][ublox-wifi-rs-docs-img]][ublox-wifi-rs-docs] |
| [ublox-cell-rs]  | Driver crate for UBlox host-based cellular devices with AT-command interface | [![crates.io][ublox-cell-rs-crate-img]][ublox-cell-rs] [![docs.rs][ublox-cell-rs-docs-img]][ublox-cell-rs-docs] |

[ublox-wifi-rs]: https://github.com/MathiasKoch/ublox-wifi-rs
[ublox-wifi-rs-crate-img]: https://img.shields.io/crates/v/ublox-wifi-rs.svg
[ublox-wifi-rs-docs-img]: https://docs.rs/ublox-wifi-rs/badge.svg
[ublox-wifi-rs-docs]: https://docs.rs/ublox-wifi-rs/

[ublox-cell-rs]: https://github.com/MathiasKoch/ublox-cell-rs
[ublox-cell-rs-crate-img]: https://img.shields.io/crates/v/ublox-cell-rs.svg
[ublox-cell-rs-docs-img]: https://docs.rs/ublox-cell-rs/badge.svg
[ublox-cell-rs-docs]: https://docs.rs/ublox-cell-rs/

## License

Licensed under either of

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
  http://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.
