# SKLO Media — Product Map

> Public overview. This document describes product boundaries at a high level and is not a substitute for product-specific source code, release notes, or internal acceptance records.

SKLO Media is a modular media direction under the SKLO brand. Its products and capabilities may work together, but they are not assumed to share one codebase, one database, one runtime, or one release line.

## Products and capabilities

### SKLO Atlas

A media/file organization product focused on controlled media identity, naming, structure, and safe file operations.

Current architectural rule:
- Atlas remains one product;
- internal capabilities may mature inside Atlas before any future extraction;
- `SKLO FileWorker` is currently an internal working capability name, not a separate product or repository.

### MediaAudit

An independent media-analysis product with its own release lineage, runtime, roadmap, contracts, and acceptance.

Other SKLO Media products may consume MediaAudit results only through owner-approved external consumer contracts.

### MediaOrder / МедіаПорядок

A local media workflow/application for creator-oriented project work.

Its role includes project context, orchestration, user-facing workflow, and consumption of independent media capabilities through explicit boundaries.

### SKLO FmediaDB

An independent data/schema product for media-domain structure, identity, validation, migration, and compatibility contracts.

FmediaDB is not a mandatory central database for every SKLO Media product.

### SKLO Scenario Matching

A separate semantic capability for matching media/take evidence to scenario sections, including confidence and uncertainty semantics.

It is developed independently from transcript generation and from MediaOrder orchestration.

### SKLO Transcript & Subtitles

A separate capability covering:
- structured transcript;
- raw ASR as transcript output;
- timed transcript / timed segments;
- SRT / VTT;
- source-media timeline timecodes;
- provenance;
- versioned machine-readable contracts for this layer.

The public product name and technical slug may still evolve.

### SKLO Image Analysis

A developing image-analysis capability.

### SKLO Photo Enhancement

A developing photo-enhancement capability.

## Boundary rule

A product may consume another SKLO Media capability without becoming its owner.

Integration does not imply:
- repository merge;
- database merge;
- release-line merge;
- shared runtime;
- mandatory gateway;
- ownership transfer.

See also:
- [Architecture](ARCHITECTURE.md)
- [Integration Contracts](INTEGRATION_CONTRACTS.md)
