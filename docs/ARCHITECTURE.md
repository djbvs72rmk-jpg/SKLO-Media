# SKLO Media — Architecture

> Public architecture overview. Product-specific implementation details remain owned by each product.

## Core model

SKLO Media is a modular family of media products and capabilities.

The architecture intentionally avoids assuming a single mandatory:
- shared core;
- monorepo;
- central database;
- runtime;
- server;
- gateway;
- message bus;
- deployment topology.

A shared component exists only when it is explicitly designed, owned, versioned, and accepted as shared.

## Ownership

Each product keeps its own:
- purpose and scope;
- architecture;
- implementation decisions;
- release lineage;
- accepted baselines;
- runtime/deployment decisions;
- acceptance process.

Cross-product coordination belongs to the SKLO Media architecture layer, but product owners remain authoritative for their own product decisions.

## Integration direction

Preferred integration model:

```text
consumer need
→ explicit contract
→ narrow sufficient interface
→ independent ownership preserved
```

The default is to expose the smallest stable interface needed by the consumer.

## Stability principles

### Explicit contracts

Cross-product boundaries should be versioned and machine-readable where appropriate.

### Fail closed

Unknown or unsupported contract versions, invalid schemas, missing identities, or ambiguous state should not be silently accepted.

### Provenance

Results intended for downstream use should preserve enough identity and provenance to explain:
- what source was processed;
- which result was consumed;
- which contract version was used;
- which execution/component identity produced it.

### Internals are not APIs

Internal file layouts, temporary paths, private call graphs, native tool payloads, and implementation-specific artifacts do not become public interfaces merely because they exist.

### No implicit ownership transfer

Copying data, consuming results, or placing products in the same SKLO Media family does not transfer ownership.

## Repository policy

The public `SKLO-Media` repository is a documentation and coordination entry point.

It is not currently the canonical source repository for every SKLO Media product.

Product-specific repositories may remain independent and may be linked here when they are ready for public use.
