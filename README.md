<h1 align="center">Aditya</h1>

<h3 align="center">
ML Engineer & Researcher — RAG, LLMs, AI Security, Open Source
</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/befa1ca3-cff0-458f-8dc7-3ff7ce398498" width="750" alt="Aditya's GitHub Banner"/>
</p>

---

## About

I work on how modern AI systems retrieve information, reason over it, and fail under adversarial conditions. My main areas are retrieval-augmented generation, LLMs, AI security, model evaluation, and reproducible ML.

I learn mostly by contributing to real repositories: reading existing architecture, reproducing issues, writing and testing changes, and going through maintainer review. I like work that sits between research and engineering, where an investigation ends in something people can actually use.

---

## Open Source

### AOSSIE / OpenVerifiableLLM

*Verifiable AI, reproducibility, model verification, frontend*

OpenVerifiableLLM aims to make model provenance, evidence, and releases transparent and reproducible. I built an isolated React + TypeScript + Vite frontend for it, following the project's contributor specification.

**What it includes**

- **Evidence Explorer:** filter by phase, scope, kind, and verification result; fixture, pilot, and production evidence kept separate; immutable references and lineage navigation.
- **Evidence Detail:** full SHA-256 digest copying, parent/child relationships, historical and superseded reports, technical metadata.
- **Model Release Interface:** separate base and conversational releases, an explicit "Not released yet" state, and download/generation actions disabled until a valid release exists.
- **Verification Guide:** artifact identity, data reconstruction, sampled replay, full end-to-end replay, inference reproduction.
- **Inference Preview:** isolated mock adapter, clear fixture-mode labelling, model identity validation, no fake production inference.
- **Claim semantics:** `PASS`, `FAIL`, `NOT_RUN`, `UNAVAILABLE`, `UNSUPPORTED`, kept separate from loading and workflow states.
- **Runtime validation:** Zod schemas, rejection of malformed metadata, handling of missing evidence, and protection against empty checks reporting success.
- **Accessibility:** keyboard navigation, responsive layouts, WCAG-oriented testing, accessible status/error/copy states, 200% zoom support.

**Validation**

```text
TypeScript Typecheck      Passed
Vitest Tests              48 passed
Playwright Tests          27 passed
Production Build          Passed
Production Isolation      Passed
Accessibility Audit       0 violations
Clean npm install         0 vulnerabilities
```

The PR has 14 commits across 56 files with 6,066 additions. The frontend stays isolated from the project's training, verification, signing, and operational infrastructure.

> The goal was not just a UI, but a frontend that doesn't make claims the underlying evidence cannot support.

### Project-HAMi

*Kubernetes, NVIDIA GPU infrastructure, security, Go*

**Issue #3120.** In the NVIDIA device-plugin `Allocate()` path, cache-directory creation used the following calls with their errors ignored:

```text
os.RemoveAll(...)
os.MkdirAll(..., 0777)
os.Chmod(..., 0777)
```

This caused two problems:

1. **Unhandled filesystem errors.** A failed directory creation could be silently ignored, letting `Allocate()` continue toward a broken mount instead of returning a useful error.
2. **Excessive permissions.** A root-level device plugin creating a host-side directory with `0777` gives unprivileged processes unnecessary write access.

I documented the issue, tied it to an existing security pattern in the repository, proposed restricted permissions with explicit error handling, and drafted the fix. It was a good lesson in how security bugs in privileged infrastructure code differ from ordinary application bugs.

**Documentation investigation.** I also found conflicting Helm docs for `devicePlugin.nvidiaDriverRoot`, where duplicate entries listed different defaults. I traced it through earlier changes and found the newer `auto` configuration had superseded the old text. The maintainer later explained the docs had moved to the project's website repository.

> Not every issue you find should become a PR. Understanding repository ownership and maintainer direction is part of contributing well.

### What I've Learned

- Reading unfamiliar production codebases and tracing bugs through them
- Writing reproducible issue reports and spotting security implications
- Working within contributor specs and keeping changes scoped
- Writing meaningful automated tests, and checking accessibility and production builds
- Responding to maintainer feedback, and knowing when not to make a change
- Keeping development fixtures separate from production evidence

---

## Research Interests

- Retrieval-augmented generation
- Large language models
- LLM security, prompt injection, and jailbreak detection
- AI/ML evaluation
- Trustworthy and verifiable AI
- AI agents
- Information retrieval and embeddings
- Reproducible and adversarial ML

I'm most interested in making AI systems more reliable, measurable, secure, and reproducible.

### Currently Exploring

| Area | Topics |
|---|---|
| Machine Learning | Deep learning, transformers, representation learning, model evaluation |
| Retrieval and RAG | Embeddings, dense retrieval, reranking, RAG evaluation, retrieval benchmarks |
| AI Security | Prompt injection, jailbreak detection, adversarial prompts, LLM guardrails |
| Open Source | AI/ML, security, infrastructure, reproducibility, developer tools |

---

## Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,cpp,go,typescript,javascript,react,nodejs,express,fastapi,tailwind,mongodb,mysql,firebase,git,github,linux,docker" />
</p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=pytorch,tensorflow" />
</p>

| Category | Tools |
|---|---|
| AI / ML | Python, PyTorch, TensorFlow, Scikit-learn, XGBoost, Transformers |
| LLM | RAG, embeddings, LLM evaluation, AI agents, prompt security |
| Software | React, TypeScript, Node.js, FastAPI, Firebase, MongoDB |
| Infrastructure | Git, GitHub, Linux, Docker, REST APIs, CI/CD, testing |

---

## Projects

| Project | Focus |
|---|---|
| **OpenVerifiableLLM** | AI verification, evidence exploration, reproducibility, model release infrastructure |
| **AI-BOUNCER** | Adversarial prompt and jailbreak detection |
| **Sentara** | AI-based cyber-threat detection |
| **TrustProof / TrustLens** | Review verification and trust scoring |
| **InternScout** | Web scraping and virality intelligence |
| **Farmer Support System** | AI-enabled agricultural assistance |

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=adityasagarr123&show_icons=true&theme=tokyonight" alt="Aditya's GitHub stats" width="48%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=adityasagarr123&theme=tokyonight" alt="GitHub streak" width="48%" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=adityasagarr123&theme=tokyo-night" alt="GitHub activity graph"/>
</p>

---

## Contact

<p align="center">
  <a href="https://www.linkedin.com/in/aditya-sagar-1b35b2323/" target="_blank">
    <img src="https://skillicons.dev/icons?i=linkedin" width="45"/>
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="https://instagram.com/d4crush" target="_blank">
    <img src="https://skillicons.dev/icons?i=instagram" width="45"/>
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="mailto:adisagar450@gmail.com">
    <img src="https://skillicons.dev/icons?i=gmail" width="45"/>
  </a>
</p>

---

**Fun fact:** I can pick up musical rhythms within 3–4 tries, and sometimes learn them in my sleep.

<p align="center">
  <i>"Code. Research. Contribute. Repeat."</i>
</p>
