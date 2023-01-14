# Yew Sample App

A sample [Yew](https://yew.rs/) app that displays a button and a number. When
the button is clicked, the number increases by one. Yew code is written in Rust
and compiles to WASM. This sample app is based on [Build a sample app on
Yew.rs](https://yew.rs/docs/getting-started/build-a-sample-app)

## Installing

Go to https://www.rust-lang.org/tools/install and follow the instructions to
install Rust.

Add the WebAssembly target to your development environment

```sh
rustup target add wasm32-unknown-unknown
```

Install trunk

```sh
cargo install --locked trunk
```

Clone this repository

```sh
git clone https://github.com/travishorn/yew-sample-app
```

Change into the directory

```sh
cd yew-sample-app
```

## Development

Serve the app for development

```sh
trunk serve
```

Navigate to http://127.0.0.1:8080/ in your web browser.

Edit `./src/main.rs` to modify the app. Changes are hot reloaded in your
browser.

## Deployment

Build for production

```sh
trunk build --release
```

Set your web server to serve the built files in `./dist`

## License

The MIT License (MIT)

Copyright © 2023 Travis Horn

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the “Software”), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
