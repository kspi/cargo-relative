# cargo-relative

A wrapper around [Cargo](http://crates.io) to use it as `makeprg` in Vim. Only
outputs Cargo's stderr and converts paths relative to the project directory to
be relative to the current directory.
