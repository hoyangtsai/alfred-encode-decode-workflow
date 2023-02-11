# Alfred Encode / Decode

[Download v1.11](https://raw.github.com/hoyangtsai/alfred-encode-decode-workflow/master/encode-decode.alfredworkflow)

Encoding and decoding a string into multiple variations.

## Requirements

1. [Alfred App](http://www.alfredapp.com/#download)
2. [Alfred Powerpack](https://buy.alfredapp.com/)

### macOS Monterey (12.0) compatibility

Starting in macOS Monterey, there won't be any PHP runtime (which is required for this workflow) bundle with the OS.

To Solve this issue, follow these steps:

1. Install Homebrew with the command provided on its [homepage](https://brew.sh/)
2. Install PHP@7.4 runtime with Homebrew

```shell
brew install php@7.4
```

If seeing this error

```sh
Error: php@7.4 has been disabled because it is a versioned formula!
```

Use another source to install php@7.4

```sh
brew tap shivammathur/php
brew install shivammathur/php/php@7.4
```

More info: [Homebrew/homebrew-core #120854](https://github.com/Homebrew/homebrew-core/issues/120854)


Note: If you've installed php with homebrew previously, you also need to
 
```shell
brew unlink php
brew link php@7.4
```

The scripts had updated for you, just installing this version from here.

> For more info refer to [willfarrell/alfred-encode-decode-workflow/issues/26](https://github.com/willfarrell/alfred-encode-decode-workflow/issues/26)

## About

Will transform your query strings through *base64*, *html*, *url*, and *utf-8* encode/decode. Pressing enter will copy the encoded/decoded string to the clipboard.

![alt text][encode]

![alt text][decode]

## Commands

- `encode {query}` - Encode magic
- `decode {query}` - Decode magic

## Contributors

- [@willfarrell](https://github.com/willfarrell)
- [@cvn](https://github.com/cvn)

## Mentions

- [15 Alfred Workflows to Turbocharge Productivity](http://www.bachyaproductions.com/15-alfred-workflows-turbocharge-productivity/)

[encode]: ./screenshots/encode.png "Encode"
[decode]: ./screenshots/decode.png "Decode"
