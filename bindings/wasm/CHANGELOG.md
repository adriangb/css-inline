# Changelog

## [Unreleased]

### Added

- `data-css-inline="ignore"` attribute to ignore CSS inlining. [#10](https://github.com/Stranger6667/css-inline/issues/10)

## [0.8.2] - 2022-11-01

### Fixed

- Ignoring selectors' specificity when applying declarations from different qualified rules. [#148](https://github.com/Stranger6667/css-inline/issues/148)

### Changed

- Unpin `parking_lot_core`.
- Remove deprecated `wee_alloc`.

## [0.8.1] - 2022-07-21

### Fixed

- Not respecting specificity in case of inlining overlapping rules like `padding` and `padding-top`. [#142](https://github.com/Stranger6667/css-inline/issues/142)
- `!important` rules not overriding inlined styles. [#152](https://github.com/Stranger6667/css-inline/issues/152)

## [0.8.0] - 2022-01-10

### Fixed

- Invalid handling of double-quoted property values like in `font-family: "Open Sans"`. [#129](https://github.com/Stranger6667/css-inline/issues/129)
- An error about missing `env` dependency.

## [0.7.5] - 2021-07-24

### Fixed

- Panic on invalid URLs for remote stylesheets.

## [0.7.4] - 2021-07-06

### Performance

- Optimize loading of external files.

## [0.7.3] - 2021-06-24

### Performance

- Improve performance for error handling.

## [0.7.2] - 2021-06-22

### Fixed

- Incorrect override of exiting `style` attribute values. [#113](https://github.com/Stranger6667/css-inline/issues/113)

### Performance

- Minor performance improvements

## [0.7.1] - 2021-06-10

### Fixed

- Ignored `style` tags when the document contains multiple of them and the `remove_style_tags: true` config option is used. [#110](https://github.com/Stranger6667/css-inline/issues/110)

## [0.7.0] - 2021-06-09

### Fixed

- Ignored selectors specificity. [#108](https://github.com/Stranger6667/css-inline/issues/108)

## [0.6.1] - 2020-12-07

### Fixed

- Compatibility with the new `cssparser` crate version.

### Performance

- Avoid string allocations during converting `InlineError` to `JsValue`.

## [0.6.0] - 2020-11-02

### Changed

- Links to remote stylesheets are deduplicated now.

### Performance

- Use `Formatter.write_str` instead of `write!` macro in the `Display` trait implementation for `InlineError`. [#85](https://github.com/Stranger6667/css-inline/issues/85)
- Use `Cow` for error messages. [#87](https://github.com/Stranger6667/css-inline/issues/87)

## [0.5.0] - 2020-08-07

### Performance

- Avoid string allocation in `get_full_url`

## [0.4.0] - 2020-07-13

- Initial public release

[Unreleased]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.8.2...HEAD
[0.8.2]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.8.1...wasm-v0.8.2
[0.8.1]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.8.0...wasm-v0.8.1
[0.8.0]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.7.5...wasm-v0.8.0
[0.7.5]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.7.4...wasm-v0.7.5
[0.7.4]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.7.3...wasm-v0.7.3
[0.7.3]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.7.2...wasm-v0.7.3
[0.7.2]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.7.1...wasm-v0.7.2
[0.7.1]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.7.0...wasm-v0.7.1
[0.7.0]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.6.1...wasm-v0.7.0
[0.6.1]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.6.0...wasm-v0.6.1
[0.6.0]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.5.0...wasm-v0.6.0
[0.5.0]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.4.1...wasm-v0.5.0
[0.4.1]: https://github.com/Stranger6667/css-inline/compare/wasm-v0.4.0...wasm-v0.4.1
