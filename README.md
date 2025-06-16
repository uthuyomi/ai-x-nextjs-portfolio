# AI-Human Collaboration: Building a Next.js + TypeScript Portfolio

_This document outlines the development experience of creating a Next.js + TypeScript portfolio site in collaboration with AI. It is part of the `/review/` folder of the `ai-x-nextjs-portfolio` repository._

---

## 1. Human Contribution

While AI provided extensive support, I led the project direction by:

- Understanding the WordPress REST API response structure
- Defining types (`Post`, `Category`) and correcting mismatches
- Structuring `props` and component communication
- Debugging logic and runtime errors
- Making architectural and naming decisions

Especially in logic-heavy parts like category-based filtering and `_embedded` image handling, I needed to read and interpret what the AI generated before implementing it.

---

## 2. Role of AI Assistance

AI was instrumental in:

- Generating component/page templates in React with Next.js and TypeScript
- Suggesting fixes for type and runtime errors
- Providing examples for `.map()`, conditional rendering, and optional chaining
- Structuring the file hierarchy and naming strategy
- Offering guidance on best practices for static generation and API integration

The assistant helped bridge my gaps—especially around type safety, data flow, and rendering logic.

---

## 3. Key Learnings

- **Type safety is critical.** A single mismatch (`Posts[]` vs `Post[]`) can cause failures in multiple components.
- **Case sensitivity matters.** Files like `about.tsx` vs `About.tsx` can break builds depending on OS or config.
- **API responses require careful handling.** The WordPress `_embedded` format demands safe access patterns.
- **AI-generated code is not always final.** Even clean code suggestions must be logically validated and adapted.

---

## 4. Reflection

This project marks my first structured attempt at building a dynamic portfolio site using:

- ✅ Next.js
- ✅ TypeScript
- ✅ WordPress REST API
- ✅ Static generation with `getStaticProps`

Although I'm still solidifying my React and TypeScript understanding, I’m more confident in reading AI output, asking better questions, and iterating logically.

> This wasn't a passive build—it was an active collaboration and a structured learning process.

In future iterations, I plan to:

- Implement responsive design for smartphones
- Improve accessibility and semantic markup
- Enhance component modularity and documentation

---

_This reflection is part of the `ai-x-nextjs-portfolio` GitHub repository._
