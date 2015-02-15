Wrapper library for low level sass-sys
https://github.com/compass-rs/sass-sys

The sass-sys library wraps libsass
https://github.com/sass/libsass

This is work in progress. To test that it works run the examples

```
cargo run --example versions

Running `target/examples/versions`
libsass: 3.1.0-beta.2-2-g420d
sass2scss: 1.0.3
```


The example below expands sass variables and calls custom functions defined in Rust.

```
cargo run --example compile_sass examples/simple.scss

Running `target/examples/compile_sass examples/simple.scss`
Compiling sass file: `examples/simple.scss`.
------- css  ------
body {
  font: 100% Helvetica, sans-serif;
  color: #333;
  content: foo-ed; }
--------
```
