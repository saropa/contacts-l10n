# Saropa Contacts — Translation CDN

Public mirror of translation ARB files for the
[Saropa Contacts](https://github.com/saropa/contacts) app.

The app APK ships with English only. All other languages are fetched
on demand from this repo via `raw.githubusercontent.com` and cached
on device.

## Layout

```
assets/l10n/app_<locale>.arb
```

## URL pattern

```
https://raw.githubusercontent.com/saropa/contacts-l10n/main/assets/l10n/app_<locale>.arb
```

## Source of truth

This repo is generated from the private `saropa/contacts` repo via
`scripts/build/setup_arb_translate.py`. Do not edit files here
directly — they are overwritten by the translation pipeline.

## Why a separate repo

`saropa/contacts` is private. GitHub's raw content CDN requires
public visibility for unauthenticated fetches. This repo exposes
only the ARB files, not the source.
