# AI-Human Collaboration: A Review of the Development Process

_This document reflects my personal experience working on a React + TypeScript project with AI support. It is part of the `/review/` folder in the `ai-x-react-portfolio` repository._

---

## 1. Scope of Human Contribution

While the project heavily relied on AI support, the human side was responsible for initiating structure, understanding API behavior, resolving TypeScript conflicts, and validating the final UI logic. At key stages—especially when the logic became abstract (e.g., `filterPosts`, category handling, and props typing)—I had to read through what the AI proposed and decide whether to approve, adapt, or reject it.

My understanding of props usage, data flow, and component typing was still in development during the project. Despite that, I actively guided the AI with prompts and made all architectural and naming decisions.

---

## 2. Role of AI Assistance

AI was primarily responsible for:

- Generating React + TypeScript components and pages
- Suggesting fixes for type mismatches and runtime errors
- Supporting debugging and error interpretation
- Proposing file structure and naming conventions
- Offering guidance on best practices and edge cases

The assistant helped bridge my gaps—especially in areas like optional chaining, conditional rendering, and using `.map()` with typed props.

---

## 3. Learning Points

- **Type definitions are critical.** TypeScript fails fast when types are mismatched or loosely defined. I saw firsthand how a wrong type (`Posts` vs `Post`) can break downstream components.
- **Naming consistency matters.** Filename case mismatches (e.g., `About.tsx` vs `about.tsx`) caused subtle yet impactful issues in the dev environment.
- **Understanding the data structure is key.** The WordPress API's `_embedded` response format was initially confusing, especially for featured images. With guidance, I safely implemented fallback logic using optional chaining.
- **AI-generated code still requires review.** Code that "looks right" can still be logically wrong. Human validation was essential—especially for dynamic filtering and conditional UI states.

---

## 4. Reflection

This was my first structured attempt at building a React + TypeScript site powered by dynamic content (WordPress API). While I'm still solidifying my grasp of advanced patterns, I've become more confident in reading, questioning, and adapting AI-generated output.

This wasn’t just copy-paste—it was an iterative cycle of learning, verifying, and restructuring.

> AI accelerates development, but growth happens through deliberate understanding.

In future iterations, I plan to handle responsive design, improve accessibility, and document component logic more clearly.

---

_This review is part of the `ai-x-react-portfolio` GitHub repository._
