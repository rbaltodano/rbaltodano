### Welcome, my name is Ryan. 👋

Over the past few years I've noticed that technology is accentuating a crisis of meaning in many
people. The world is advancing faster than ever and so many people are unsure where they fit into
it. AI is a powerful tool to increase productivity, but as it advances some are afraid that they
might get optimized out of a job, streamlined out of their future. I wanted to be on the side of AI
that is not meant to replace our humanity but enhance it.

When I first saw that there were AI models small enough to run on mobile hardware, the technical
side of me was enamored by the possibilities. As I started to poke around I realized the potential
for leveraging AI in a way only a local model could: true privacy. How could I use this technology
in my larger goal of addressing the crisis of meaning? That's when I began to conceptualize this
project. This app is a space for you to explore some of life's biggest questions in a place that is
private, offline, and free forever. I have a moral responsibility to use all my skills and
abilities to achieve the highest possible good I can, and this project is one expression of that.

## Currently building: Aquinas

<a href="https://github.com/rbaltodano/Aquinas-iOS">
  <img src="https://raw.githubusercontent.com/rbaltodano/Aquinas-iOS/main/Documentation/Screenshots/insight-tree-church-doctrine-authority.jpg" alt="The Aquinas Insight Tree" width="220" align="right">
</a>

**[Aquinas](https://github.com/rbaltodano/Aquinas-iOS)** is an iOS study and conversation app for
serious questions in philosophy, theology, Scripture, and human flourishing. It runs a fine-tuned
language model on the phone, grounds answers in a bundled library of primary sources, and maps a
person's developing ideas as an **Insight Tree**: concepts are embedded as vectors, compared for
relatedness, and laid out spatially so you can see how ideas connect instead of scrolling a
linear chat.

| Repository | What it is |
| --- | --- |
| [**Aquinas-iOS**](https://github.com/rbaltodano/Aquinas-iOS) | SwiftUI app: on-device LiteRT inference, local retrieval, the Insight Tree, and a custom design system |
| [**Aquinas-Backend**](https://github.com/rbaltodano/Aquinas-Backend) | FastAPI + MLX development service: generation, retrieval evaluation, embeddings, and tree persistence |
| [**Aquinas-Foundations**](https://github.com/rbaltodano/Aquinas-Foundations) | Product, design, and architecture docs, plus model research such as quantization and fine-tuning studies |

<br clear="right">

## What I work with

- **Apple platforms:** Swift, SwiftUI, Xcode, on-device performance and memory tuning
- **On-device ML:** LiteRT-LM, MLX, LoRA fine-tuning, quantization (QAT, DWQ), model evaluation
- **Retrieval and semantics:** sentence embeddings (MiniLM), vector similarity, source-grounded RAG
- **Services:** Python, FastAPI, SQLite, structured-output contracts between client and model
