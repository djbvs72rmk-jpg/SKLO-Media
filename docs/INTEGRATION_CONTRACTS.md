# SKLO Media — Integration Contracts

> Public contract policy. This document defines how SKLO Media products should integrate at a high level. It does not publish private schemas or internal implementation artifacts.

## Contract principles

A cross-product interface should be:

- explicitly owned;
- versioned;
- narrow enough for the consumer need;
- independently understandable;
- validated before consumption;
- fail-closed for unknown required semantics;
- provenance-preserving;
- independent from internal filesystem or runtime layout.

## Consumer rule

A consumer should depend on the public contract, not on producer internals.

Examples of things that should not become accidental APIs:

- private function names;
- internal call paths;
- temporary files;
- cache/checkpoint layout;
- native third-party tool JSON;
- current ZIP/TAR packaging structure;
- model file paths;
- runtime installation directories;
- implementation-specific chunking details.

## Identity and provenance

Where applicable, a consumer-facing result should carry or bind to:

- contract identity and version;
- source identity;
- result identity;
- execution/component identity;
- artifact identity;
- completion/finality state;
- warnings, degraded state, or stop/gate semantics when relevant.

A filename or path hint should not be the sole identity for an important result.

## Compatibility

Compatibility should be explicit.

Preferred rule:

```text
known contract
+ supported version
+ schema validation
+ required semantic checks
→ compatible
```

Unknown required versions or semantics should fail closed.

Generic forward compatibility such as “accept anything newer” is discouraged unless specifically designed and tested.

## Current product relationships

### MediaAudit

MediaAudit is an independent producer. Downstream consumers use only owner-approved external consumer contracts.

Producer internals are not public APIs.

### SKLO FmediaDB

FmediaDB provides product/schema-level contracts and does not automatically become the central database for every consumer.

Consumers should prefer the narrowest sufficient access model.

### SKLO Scenario Matching

Scenario Matching owns semantic matching logic and result semantics.

It does not own transcript generation, MediaAudit internals, or MediaOrder orchestration.

### SKLO Transcript & Subtitles

Transcript/Subtitles owns transcript/timed-text outputs and the contracts for that layer.

It does not own scenario matching or application orchestration.

### SKLO Atlas

Atlas may consume external capabilities where appropriate, but it is not a mandatory gateway for the SKLO Media family.

Its internal `SKLO FileWorker` capability is not currently a shared external service.

## Public contract publication

When a contract becomes ready for public use, it should be published with:
- owner;
- contract name/version;
- stability status;
- schema or normative field definition;
- compatibility policy;
- examples;
- change policy.

Until then, implementation artifacts should not be treated as public contracts.
