# ocrs

This crate contains the **ocrs** OCR engine as a library. See the
[main project README][main_readme] for general details about the project.

[main_readme]: https://github.com/robertknight/ocrs/blob/main/README.md

## Performance note

Make sure you build the `ocrs` crate and its `rten*` dependencies in **release
mode**. Debug builds of these crates will be extremely slow.

## Usage

See [examples/hello_ocr/](./examples/hello_ocr/README.md) for a minimal example of using this library in
a Rust application.

```sh
cd examples/hello_ocr

# Download models in .rten format.
./download-models.sh

# Run OCR on an image and print the extracted text.
cargo run --release rust-book.jpg
```
