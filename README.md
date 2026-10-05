<!-- tyhp-readme:start -->
# tyhpdef/psr-http-client

Tyhp type definitions for `psr/http-client` `1.0.3`.

```bash
composer require --dev tyhpdef/psr-http-client:1.0.3
```

This is a metapackage. Composer also installs `tyhpdef/psr-http-client-impl` (type files).
Require **this** name, not `tyhpdef/psr-http-client-impl`.

See https://tyhplang.com.

## Maintain `psr/http-client`? Ship the types yourself

If you are a Packagist maintainer of `psr/http-client`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/psr-http-client-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `psr/http-client` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/psr-http-client": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `psr/http-client` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `psr/http-client` with a real constraint,
   `"replace": { "tyhpdef/psr-http-client": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `psr/http-client` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/psr-http-client` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
