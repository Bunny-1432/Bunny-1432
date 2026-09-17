# Bunny Yadav — Intelligent Systems Portfolio
## Product Requirements Document (PRD)

**Status:** Draft for design and implementation  
**Owner:** Bunny Yadav  
**Primary references:** [GitHub](https://github.com/Bunny-1432) · [LinkedIn](https://www.linkedin.com/in/bunny-yadav-1a86b32a1/)  
**Last updated:** 2026-09-17

> This PRD defines the product, content, design direction, and technical requirements for a premium portfolio. It is intentionally grounded in publicly visible GitHub material; LinkedIn-specific employment and education details should be verified by Bunny before publication.

---

## 1. Product vision

Build a portfolio that presents Bunny Yadav as an **AI/ML engineer and full-stack builder who turns complex, multimodal data into usable intelligent systems**.

The site should feel less like a resume and more like an **instrument panel for understanding intelligence**: precise, calm, dimensional, and evidence-led. The visual language should make systems, signals, and model decisions tangible without turning the page into a generic “futuristic AI” showcase.

### Positioning statement

> I build intelligent products across healthcare, finance, audio, and the web—from model experiments to clear, deployable interfaces.

This statement is a working draft. Replace it with Bunny’s preferred wording before launch.

### Product promise

Within the first minute, a visitor should understand:

1. Bunny’s role and professional direction.
2. The problem spaces he explores: healthcare AI, financial ML, audio intelligence, and full-stack delivery.
3. The difference between a notebook experiment and a complete product system.
4. Which projects deserve deeper inspection.
5. How to contact or connect with him.

---

## 2. Audience and user needs

### Primary audiences

- **Hiring managers and recruiters:** need fast evidence of capability, clarity of role, and contact details.
- **Engineering leads:** need architecture, deployment, APIs, model evaluation, and technical trade-offs.
- **Product/design leaders:** need to see how technical work becomes understandable and usable.
- **Potential collaborators:** need shared interests and an easy path to start a conversation.
- **Learners and open-source visitors:** need readable project explanations and links to source code.

### Core user tasks

- Identify who Bunny is and what he builds.
- Browse selected projects by problem domain.
- Understand one project deeply through context, process, technical execution, and outcome.
- Verify claims through GitHub, demos, metrics, and implementation details.
- Contact Bunny without a form-heavy workflow.

### Non-goals

- Listing every repository on the home page.
- Making 3D complexity the primary proof of skill.
- Presenting unverified employment, education, client, or performance claims.
- Replacing project evidence with generic personality copy.
- Building a dashboard of vanity GitHub statistics.

---

## 3. Product principles

1. **Evidence over adjectives.** Show the model, interface, metric, architecture, or decision that supports each claim.
2. **Systems, not spectacle.** Motion and 3D should explain relationships between input, inference, and output.
3. **One world, varied compositions.** Projects can have distinct layouts, but all use the same underlying visual grammar.
4. **Readable under pressure.** A recruiter scanning on a phone must get the point without waiting for effects.
5. **Progressive enhancement.** Semantic content is the baseline; motion and WebGL are optional layers.
6. **Specific human voice.** Prefer concrete observations and lessons over “passionate,” “innovative,” or “cutting-edge.”
7. **Curated restraint.** Feature four strong projects first; move the rest into an archive or GitHub index.

---

## 4. Creative direction

### Concept: **Signal / System / Human**

The portfolio is an editorial observatory for intelligent systems. A visitor moves from raw signal, to model interpretation, to human-facing product. The experience is not a cyberpunk command center; it is a controlled laboratory with warmth and editorial judgment.

### Visual metaphor

A **signal field**: thin paths, measured nodes, waveform traces, and layered planes respond to focus. The metaphor supports Bunny’s work across images, audio, health data, financial features, and interfaces while remaining abstract enough to avoid medical or financial cliché.

### Art direction

- Dark graphite foundation with warm paper-like surfaces for reading sections.
- A restrained signal color used only for active states, model outputs, and key metrics.
- Editorial typography with compact technical metadata.
- Diagrams and data traces treated as composition, not decoration.
- Material contrast: matte surfaces for content, translucent depth only in the hero system.
- No generic floating blobs, purple-blue gradients, excessive glass, or always-on particle fields.

### Typography

Use one expressive grotesk or neo-humanist sans for display and UI, paired with a restrained monospace for metadata and technical labels.

- **Display:** strong, slightly condensed, responsive; used for positioning and project titles.
- **Text:** high x-height, comfortable reading width, 16–19px body size.
- **Technical:** monospace for years, stack labels, metrics, and system annotations.
- Avoid oversized type that prevents the work from becoming the focal point.

### Color tokens

```css
:root {
  --ink-950: #111312;
  --ink-800: #242824;
  --paper-050: #f2f0e9;
  --paper-100: #e4e1d7;
  --signal-lime: #c8ed5f;
  --signal-coral: #e8896b;
  --signal-blue: #88b9d8;
  --line-dark: rgba(242, 240, 233, .18);
  --line-light: rgba(17, 19, 18, .16);
}
```

Use lime for interaction and status, coral for tension/risk, and blue for signal/data—not as decorative gradients.

### Motion language

- **Idle:** near-still; the signal field has a slow, low-amplitude drift.
- **Focus:** nodes connect, labels clarify, and lighting shifts subtly toward the selected project.
- **Transition:** depth and displacement before opacity; 450–800ms for major transitions.
- **Feedback:** immediate 120–180ms response for hover, focus, and button states.
- **Reduced motion:** remove camera movement, looping traces, and transforms; preserve content and state changes.

---

## 5. Information architecture

### Routes

- `/` — curated landing page and selected work.
- `/work` — project index with domain filters.
- `/work/[slug]` — editorial case study.
- `/about` — working philosophy, capabilities, tools, and verified experience.
- `/contact` — direct contact and social links.
- Optional `/lab` — experiments only after the core portfolio is complete.

### Navigation

Persistent, compact navigation:

- Bunny Yadav / system builder
- Work
- About
- Contact
- Current availability indicator (only if accurate)

On mobile, use a simple disclosure menu with a visible close control and focus trapping.

### Primary flow

`Entry → Positioning → Selected work → Deep case study → Capabilities → Contact`

Secondary flow: `GitHub verification` from every project and the about section.

---

## 6. Page requirements

### 6.1 Home / entry

**Goal:** establish identity and visual world in 5–10 seconds.

Required content:

- Name: Bunny Yadav.
- Role: AI/ML Engineer · Data Scientist · Full-Stack Developer (final wording to verify).
- One specific positioning statement.
- Primary CTA: **Explore selected work**.
- Secondary CTA: **Connect on LinkedIn** or **Open GitHub**.
- Small metadata line: domains and current focus.

Signature interaction: a responsive **signal-to-system sculpture**. Four input traces (image, audio, health data, financial features) converge into a calm modular form. Hovering or keyboard-focusing a project changes one trace and reveals a short label. The scene must never block the headline or CTA.

Fallback: a static SVG/Canvas composition showing the same traces and labels.

### 6.2 Selected work

Feature four projects with intentionally different treatments:

1. **Multi-Disease AI** — flagship, full-width system narrative.
2. **Emotion Recognition System** — audio waveform and real-time inference story.
3. **Credit Scoring Model** — compact analytical case with metric and trade-off emphasis.
4. **Handwritten Recognition** — focused computer-vision study showing the path from input image to classification.

Each project must show title, domain, year, role, one-line premise, verified stack, evidence/metric where available, and a route to source code or demo.

Do not fabricate clients, users, production status, or outcomes. Labels such as “production-ready” must be supported by deployment evidence.

### 6.3 Featured case study

Default candidate: **Multi-Disease AI**. Before publication, confirm the scope and claims in the repository.

Narrative structure:

1. Context: why multimodal health signals create a difficult product problem.
2. Problem: fragmented inputs and the need for understandable predictions.
3. Objective: define the intended user and decision—not only model accuracy.
4. Strategy: data flow, model choices, API boundary, and explainability.
5. Experiments: alternatives, failures, and evaluation approach.
6. Final system: interface, inference path, and deployment shape.
7. Technical execution: React, FastAPI, PyTorch, Docker, databases, and observability where verified.
8. Outcome: measured result, demo behavior, or clearly labeled prototype outcome.
9. Reflection: what would be improved with better data, validation, or clinical collaboration.

Use diagrams, selected screenshots, model cards, and short annotations. Avoid a long unbroken wall of prose.

### 6.4 About

Write in first person and keep it evidence-led. Include:

- professional identity;
- the kinds of problems Bunny likes to make legible;
- capabilities grouped into **Intelligence**, **Product**, and **Delivery**;
- verified experience and education only;
- current learning areas: transformers, multimodal learning, MLOps, distributed systems, and explainable AI;
- working principles and interests.

### 6.5 Contact

The final interaction should take one step:

- `ybunny500@gmail.com` (verify before launch);
- LinkedIn;
- GitHub;
- optional “Tell me what you’re building” CTA using a `mailto:` link.

No required contact form in v1.

---

## 7. Content model

```ts
type Project = {
  slug: string;
  title: string;
  domain: 'healthcare' | 'audio' | 'finance' | 'computer-vision' | 'web';
  year?: string;
  role: string;
  summary: string;
  premise: string;
  status: 'prototype' | 'experiment' | 'deployed';
  thumbnail: string;
  hero?: string;
  gallery?: string[];
  githubUrl: string;
  demoUrl?: string;
  stack: string[];
  metric?: { label: string; value: string; context: string };
  caseStudy?: {
    context: string;
    problem: string;
    objective: string;
    strategy: string;
    process: string[];
    solution: string;
    technicalExecution: string;
    outcome: string;
    reflection: string;
  };
};
```

Content lives independently from components. Every public claim should have a source, repository link, demo, or an explicit `prototype` label.

---

## 8. Technical architecture

Recommended implementation: **Next.js App Router + TypeScript**, with CSS tokens and a small component system. Use React Three Fiber only for the progressive hero layer; keep project pages primarily semantic HTML and optimized media.

```text
app/
  layout.tsx
  page.tsx
  work/page.tsx
  work/[slug]/page.tsx
  about/page.tsx
  contact/page.tsx
components/
  navigation/
  layout/
  project/
  case-study/
  ui/
3d/
  SignalField.tsx
  materials.ts
  lighting.ts
  fallback.tsx
motion/
  transitions.ts
  reduced-motion.ts
content/
  projects.ts
  profile.ts
lib/
  device.ts
  performance.ts
  metadata.ts
styles/
  tokens.css
  globals.css
public/
  images/
  models/
```

### Component requirements

Create reusable, purposeful primitives: `Container`, `Section`, `ProjectTeaser`, `ProjectMeta`, `CaseStudySection`, `Metric`, `Reveal`, `SignalField`, `SceneFallback`, `ProjectNavigation`, and `Footer`.

### 3D requirements

- Prefer procedural geometry or lightweight SVG/Canvas over large model files.
- Cap device pixel ratio at 1.5 on desktop and 1 on constrained/mobile devices.
- Use one key, one fill, and one restrained rim light.
- Pause or simplify when offscreen, hidden, battery-constrained, or `prefers-reduced-motion` is enabled.
- Do not load WebGL before primary text and navigation are interactive.
- Dispose geometries, materials, textures, and event listeners on unmount.
- Provide a static fallback for unsupported WebGL, failed assets, and slow connections.

---

## 9. Performance budgets

Initial targets for the home page:

- Largest Contentful Paint: **≤ 2.5s** on a mid-range mobile connection.
- Interaction to Next Paint: **≤ 200ms** for primary interactions.
- Cumulative Layout Shift: **≤ 0.1**.
- Initial JavaScript: **≤ 170KB compressed**, excluding lazy 3D code.
- Hero enhancement: lazy-loaded and independently chunked.
- Images: responsive AVIF/WebP, explicit dimensions, lazy-loaded below the fold.
- No autoplay video in the first viewport.

Measure with Lighthouse, WebPageTest, and a real low-power mobile device before launch.

---

## 10. Accessibility and resilience

- Semantic landmarks and one clear `h1` per route.
- Full keyboard access to navigation, project links, hero controls, and interactive diagrams.
- Visible `:focus-visible` styles with sufficient contrast.
- Every project image has meaningful alternative text or is marked decorative.
- Do not encode important information only in color, motion, or 3D.
- Respect `prefers-reduced-motion` and provide a user-facing motion toggle if the hero is interactive.
- Provide a skip link and descriptive link labels.
- Preserve readable content when JavaScript, WebGL, fonts, or external analytics fail.
- Use `mailto:` and external links with clear accessible names.

---

## 11. Analytics and privacy

For v1, prefer privacy-conscious, cookie-free measurement or no analytics until content is validated. If added, measure only:

- project opens;
- case-study depth/completion;
- GitHub and LinkedIn outbound clicks;
- contact CTA clicks;
- WebGL fallback rate.

Do not collect sensitive health, financial, or user-entered data through the portfolio.

---

## 12. Delivery phases

### Phase 1 — Discovery and verification

- Confirm preferred title, bio, email, availability, education, experience, and project claims.
- Audit each selected repository for screenshots, demos, metrics, architecture, and licensing.
- Select the flagship case study.

### Phase 2 — Art direction and prototype

- Create type, color, layout, and motion tokens.
- Prototype the signal-field hero with a static fallback.
- Test the concept without color and without 3D to ensure the layout remains distinctive.

### Phase 3 — Content and interface

- Build content schema and project index.
- Implement home, work, case study, about, and contact routes.
- Add responsive compositions before enhancement effects.

### Phase 4 — Integration and polish

- Connect GitHub/demo links.
- Add motion and hover relationships.
- Validate desktop, tablet, mobile, keyboard, reduced motion, and no-WebGL modes.

### Phase 5 — Launch review

Review as creative director, hiring manager, frontend engineer, accessibility reviewer, mobile user, and performance engineer. Remove any effect that does not improve comprehension, hierarchy, or evidence.

---

## 13. Acceptance criteria

### Product

- A new visitor can identify Bunny’s role and focus within 10 seconds.
- Four projects are discoverable without scrolling through a generic grid.
- At least one project explains context, decisions, technical execution, and outcome.
- Contact and verification links are reachable from every route.

### Design

- The signal/system concept is recognizable without relying on color gradients or 3D.
- Typography, spacing, metadata, and project compositions form a consistent system.
- No repeated decorative animation, meaningless glass, or template-like card wall.

### Engineering

- Project content is data-driven.
- The hero is lazy-loaded, capped, disposable, and has a static fallback.
- Routes render useful semantic content without WebGL.
- Performance and accessibility budgets are tested on mobile hardware.

### Content integrity

- All professional claims are verified by Bunny.
- Prototype, experiment, and deployed work are clearly differentiated.
- Metrics include context; no unsupported accuracy or production claims are published.

---

## 14. Open questions before implementation

1. What exact role/title should appear under Bunny’s name?
2. Which projects have a working demo, deployment, or screenshots?
3. What are the verified years, education, internships, employment, and awards?
4. Which project has the strongest end-to-end story for the flagship case study?
5. Are the email and LinkedIn URLs current and intended for public contact?
6. Should the portfolio be a personal site, GitHub Pages site, or independently deployed application?
7. Are there brand, accessibility, or privacy constraints from any target employer or client?

---

## Launch definition

The portfolio is ready when it communicates a specific point of view—**intelligent systems made understandable**—even with the 3D layer disabled, while the enhanced experience rewards deeper exploration without slowing or confusing the visitor.
