<h1 align="center">Hey, I'm Aditya.</h1>

<h3 align="center">
ML Engineer & Researcher · Full-Stack Developer · Open-Source Contributor
</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/befa1ca3-cff0-458f-8dc7-3ff7ce398498" width="750" alt="Aditya's GitHub Banner"/>
</p>

---

## About Me

I'm a Computer Science student and Full-Stack Developer with a growing focus on **Machine Learning, RAG, LLMs, AI security, and research**.

I like understanding systems from the inside — how they retrieve information, where they fail, how they can be attacked, and how we can make them more reliable.

My foundation is in full-stack engineering. I build applications end-to-end, but increasingly my work sits closer to the intersection of **machine learning, security, and systems engineering**.

I'm also actively contributing to open source, where I'm learning to work with unfamiliar codebases, investigate real problems, write production-oriented code, and collaborate with maintainers.

I don't want to just use intelligent systems.

**I want to understand them.**

---

## Tech Stack

### Development

<p>
  <img src="https://skillicons.dev/icons?i=html,css,javascript,typescript,react,tailwind,nodejs,express,fastapi,mongodb,mysql,firebase,git,github,linux,docker" />
</p>

### Machine Learning

<p>
  <img src="https://skillicons.dev/icons?i=python,pytorch,tensorflow" />
</p>

`Scikit-learn` · `XGBoost` · `Pandas` · `NumPy` · `Transformers`

### Areas I'm Exploring

`RAG` · `LLMs` · `Information Retrieval` · `Embeddings` · `AI Security` · `Adversarial ML` · `LLM Evaluation` · `AI Agents` · `Reproducible ML`

---

# Projects

### Sentara

An AI-based cyber-threat detection framework built around two ML pipelines:

- Network activity classification using NSL-KDD
- Malicious vs. benign executable classification using PE features
- DNN and Random Forest baselines
- FastAPI inference backend
- React frontend

**Stack:** Python · Machine Learning · FastAPI · React

