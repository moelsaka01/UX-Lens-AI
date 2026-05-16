# UXLens AI

Production-style AI visual intelligence platform for website analysis, UX scoring, redesign reasoning, visual overlays, and AI-assisted redesign previews.

UXLens AI analyzes real websites, captures desktop and mobile screenshots, extracts layout and UX signals, scores user experience quality, identifies friction patterns, generates redesign recommendations, and produces visual redesign previews through a local-first AI pipeline.

The project is designed as a real AI product system, not a notebook demo.

---

# Overview

UXLens AI is a full-stack AI system focused on visual intelligence and UX analysis.

The platform combines:

- browser automation
- screenshot intelligence
- UX scoring
- redesign reasoning
- overlay visualization
- observability
- ranking systems
- learning infrastructure
- deterministic rendering
- async orchestration

into a production-style AI engineering system.

Unlike simple UI mockup generators or isolated notebook projects, UXLens AI is structured like a deployable AI SaaS backend with real frontend integration, observability, evaluation, and extensibility layers.

---

# What It Does

UXLens AI helps answer:

- How strong is this website's UX?
- Where is the page losing attention or clarity?
- Is the CTA visually dominant enough?
- Is the first screen overloaded?
- What redesign direction would improve conversion clarity?
- How does the page compare against another website?
- Can feedback improve future ranking decisions?
- How would a redesigned version visually look?

---

# Core Features

## Website Intelligence Pipeline

- Live URL analysis
- Desktop and mobile screenshot capture
- Above-the-fold rendering
- Full-page rendering
- UX signal extraction
- Navigation analysis
- CTA hierarchy analysis
- Hero section analysis
- Layout density analysis
- Readability analysis
- Visual structure analysis
- Design pattern classification
- Benchmark-style layout similarity

---

## UX Scoring Engine

UXLens AI produces structured scores for:

- Overall UX
- Attention focus
- CTA visibility
- Readability
- Cognitive load

The scoring system is based on:
- structural signals
- visual hierarchy
- first-screen density
- CTA dominance
- navigation complexity
- hero clarity
- scan friction

---

## AI Redesign Reasoning

The platform generates redesign recommendations based on:

- extracted visual signals
- UX scoring
- layout density
- hero structure
- CTA hierarchy
- navigation complexity
- benchmark similarity
- evaluation confidence
- historical feedback

Suggestions include:
- rationale
- evidence
- redesign direction
- expected outcomes
- ranking confidence

---

## Visual Overlay System

UXLens AI creates structural overlay previews on top of real screenshots to visualize:

- navigation simplification
- hero focus improvements
- CTA emphasis
- density reduction
- attention guidance
- layout cleanup

The overlay engine highlights likely redesign improvements directly on captured screenshots.

---

## Redesign Preview Renderer

The system includes a deterministic redesign preview renderer designed for:

- local reliability
- quota-free demos
- async generation
- stable output
- fast generation
- CPU-safe execution

Renderer mode avoids dependence on:
- paid APIs
- external GPU quotas
- unstable image generation pipelines

Optional external AI image providers are supported separately.

---

## AI Image Generation (Optional)

UXLens AI also supports optional external AI image providers for redesign visualization.

Provider architecture is extensible and separated from the core renderer system.

Current experimental integrations:
- Replicate / FLUX
- Gemini image generation

These are intentionally optional and not required for the main demo pipeline.

---

## Compare Mode

Compare mode analyzes two websites simultaneously and evaluates:

- UX differences
- CTA hierarchy differences
- readability differences
- attention focus differences
- cognitive load differences

The system then generates:
- winner selection
- reasoning
- comparison insights
- score deltas

---

## Feedback and Learning System

UXLens AI includes a local learning pipeline supporting:

- helpful / not useful signals
- accepted / rejected redesigns
- ranking weight updates
- feedback persistence
- learning diagnostics
- recommendation adaptation

The system includes infrastructure for:
- ranking feedback ingestion
- future online learning
- ML retraining hooks
- production simulation workflows

---

## ML Ranking Infrastructure

The project includes:
- ranking diagnostics
- weight systems
- ML ranker hooks
- retraining endpoints
- rollback support
- production simulation endpoints

Designed to emulate real AI platform infrastructure patterns.

