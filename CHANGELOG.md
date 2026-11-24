# Changelog

The **Frontier Models guide (FMg)** is a living technical publication. Its content evolves as knowledge advances, evidence improves, and explanations are refined. The website that publishes FMg also evolves independently.

This changelog documents meaningful changes to both **FMg** and the **Website**, helping readers understand what has changed between releases.

The format is adapted from [Keep a Changelog 1.1.0](https://keepachangelog.com/en/1.1.0/), with releases listed in reverse chronological order and change categories such as Added, Changed, Fixed, and Removed where appropriate.

## Versioning Policy

FMg uses a custom versioning system suited to a continuously evolving, multilingual technical book. Unlike software Semantic Versioning, its numbers describe the **editorial scope of changes**, not compatibility between software interfaces.

### FMg Versioning

FMg follows:

**`Major.Minor.Patch.Translation`**

The first three components identify the authoritative English edition. The fourth identifies a revision of a translation derived from that exact English edition.

| Component | Definition |
|---|---|
| **Major** | Changes to FMg's overall structure, such as adding or removing Parts or substantially reorganizing relationships across multiple chapters. |
| **Minor** | Changes at the chapter level, such as adding, removing, restructuring, or substantially rewriting a chapter. |
| **Patch** | Changes within existing chapter content, including corrections, clarifications, updated evidence, equations, examples, and references. |
| **Translation** | Independent revision number for each translated language, tied to an exact English edition. |

**Rules:**

- The English edition is the authoritative source and uses `Major.Minor.Patch`, without the Translation component.
- The highest applicable level of editorial change determines the English version increment. The number of modified chapters alone does not determine it.
- Incrementing Major resets Minor and Patch to zero; incrementing Minor resets Patch to zero.
- Each language maintains its own Translation sequence, beginning at `1` for each English edition.
- Translation-only improvements increment Translation without changing the English source version.
- Each translation must preserve the meaning of its identified English source edition.
- Changes to FMg do not automatically trigger a Website version change.

For example, the same English edition `7.7.7` might have a French translation `7.7.7.1` and a Vietnamese translation `7.7.7.3`. These numbers identify different translation revision histories, not different English content editions.

### Multilingual Edition Management

The Website supports **independent FMg versions for each language**. Each language can display its own published edition, including both its English source version and its Translation revision.

The editorial goal is to keep all available languages aligned with the latest authoritative English edition. However, temporary differences are permitted, for example while translating or reviewing a new edition.

For example:

| Language | Published version |
|---|---|
| English | `7.8.0` |
| French | `7.7.7.2` |
| Vietnamese | `7.8.0.1` |

In this example, French temporarily follows an earlier English edition, while Vietnamese follows the current one.

A translation always identifies its exact English source edition. Language switching does not imply that the available translations contain identical content when their source versions differ.

**Synchronization is the preferred publication state, not a technical requirement.**

### Website Versioning

The Website follows an **independent release sequence**, beginning with `1.0` for the first official public release.

Website versions describe meaningful changes to the reading and publication experience, including navigation, accessibility, search, language support, AI Reading integration, and installation capabilities.

- Website releases do not change FMg's editorial version.
- FMg editions and translation revisions do not automatically require a new Website version.
- Components such as the **AI Reading setup and prompt** maintain their own independent versions.
- Internal development milestones, implementation details, and routine maintenance are excluded unless they produce meaningful public-facing changes.

### Changelog Scope

The public changelog begins with the first official publication. Earlier private development iterations are not included. Each release is identified by its version number and publication date (YYYY-MM-DD).

The **FMg** section records editorial changes and translation releases. The **Website** section records changes to the publication and reading experience.

Both sections track significant published changes rather than every internal edit or development step.

---

## FMg

### [7.7.7] - 2026-11-17 - First Official Publication

#### Added

- First official public edition of the **Frontier Models guide (FMg)**.
- **7 Parts and 73 chapters** covering the foundations of frontier models and systems:
  1. Foundations
  2. The Mechanics of Neural Models
  3. Before Transformers
  4. The Transformer Revolution
  5. LLMs in Reality
  6. From LLM to Large Multimodal Foundation Model
  7. Frontier Models
- A first-principles approach connecting fundamental problems, causal mechanisms, mathematical relationships, and system-level understanding.
- Explanations of technical mechanisms, their assumptions, limitations, and relationships throughout FMg.
- Initial publication in **English, French, and Vietnamese**, with English as the authoritative edition.
- Support for independent reading and AI-assisted exploration.

---

## Website

### [1.1] - 2026-11-24
#### Changed
- Improve SEO 

### [1.0] - 2026-11-17 - First Official Publication

#### Added

- **AI Reading:** a dedicated setup experience and versioned reading companion prompt for exploring FMg with an AI assistant.
- **Multilingual publication:** full reading experience in English, French, and Vietnamese.
- **Independent language editions:** support for publishing and displaying different FMg versions for each language, while maintaining a common English source of truth.
- **Localized navigation:** dedicated homepages, menus, and FMg navigation for each language.
- **Language switching:** navigation between corresponding pages across available languages.
- **Local search:** built-in search across published website content.
- **Share:** share FMg chapters through native device sharing where supported, with a fallback to copying the page link.
- **Install App:** ability to install FMg as a standalone web app on supported browsers and devices, without offline reading support.
- **Responsive interface:** reading and navigation optimized for desktop and mobile devices.
- **Theme switching:** support for light and dark modes, with automatic adaptation to system preferences.