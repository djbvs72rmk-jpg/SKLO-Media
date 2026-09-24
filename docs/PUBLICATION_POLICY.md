# SKLO Media — Public Documentation Policy

This repository is public.

## Publish only material that is safe for public use

Do not publish:
- secrets, credentials, tokens, private keys, or access details;
- unnecessary personal or family data;
- private media;
- private filesystem paths or host-specific scratch paths;
- internal-only acceptance evidence unless explicitly approved for publication;
- implementation artifacts that would accidentally become a public API;
- claims that a planned or proposed capability is already released.

## Product ownership

Each product owner is responsible for the public accuracy of that product's page.

The central SKLO Media documentation may coordinate:
- family-level terminology;
- product map;
- cross-product boundaries;
- integration rules;
- links.

It should not silently replace product-owner decisions about:
- product status;
- releases;
- runtime;
- roadmap;
- public contracts;
- repository ownership.

## Status language

Prefer explicit status labels where useful, for example:

- PROPOSED
- ACTIVE
- EXPERIMENTAL
- ACCEPTED
- RELEASED
- DEPRECATED
- NOT YET PUBLIC
- OWNER CONTENT PENDING

Do not present a proposal as a release.

## Contracts

A public contract should be published only when its owner is prepared to maintain:
- contract identity and version;
- normative field semantics or schema;
- compatibility policy;
- change policy;
- examples where appropriate.

Internal implementation files are not public contracts by default.

## Product pages

Product pages under `docs/products/` are intentionally owner-maintained.

A placeholder page means the page location exists; it does not mean all product information is public or frozen.

## Licensing

Except where otherwise stated, documentation and other non-code content in this repository are licensed under **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

The governing repository notice is [LICENSE-DOCS.md](../LICENSE-DOCS.md).

This documentation license does not automatically apply to:
- source code in product-specific repositories;
- binaries, models, datasets, media assets, or third-party materials;
- trademarks, logos, or brand identifiers;
- material with its own explicit license or copyright notice.

Each product owner is responsible for selecting and publishing the license, if any, for that product's code and other product-specific artifacts.

Do not infer a software license from the SKLO Media documentation license.