[Live Demo](https://cyber-threat-detection-backend.vercel.app/) · [GitHub](https://github.com/AdityasagarR123/Sentra)

---

### AI-BOUNCER

A machine-learning pipeline for detecting adversarial prompts and jailbreak attempts against LLM applications.

The system uses a two-stage architecture:

**XGBoost** handles fast initial classification, while **DeBERTa-v3** evaluates uncertain or higher-risk prompts.

The project focuses on building practical defenses against adversarial inputs while keeping inference cost and latency in mind.

**Stack:** Python · XGBoost · DeBERTa · Transformers · PyTorch

---

### TrustProof / TrustLens

An AI-assisted review verification platform designed to distinguish trustworthy reviews from potentially manipulated or fabricated ones.

The system combines:

- Purchase and bill verification
- OTP validation
- Text authenticity analysis
- Media validation
- Experience consistency checks
- Trust scoring

**Stack:** React · TypeScript · Firebase · Gemini · AI Agents

---

### InternScout

A web intelligence platform built around automated data collection and analysis.

The project combines web scraping, API-based processing and a deployed frontend/backend system to discover and analyze online opportunities and signals.

**Stack:** React · Python · Web Scraping · APIs · Vercel · Render

[Live](https://interscout-webscrapper-fqcu.vercel.app/) · [API](https://interscout-webscrappervirality-intel-api.onrender.com/)

---

### Farmer Support System

A full-stack platform designed to provide farmers with accessible information and technology-driven assistance.

**Stack:** React · Node.js · MongoDB · AI/ML

---

# Open Source

Open source has become one of the most important parts of how I learn.

Personal projects let you control the environment.

Open source doesn't.

You have to understand code written by someone else, work within an existing architecture, respect project conventions, justify your changes, test them properly, and accept that maintainers may tell you that your solution isn't needed.

That process is what interests me.

## OpenVerifiableLLM — AOSSIE

**Focus:** AI verification · reproducibility · evidence · model releases

I was given a dedicated frontend contributor brief and built the public frontend around the project's evidence and verification architecture.

### What I worked on

- Evidence Explorer with filtering across phase, scope, kind and result
- Evidence detail and parent/child lineage
- SHA-256 digest handling
- Historical and superseded evidence
- Base and conversational model release interfaces
- Verification profiles and result semantics
- Isolated mock inference adapter
- Runtime schema validation with Zod
- Responsive frontend architecture
- Accessibility testing
- Unit and browser testing
- Production build and isolation checks

The current PR contains:

**14 commits · 56 files · 6,066 additions**

Validation:

```text
TypeScript typecheck       Passed
48 Vitest tests            Passed
27 Playwright tests        Passed
Production build           Passed
Production isolation       Passed
Accessibility audit        0 violations
Clean dependency install   0 vulnerabilities
```

### Contribution

**[PR #178 — feat(frontend): add static evidence explorer and model release interface](https://github.com/AOSSIE-Org/OpenVerifiableLLM/pull/178)**

The interesting part of this contribution wasn't simply building the interface.

The project required the frontend to distinguish between **what has actually been verified, what has merely been reported, and what is still unavailable**.

That meant designing the UI around evidence rather than assumptions.

---

## Project-HAMi

**Focus:** Kubernetes · NVIDIA GPU infrastructure · Security · Go

My work on HAMi began with a security-oriented investigation of the NVIDIA device-plugin implementation.

I identified an issue in the `Allocate()` path involving:

```go
os.RemoveAll(...)
os.MkdirAll(..., 0777)
os.Chmod(..., 0777)
```

The filesystem errors were being ignored, while the host-side cache directory was being created with world-writable permissions.

I documented the potential reliability and security implications, traced the issue against an existing security pattern in the repository, proposed explicit error handling and restricted permissions, and drafted the corresponding implementation.

### Contributions

**[Issue #3120 — insecure 0777 permissions and unhandled directory creation errors](https://github.com/Project-HAMi/HAMi/issues/3120)**

**[Issue #3122 — restrict permissions and handle errors for cache directory](https://github.com/Project-HAMi/HAMi/issues/3122)**

I also investigated a conflicting Helm documentation entry:

**[Issue #3111 — duplicate/conflicting `devicePlugin.nvidiaDriverRoot`](https://github.com/Project-HAMi/HAMi/issues/3111)**

The documentation was ultimately maintained in another repository, which was another useful lesson: **contribution is also knowing when not to change something.**

---

## What Open Source Is Teaching Me

Open source has changed how I approach engineering.

I'm learning to:

- Read unfamiliar systems before changing them
- Investigate instead of assuming
- Write issues that others can reproduce
- Make changes that respect existing architecture
- Treat security as part of engineering, not an afterthought
- Test what I build
- Separate evidence from claims
- Accept review and criticism
- Understand the reasoning behind maintainers' decisions

I'm still early in this journey.

But I'm no longer learning only by building things from scratch.

I'm learning by **entering systems that already exist and trying to make them better.**

---

# GitHub

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=adityasagarr123&show_icons=true&theme=tokyonight" width="48%" alt="Aditya's GitHub Stats"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=adityasagarr123&theme=tokyonight" width="48%" alt="Aditya's GitHub Streak"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=adityasagarr123&theme=tokyo-night" alt="GitHub Activity Graph"/>
</p>

---

# Beyond Code

I spend a lot of my time in front of a screen.

So when I get away from it, I usually go as far away as possible.

I'm drawn to **mountains and high-altitude climbing**.

I've spent time trekking through the Himalayas, and I want to keep pushing toward higher and harder routes.

There's something about being above the clouds, carrying everything you need on your back, and having no shortcut to the summit that I find difficult to replace.

**Build quietly. Go farther.**

---

## Connect

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

<p align="center">
  <i>“The journey matters more than the destination.”</i>
</p>
