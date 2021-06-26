# bsdutils-extra

Chimera uses https://github.com/dcantrell/bsdutils as its coreutils replacement,
but not all GNU tools are covered under that, and not all FreeBSD tools are made
portable.

Therefore, this project aims to provide permissive-licensed reimplementations of
various GNU/BSD tools that did not/could not make it into `bsdutils`.

Some of these are imlpemented as wrappers around existing utils (shell scripts)
while others are implemented from scratch in C. They are not guaranteed to cover
all of the features of their counterparts.

Currently includes equivalents of the following GNU tools:

- `basenc`
- `base32`
- `base64`
- `dir`
- `vdir`
- `hostid`
- `nproc`
- `b2sum`
- `md5sum`
- `sha1sum`
- `sha224sum`
- `sha256sum`
- `sha384sum`
- `sha512sum`

As well as the following BSD ones:

- `md5`
- `sha1`
- `sha224`
- `sha256`
- `sha384`
- `sha512`
- `rmd160`
