# Project Architecture – React Blog Archive

## Page Structure

- `/` → Home page
- `/archive` → Blog archive page (with category filter via `useRouter`)
- `/blog/[slug]` → Single blog post (not yet implemented)

## Component Structure

- `Header` – navigation links
- `ArchiveItem` – loops through posts and renders article cards
- `Category` – category-based filtering (planned)

## Data Flow

- `getStaticProps` fetches data from WordPress API
- `posts` passed via props
- `ArchiveItem` receives filtered posts
- Category ID from URL determines filtering logic

## Styling

- SCSS modules are used (`archive.module.scss`)
- Responsive design not yet implemented
