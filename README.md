# cargo-relative

A wrapper around [Cargo](http://crates.io) to use it as `makeprg` in Vim with
`autochdir` set. Only outputs Cargo's stderr and converts paths relative to the
project directory to be relative to the current directory.

To use it as `makeprg` put the following in `~/.vim/after/ftplugin/rust.vim`:

```VimL
setlocal makeprg=path/to/repository/cargo-relative\ build
```

Then calling `:make` in Rust buffers should execute Cargo and properly populate
the quickfix buffer.
