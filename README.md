# Ryan Baltodano

Applied AI engineer and product designer building local-first tools for study and research: **[Angrove](https://github.com/rbaltodano/Angrove-iOS)**, a private on-device AI study app for iPhone and Mac, and **[inVectus](https://github.com/rbaltodano/inVectus)**, a desktop workspace for exploring document collections and investigating potential coverage gaps.

**[Read the case study](https://angrove.app/case-study.html)** · [Try the iPhone beta on TestFlight](https://testflight.apple.com/join/qHDFeAUa) · [Watch the 1:49 demo](https://angrove.app/case-study.html#demo-conversation) · [Résumé (PDF)](https://angrove.app/assets/Ryan-Baltodano-Resume.pdf)

**Explore the projects:** [Angrove](#angrove) · [inVectus](#invectus) · [All repositories](#repositories)

## Angrove

<a href="https://github.com/rbaltodano/Angrove-iOS">
  <img src="https://raw.githubusercontent.com/rbaltodano/Angrove-iOS/main/Documentation/Screenshots/case-study-2026-10-05/insight-map.jpg" alt="Angrove's Insight Tree: a semantic map of saved ideas" width="220" align="right">
</a>

Angrove answers questions about philosophy, theology, and history from a curated library of primary sources, cites them, and says so when a source is missing instead of inventing a quotation. Generation, retrieval, and the Insight Tree (a semantic map of saved ideas) all run on-device; there is no model server and no account.

- On-device Gemma 4 E4B through LiteRT-LM, with Core ML MiniLM embeddings retrieving from 51,836 passages across 37 bundled works
- SwiftUI iPhone app and a native Mac app sharing one codebase, with a Figma-based design system
- AES-256-GCM encrypted local storage with Keychain-protected keys
- Evaluation-driven decisions: in an 80-case comparison, native model thinking gave the same pass rate (74/80) at roughly double the latency, so it ships off by default
- iPhone public beta on TestFlight, App Store release next; Mac app in progress

<br clear="right">

### See the app

October 22, 2026 captures from the iPhone app and native Mac app in development.

[![Angrove Mac Board](https://raw.githubusercontent.com/rbaltodano/Angrove-iOS/main/Documentation/Screenshots/2026-10-22/mac-boards-1.png)](https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Screenshots/2026-10-22/README.md)

<p align="center">
  <a href="https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Screenshots/2026-10-22/ios-homescreen.png"><img src="https://raw.githubusercontent.com/rbaltodano/Angrove-iOS/main/Documentation/Screenshots/2026-10-22/ios-homescreen.png" alt="Angrove Home on iPhone" width="23%"></a>
  <a href="https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Screenshots/2026-10-22/ios-library.png"><img src="https://raw.githubusercontent.com/rbaltodano/Angrove-iOS/main/Documentation/Screenshots/2026-10-22/ios-library.png" alt="Angrove Library on iPhone" width="23%"></a>
  <a href="https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Screenshots/2026-10-22/ios-sidebar.png"><img src="https://raw.githubusercontent.com/rbaltodano/Angrove-iOS/main/Documentation/Screenshots/2026-10-22/ios-sidebar.png" alt="Angrove side menu on iPhone" width="23%"></a>
  <a href="https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Screenshots/2026-10-22/ios-study-topics.png"><img src="https://raw.githubusercontent.com/rbaltodano/Angrove-iOS/main/Documentation/Screenshots/2026-10-22/ios-study-topics.png" alt="Angrove Study Topic on iPhone" width="23%"></a>
</p>

[Watch: Lay your ideas out](https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Screenshots/2026-10-22/lay-your-ideas-out.mp4) · [Watch: Learn easier](https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Screenshots/2026-10-22/learn-easier.mp4) · [All screenshots and recordings](https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Screenshots/2026-10-22/README.md)

## inVectus

**[View the repository](https://github.com/rbaltodano/inVectus)** · [Reproducible demo](https://github.com/rbaltodano/inVectus/blob/main/docs/demo.md) · [Architecture and tradeoffs](https://github.com/rbaltodano/inVectus/blob/main/docs/architecture.md)

A local-first desktop research tool for mapping document collections, searching by meaning, and inspecting areas with limited coverage. It brings the collection map, ranked gap candidates, supporting evidence, and saved research decisions into one workspace.

[![inVectus: ranked gap candidates beside an interactive map of a 5,000-paper ophthalmology collection](https://raw.githubusercontent.com/rbaltodano/inVectus/main/docs/screenshots/ophthalmology-gap.png)](https://github.com/rbaltodano/inVectus)

- **Shared Rust engine:** a Tauri 2 desktop app with React/TypeScript and a CLI built on the same workspace
- **Local data and inference:** DuckDB for metadata, LanceDB for vectors, ONNX Runtime for embeddings, and optional llama.cpp descriptions
- **Inspectable search and scores:** semantic search, collection-level gap assessments, supporting items, and score breakdowns
- **Durable research workflows:** resumable embedding jobs, cancellation, saved gaps, notes, and a persistent decision log

**Working prototype, tested locally on Apple Silicon macOS.** Windows and Linux remain unverified. Gap candidates indicate limited coverage within the imported collection; they are not validated discoveries. The repo includes a reproducible fictional demo.

## Repositories

Direct links to every public repository. Start with Angrove-iOS or inVectus to review the application code.

| Repository | What it is |
| --- | --- |
| [inVectus](https://github.com/rbaltodano/inVectus) | Desktop research workspace and CLI: Rust, Tauri, React/TypeScript, local embeddings, and collection analysis |
| [Angrove-iOS](https://github.com/rbaltodano/Angrove-iOS) | The iPhone and Mac apps: on-device runtime, retrieval, encrypted persistence, and the Insight Tree |
| [Angrove-Foundations](https://github.com/rbaltodano/Angrove-Foundations) | Product, design, and model-integration documentation, plus case studies |
| [Angrove-Backend](https://github.com/rbaltodano/Angrove-Backend) | Offline Python tooling: corpus preparation, model conversion, and evaluation |
| [angrove-website](https://github.com/rbaltodano/angrove-website) | Angrove's product site, User Guide, demos, case studies, and development notes |
| [ryanbaltodano.com](https://github.com/rbaltodano/ryanbaltodano.com) | Personal portfolio website: static HTML, CSS, and JavaScript |
| [rbaltodano](https://github.com/rbaltodano/rbaltodano) | This GitHub profile README and project index |

[Browse all repositories](https://github.com/rbaltodano?tab=repositories)

## Read more

- [Case studies: architecture, evaluation, and engineering decisions](https://angrove.app/case-study.html)
- [Technical case study](https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Case-Study.md) and [evaluation methodology](https://github.com/rbaltodano/Angrove-iOS/blob/main/Documentation/Evaluation.md)
- [Development notes](https://angrove.app/blog/): dated experiments with methods and limitations

## What I work with

- **Apple platforms:** Swift, SwiftUI, Swift Testing, Xcode, App Store and TestFlight delivery
- **On-device ML:** LiteRT-LM, Core ML, MLX, quantization, model evaluation
- **Retrieval:** sentence embeddings, vector similarity, source-grounded generation
- **Desktop and systems:** Rust, Tauri, React, TypeScript, DuckDB, LanceDB, ONNX Runtime
- **Tooling:** Python, GitHub Actions, Figma

Tampa, FL · Open to applied AI and iOS engineering roles

