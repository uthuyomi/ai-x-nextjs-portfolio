# AI-Human Collaboration: A Review of the Development Process

## 1. Scope of Human Contribution

While the project heavily relied on AI support, the human side was responsible for initiating structure, understanding API behavior, resolving TypeScript conflicts, and validating the final UI logic. At key stages, especially when the logic became abstract (e.g., `filterPosts`, category handling, and props typing), I had to read through what AI proposed and make sense of it before approving or adjusting.

My understanding of props usage, data flow, and component typing was still in development during the project. Despite that, I actively guided the AI with prompts and made decisions on code style, structure, and naming conventions.

## 2. Role of AI Assistance

AI was primarily responsible for:

- Generating component and page code in React + TypeScript
- Suggesting fixes to type mismatches and runtime errors
- Supporting me in debugging and interpreting errors
- Structuring the file hierarchy and naming
- Providing guidance on best practices

The assistant helped me bridge my understanding gap—especially in areas like optional chaining, conditional rendering, and the use of `.map()` with properly typed props.

## 3. Learning Points

- **Type definition is key.** TypeScript will break down if types are loosely defined or mismatched. I experienced firsthand how a wrong type (`Posts` vs `Post`) creates a chain of failures in child components.
- **Naming consistency matters.** Case mismatches in filenames (e.g., `About.tsx` vs `about.tsx`) caused avoidable confusion.
- **Understanding data structure is crucial.** WordPress API's `_embedded` structure for featured images was confusing at first, but once clarified, it enabled safe image loading using optional chaining.
- **Even AI-generated code requires human review.** There were cases where the code _looked_ right but needed logical validation—especially with category-based filtering or conditional rendering.

## 4. Reflection

This was my first structured attempt at building a React + TypeScript site with dynamic content (WordPress API). While I’m not yet fluent in all the patterns used, I’m more confident now in reading, questioning, and adapting AI-generated code.

More than just “copy-paste,” this was an iterative process of understanding, questioning, and learning.

> I believe AI can accelerate development, but growth comes from actively engaging with what it writes.

In future iterations, I plan to handle responsive design, refine accessibility, and better document components.
