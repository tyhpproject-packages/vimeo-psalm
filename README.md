<!-- tyhp-readme:start -->
# tyhpdef/vimeo-psalm

Tyhp type definitions for `vimeo/psalm` `7.0.0-beta22`.

```bash
composer require --dev tyhpdef/vimeo-psalm:7.0.0-beta22
```

This is a metapackage. Composer also installs `tyhpdef/vimeo-psalm-impl` (type files).
Require **this** name, not `tyhpdef/vimeo-psalm-impl`.

See https://tyhplang.com.

## Maintain `vimeo/psalm`? Ship the types yourself

If you are a Packagist maintainer of `vimeo/psalm`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/vimeo-psalm-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `vimeo/psalm` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/vimeo-psalm": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `vimeo/psalm` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `vimeo/psalm` with a real constraint,
   `"replace": { "tyhpdef/vimeo-psalm": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `vimeo/psalm` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/vimeo-psalm` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
