<!-- tyhp-readme:start -->
# tyhpdef/laravel-prompts

Tyhp type definitions for `laravel/prompts` `0.3.24`.

```bash
composer require --dev tyhpdef/laravel-prompts:0.3.24
```

This is a metapackage. Composer also installs `tyhpdef/laravel-prompts-impl` (type files).
Require **this** name, not `tyhpdef/laravel-prompts-impl`.

See https://tyhplang.com.

## Maintain `laravel/prompts`? Ship the types yourself

If you are a Packagist maintainer of `laravel/prompts`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/laravel-prompts-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `laravel/prompts` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/laravel-prompts": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `laravel/prompts` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `laravel/prompts` with a real constraint,
   `"replace": { "tyhpdef/laravel-prompts": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `laravel/prompts` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/laravel-prompts` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