---

## Observability and Diagnostics

UXLens AI exposes:
- pipeline timing
- evaluation diagnostics
- architecture readiness
- ranking diagnostics
- redesign transformation data
- feedback summaries
- mockup generation states
- ML ranker state

The system tracks:
- screenshot timing
- scoring timing
- retrieval timing
- evaluation timing
- redesign timing
- total analysis timing

---

# Architecture

UXLens AI is designed as a local-first full-stack AI system.

```text
Frontend
  React + Vite dashboard
  Analysis views
  Redesign preview system
  Feedback controls
  Observability panels
  Compare mode UI

Backend
  FastAPI API layer
  Async orchestration
  Playwright screenshot engine
  UX scoring engine
  Visual analysis system
  Redesign reasoning engine
  Overlay generation
  Ranking service
  Feedback service
  Learning infrastructure
  ML ranker hooks
  Static asset serving

AI / ML Layer
  CLIP-style layout similarity
  Embedding-based benchmark retrieval
  Rule-based scoring
  Feedback-aware ranking
  Deterministic renderer
  Optional external AI image providers

Storage
  SQLite persistence
  Generated screenshots
  Generated overlays
  Generated mockups
  Feedback events
  Observability records
  A/B scoring data

Tech Stack
Backend
Python
FastAPI
Playwright
Pillow
Pydantic
SQLite
ChromaDB
Transformers
Scikit-learn
Docker
Frontend
React
Vite
JavaScript
CSS modules
Custom dashboard UI system
Lucide React
AI / ML
CLIP-style visual similarity
Embedding retrieval
Heuristic UX scoring
Ranking systems
Local ML infrastructure
Feedback-aware ranking
Optional external image providers
Screenshots

Add screenshots here.

![Dashboard](docs/screenshots/dashboard.png)

![Analysis Results](docs/screenshots/analysis-results.png)

![Redesign Preview](docs/screenshots/redesign-preview.png)

![Overlay Preview](docs/screenshots/overlay-preview.png)

![Observability](docs/screenshots/observability.png)
Local Setup
1. Clone the repository
git clone https://github.com/moelsaka01/uxlens-ai.git

cd uxlens-ai
2. Create environment file
cp .env.example .env

The default demo path uses the deterministic local renderer.

External AI image generation is optional.

3. Start with Docker
docker compose up --build

Frontend:

http://localhost:5173

Backend:

http://localhost:8000
Environment Variables

Example:

FRONTEND_ORIGIN=http://localhost:5173

ENABLE_MOCKUP_GENERATION=true
ENABLE_ASYNC_MOCKUPS=true
ENABLE_CPU_MOCKUPS=false

MOCKUP_HEIGHT=900
MOCKUP_WIDTH=1280
MOCKUP_COUNT=1

IMAGE_PROVIDER=renderer

REPLICATE_API_TOKEN=
REPLICATE_MODEL=black-forest-labs/flux-schnell
Demo Flow
Enter a public website URL
Run analysis
Review UX scores
Inspect findings
Review redesign suggestions
View overlay preview
Render redesign preview
Compare before/after structure
Submit feedback
Inspect observability and learning panels
Why This Project Matters

UXLens AI demonstrates production-style AI engineering across multiple layers:

AI backend architecture
async orchestration
screenshot intelligence
UX analysis
ranking systems
evaluation infrastructure
observability
learning pipelines
frontend AI product integration
local-first reliability
visual AI systems

The project is intentionally designed to resemble a real AI product platform rather than a simple portfolio demo.

Current Status

Demo-ready local version.

The deterministic renderer path is stable and reliable for demonstrations.

External AI image generation exists as an optional experimental provider system.

Roadmap
Cloud deployment
Auth/workspaces
Team collaboration
PDF report export
Advanced redesign ranking
Stronger image generation abstraction
Longitudinal UX tracking
Browser extension integration
Experiment tracking
Agentic redesign workflows
Author

Mohamed Elsaka

AI Systems / GenAI Engineer focused on:

production AI systems
AI backend architecture
evaluation pipelines
observability
multimodal systems
full-stack AI products

LinkedIn:
https://linkedin.com/in/moelsaka

GitHub:
https://github.com/moelsaka01
