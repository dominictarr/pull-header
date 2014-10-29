# pull-header

read a fixed length binary header from a pull-stream.

``` js
pull(
  binarySource,
  header(196, function (data) {
    //this is a 196 byte header from the start of the stream.
    console.log('head:', data)
  }),
  pull.drain(function (chunk) {
    console.log('body chucnk', chunk)
  }))

```

## License

MIT
