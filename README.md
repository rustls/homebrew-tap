# homebrew-tap

Third-party [Homebrew](https://brew.sh) repository for [rustls-ffi](https://github.com/rustls/rustls-ffi) related packages.

## Installation

```
brew tap rustls/tap
brew install rustls/tap/curl
```

See also [Homebrew documentation for Taps](https://docs.brew.sh/Taps).

## FAQ

```
cargo: error while loading shared libraries: librustls.so.0.14.0: cannot open shared object file: No such file or directory
```

In some cases you may need to manually rebuild your rustls-linked curl binary/library after updating the rustls-ffi package, this can be done with the following command. If you know of a way to have homebrew automatically detect this please let us know. ✨

```
brew reinstall rustls/tap/curl
```
